This page attempts to document the features that various MQTT servers (brokers) support. This is specific to their MQTT support; many of these servers have much wider capabilities beyond just MQTT.

# Capabilities


Server                                                                            | QoS 0 | QoS 1 | QoS 2 | auth | [bridge](bridge_protocol) | [$SYS](conventions#$sys) | SSL | [dynamic topics](are_topics_dynamic) | cluster | websockets | plugin system
------                                                                            | ----- | ----- | ----- | ---- | ------------------------- | ------------------------ | --- | ------------------------------------ | ------- | ---------- | ------------- | 
[mosquitto](mosquitto_message_broker)                                             | ✔     | ✔     | ✔     | ✔    | ✔                         | ✔                        | ✔   | ✔                                    | §       | ✔          | ✔             | 
[RSMB](Really-Small-Message-Broker)                                               | ✔     | ✔     | ✔     | ✔    | ✔                         | ✔                        | ✘   | ✔                                    | ✘       | ✘          | ?             | 
[WebSphere MQ](http://www-03.ibm.com/software/products/en/wmq/)                   | ✔     | ✔     | ✔     | ✔    | ✔                         | ✔                        | ✔   | ✔                                    | ?       | ?          | ?             | 
[HiveMQ](http://www.hivemq.com)                                                   | ✔     | ✔     | ✔     | ✔    | ✔                         | ✔                        | ✔   | ✔                                    | ✔       | ✔          | ✔             | 
[Apache Apollo](http://activemq.apache.org/apollo)                                | ✔     | ✔     | ✔     | ✔    | ✘                         | ✘                        | ✔   | ✔                                    | ?       | ✔          | ?             | 
[Apache ActiveMQ](http://activemq.apache.org/)                                    | ✔     | ✔     | ✔     | ✔    | ✘                         | ✘                        | ✔   | ✔                                    | ✔       | ✔          | ✔             | 
[Software AG Universal Messaging](http://um.terracotta.org/#page/%2Fum.terracotta.org%2Funiversal-messaging-webhelp%2Fto-mqttoverview.html%23) | ✔     | ✔     | ✔     | ✔    | ✘                         | ✘                        | ✔   | ✔                                    | ✔       | rm          | ✘             | 
[RabbitMQ](http://www.rabbitmq.com/blog/2012/09/12/mqtt-adapter/)                 | ✔     | ✔     | ✘     | ✔    | ✘                         | ✘                        | ✔   | ✔                                    | ?       | ?          | ?             | 
[Solace](http://dev.solacesystems.com/tech)                                       | ✔     | ✔     | ✘     | ✔    | §                         | ✔                        | ✔   | ✔                                    | ✔       | ✔          | ✘             | 
[MQTT.js](https://github.com/mqttjs/MQTT.js)                                      | ✔     | ✔     | ✔     | §    | ✘                         | ✘                        | ✔   | ✔                                    | ✘       | ✔          | ✘             | 
[moquette](https://github.com/andsel/moquette)                               | ✔     | ✔     | ✔     | ✔    | ?                         | ?                        | ✔   | ?                                    | **rm**       | ✔          | ✘             | 
[mosca](mosca)                                                                    | ✔     | ✔     | ✘     | ✔    | ?                         | ?                        | ?   | ?                                    | ✘       | ✔          | ✘             | 
[IBM MessageSight](http://www-03.ibm.com/software/products/en/messagesight/)      | ✔     | ✔     | ✔     | ✔    | ✘                         | ✔                        | ✔   | ✔                                    | §       | ✔          | ✘             |
[2lemetry](http://2lemetry.com/platform/)                                         | ✔     | ✔     | ✔     | ✔    | ✔                         | §                        | ✔   | ✔                                    | ✔       | ✔          | ✘             |
[GnatMQ](http://mqttbroker.codeplex.com/)                                         | ✔     | ✔     | ✔     | ✔    | ✘                         | ✘                        | ✘   | ✔                                    | ✘       | ✘          | ✘             |
[JoramMQ](http://mqtt.jorammq.com)                                                | ✔     | ✔     | ✔     | ✔    | ✔                         | ✔                        | ✔   | ✔                                    | ✔       | ✔          | ✔             | 
[ThingMQ](http://thingmq.com)                                                    | ✔     | ✔     | ✔     | ✔    | ✔                         | ✘                        | ✔   | ✔                                    | ✔       | ✔          | ✔             | 
[VerneMQ](https://verne.mq)                                                       | ✔     | ✔     | ✔     | ✔    | ✔                         | ✔                        | ✔   | ✔                                    | ✔       | ✔          | ✔             | 
[emqttd](http://emqtt.io)                                                       | ✔     | ✔     | ✔     | ✔    | ✔                         | ✔                        | ✔   | ✔                                    | ✔       | ✔          | ✔             | 
[HBMQTT](https://github.com/beerfactory/hbmqtt)                                   | ✔     | ✔     | ✔     | ✔    | ✘                         | ✔                        | ✔   | ✔                                    | ✘       | ✔          | ✔             | 
[Mongoose](https://github.com/cesanta/mongoose)                                   | ✔     | ✔     | ?     | ?    | ?                         | ?                        | ?   | ?                                    | ?       | ?          | ?             | 
[emitter](https://github.com/emitter-io/emitter)                                   | ✔     | §     | ✘     | ✔    | ✘                         | ✘                        | ✔   | ✔                                    | ✔       | ✔          | ✘             | 
[Bevywise IoT Platform](https://www.bevywise.com/)                                | ✔     | ✔     | ✔     | ✔    | **rm**                     | ✔                        | ✔   | ✔                                    | **rm**  | ✔          | **rm**        | 


Key: ✔ supported ✘ not supported ? unknown § see limitations **rm** roadmap (planned)
# Limitations


*  MQTT.js  will accept connections with username and password supplied, but do not actually authenticate the connection

* IBM MessageSight supports a High-Availability mode which provides the redundancy advantage of a cluster, but does not support any sort of load balancing for MQTT.

* 2lemetry uses domains, where the first topic segment is the domain name. The `$SYS` topic space is under the domain (i.e. `com.example/$SYS/#`)

* Solace does provide a proprietary bridge solution between brokers.

* mosquitto clustering is achieved on backend level (redis, amqp, etc).

* Software AG Universal Messaging provides Active/Active clustering (over a proprietary protocol) and bridging (over a proprietary protocol).

Potentially should add columns to track: LWT; additional protocols (WMQ, AMQP, MQTTs etc)

_This is in need of expanding. Please add known information about known brokers to this table and include any known limitations below it._