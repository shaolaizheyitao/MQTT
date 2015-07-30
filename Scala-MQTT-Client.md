MQTT is broker based message queuing system. So to work with MQTT, MQTT Message broker/server required. [Mosquitto](http://mosquitto.org/) is an open source MQTT Broker. In Ubuntu mosquitto can be installed using the command 
```
$ sudo apt-get install mosquitto
```
Eclipse Paho is one mqtt client work well with mosquitto. You may read more about it [here](http://www.eclipse.org/paho/).

MQTT Publisher

```Scala
package main.scala

import org.eclipse.paho.client.mqttv3.MqttClient
import org.eclipse.paho.client.mqttv3.MqttException
import org.eclipse.paho.client.mqttv3.MqttMessage
import org.eclipse.paho.client.mqttv3.persist.MqttDefaultFilePersistence

/**
 *
 * MQTT publisher
 * @author Prabeesh K
 * @mail prabsmails@gmail.com
 *
 */

object Publisher {

  def main(args: Array[String]) {
    val brokerUrl = "tcp://localhost:1883"
    val topic = "foo"
    val msg = "Hello world test data"

    var client: MqttClient = null

    // Creating new persistence for mqtt client
    val persistence = new MqttDefaultFilePersistence("/tmp")

    try {
      // mqtt client with specific url and client id
      client = new MqttClient(brokerUrl, MqttClient.generateClientId, persistence)

      client.connect()

      val msgTopic = client.getTopic(topic)
      val message = new MqttMessage(msg.getBytes("utf-8"))

      while (true) {
        msgTopic.publish(message)
        println("Publishing Data, Topic : %s, Message : %s".format(msgTopic.getName, message))
        Thread.sleep(100)
      }
    }

    catch {
      case e: MqttException => println("Exception Caught: " + e)
    }

    finally {
      client.disconnect()
    }
  }
}

```
MQTT Scala Subscriber
```Scala
package main.scala

import org.eclipse.paho.client.mqttv3._
import org.eclipse.paho.client.mqttv3.persist.MemoryPersistence

/**
 *
 * MQTT subcriber
 * @author Prabeesh K
 * @mail prabsmails@gmail.com
 *
 */

object Subscriber {

  def main(args: Array[String]) {

    val brokerUrl = "tcp://localhost:1883"
    val topic = "foo"

    //Set up persistence for messages 
    val persistence = new MemoryPersistence

    //Initializing Mqtt Client specifying brokerUrl, clientID and MqttClientPersistance
    val client = new MqttClient(brokerUrl, MqttClient.generateClientId, persistence)

    //Connect to MqttBroker    
    client.connect

    //Subscribe to Mqtt topic
    client.subscribe(topic)

    //Callback automatically triggers as and when new message arrives on specified topic
    val callback = new MqttCallback {

      override def messageArrived(topic: String, message: MqttMessage): Unit = {
        println("Receiving Data, Topic : %s, Message : %s".format(topic, message))
      }

      override def connectionLost(cause: Throwable): Unit = {
         println(cause)
       }

      override def deliveryComplete(token: IMqttDeliveryToken): Unit = {

      }
    }

    //Set up callback for MqttClient
    client.setCallback(callback)

  }
}

```
SBT file
```sbt
name := "MQTTScalaClinet"

version := "0.2.0"

scalaVersion := "2.10.3"

libraryDependencies += "org.eclipse.paho" % "mqtt-client" % "0.4.0"

resolvers += "MQTT Repository" at "https://repo.eclipse.org/content/repositories/paho-releases/"
```

MQTT Scala subscriber and publisher code based on eclipse paho library 0.4.0 is available in [github](https://github.com/prabeesh/MQTTScalaClient) with SBT build tool.