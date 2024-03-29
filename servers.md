# Servers/Brokers

### For more information on brokers0

*  [compare the capabilities](server-support) of different brokers
*  see some of the [public brokers](public_brokers) available for testing on the wiki

***

## Apache ActiveMQ

Details of “classic” [ActiveMQ’s](http://activemq.apache.org/index.html) support for MQTT are available [here](http://activemq.apache.org/mqtt.html).

## Apache ActiveMQ Artemis

The “next generation” of ActiveMQ, [Artemis](http://activemq.apache.org/artemis/) is a multi protocol messaging broker that supports MQTT.

## Bevywise MQTT Broker

[MQTTRoute](https://www.bevywise.com/mqtt-broker/) is a high performance broker.  The [Secure MQTT Broker](https://www.bevywise.com/mqtt-broker/) is written in C & Python and works with all standard MQTT Clients. Bevywise MQTT Broker has a FREE and affordable premium version. MQTTRoute can be customized to write data to any data store using [standard connectors](https://github.com/bevywise-networks/) or custom implementations. Try the [publicly hosted MQTTRoute](http://mqttroute.com/)

## Emitter 

[Emitter](https://emitter.io) is clustered and open-source MQTT broker, written entirely in Go. It proposes several additional features on top of a traditional MQTT broker, as it includes custom per-topic security and shared-nothing scalable architecture which helps you avoid single points of failure. Full source-code available on [GitHub](https://github.com/emitter-io/emitter).

## emqttd

[emqttd](https://github.com/emqtt/emqttd) is a distributed, massively scalable, highly extensible MQTT message broker written in Erlang/OTP. [emqtt.io](http://emqtt.io/) / [@emqtt](https://twitter.com/emqtt)

emqttd is fully open source and licensed under the Apache Version 2.0. EMQ implements both MQTT V3.1 and V3.1.1 protocol specifications, and supports MQTT-SN, CoAP, WebSocket, STOMP and SockJS at the same time.

emqttd provides a scalable, reliable, enterprise-grade MQTT message Hub for IoT, M2M, Smart Hardware and Mobile Messaging Applications. The 1.0 release of the emqttd broker has scaled to 1.3 million concurrent MQTT connections on a 12 Core, 32G CentOS server.

## Eurotech Everywhere Device Cloud

[Eurotech Everywhere Device Cloud](http://www.eurotech.com/en/solutions/device+to+cloud/mqtt+protocol) is a cloud-based service provided by [Eurotech](http://www.eurotech.com).

## flespi
[flespi](https://flespi.com/mqtt-broker) is a public and free cloud-based MQTT broker service with declared 3.1, 3.1.1, 5.0 protocols compliance. High-volume targeted architecture, isolated MQTT namespace, WebSockets/SSL support, configurable ACL, commercial and free SLA, managed by [HTTP REST API](https://flespi.io/mqtt). 

## HBMQTT

[HBMQTT](https://github.com/beerfactory/hbmqtt) is an open-source implementation of MQTT broker and client. It uses Python 3.4+ asyncio library for providing a mono-threaded, non-blocking implementation of the protocol.

## HiveMQ

[HiveMQ](http://www.hivemq.com/ ) is a MQTT broker which was built from the ground up with maximum scalability and enterprise-ready security in mind. It comes with native web socket support and an open source plugin SDK to extend its functionality or integrate it with other components. A public test server is also available ([more information](public_brokers)).

## Jmqtt

[Jmqtt](https://github.com/Cicizz/jmqtt ) is a MQTT broker which implemented by java and netty,support persistence and cluster.

## IBM Integration Bus

[IBM Integration Bus](http://www-03.ibm.com/software/products/us/en/integration-bus/) V9 has Telemetry feature built-in as optional licensed feature. IBM WebSphere MessageBroker V7 & V8 also include it as optionally licensed feature.

[Really Small Message Broker](http://www.alphaworks.ibm.com/tech/rsmb) 75KB MQTT broker runtime free download as binaries from IBM alphaWorks, RSMB is a C implementation of a tiny MQTT server suitable for development, embedded systems, concentrators or small to medium sized deployments. It provides complete MQTT v3.1 support, bridging, and a C client API.

## IBM WIoTP Message Gateway

[IBM WIoTP Message Gateway](https://developer.ibm.com/iotplatform/messagegateway/) is a scalable, hightly available messaging broker for MQTT (including MQTT v5, HTML5 WebSockets, JMS. Also connects/bridges IBM MQ, IBM Integration Bus. (Was formerly called IBM IoT MessageSight)

## IBM Websphere MQ Telemetry

The Telemetry MQTT feature is built-in optionally licensed feature in 
[WebSphere MQ](http://www-01.ibm.com/software/integration/wmqfamily/telemetry/ ) version 7.1 and above. It provides full MQTT v3.1 support, IBM MQ and JMS support. IBM WebSphere MQ Advanced includes the MQTT license at no charge. It ships with reference Java (MIDP and above), C and JavaScript (MQTT over WebSocket) clients.

## JoramMQ

[JoramMQ](http://mqtt.jorammq.com) is an offering by ScalAgent providing a message broker that fully supports MQTT 3.1, JMS 2.0, and AMQP 1.0. Interoperability between these standards is ensured by the message broker. MQTT can be used over TCP/IP, TLS (SSL), WebSocket, and secure WebSocket. JoramMQ is particularly appropriate for applications that need to scale with the number of MQTT clients while allowing the publishers to reliably transmit a large volume of messages with a low latency.

## Litmus Automation Loop

[ Loop](http://litmusautomation.com ) is a cloud based MQTT broker with scalability, high availability and security at core. Loop provides full MQTT 3.1 support and JMS connectivity. It can handle extremely large numbers of connected clients. On the other side it can be connected to any ERP, CRM and enterprise architecture with ESB or NoSQL databases for blazing fast data storage.

## Moquette

[Moquette](https://github.com/andsel/moquette) is a Java MQTT broker based on an eventing model with Netty.

## Mosca

As node.js MQTT broker can [ Mosca](https://github.com/mcollina/mosca ) be plugged on top of Redis, AMQP, MQTT, or ZeroMQ.

## Mosquitto

[Mosquitto](http://mosquitto.org) is an Open Source MQTT server. A public, hosted test server is also available ([more information](public_brokers))

## MyQttHub.com

[MyQttHub.com](https://myqtthub.com) Cloud MQTT platform to build your IoT projects. It includes support for MQTT, MQTT-TLS, Web Interface and REST API for full HTTP+MQTT integration. 

## MQTTnet
[MQTTnet](https://github.com/chkr1011/MQTTnet/) is a .NET library for MQTT based communication. It provides a MQTT client and a MQTT server (broker). 

## MqttWk

[MqttWk](https://github.com/Wizzercn/MqttWk) is a Java MQTT broker based on NutzBoot + Netty + Redis + Kafka(Optional).The broker supports QoS 0, QoS 1 and QoS 2.It uses Netty for the protocol encoding and decoding part.Using NutzBoot to provide dependency injection and attribute configuration, using Redis to implement message caching and clustering, and using Kafka to implement message proxy.

## RabbitMQ

[ RabbitMQ](http://rabbitmq.com/ ) is an AMQP message broker – with an [MQTT plugin](http://www.rabbitmq.com/blog/2012/09/12/mqtt-adapter/) (bundled in version 3.x onwards). A public test server is also available ([more information](public_brokers)).

## Solace

[Solace Message Routers](http://dev.solacesystems.com/tech/) (available as hardware and software) are message brokers that support MQTT, JMS, and REST among other APIs, protocols and qualities of service for enterprise messaging, data collection and web/mobile streaming. They support very high connection counts and throughput with built-in buffering to handle bursty traffic, and offer enterprise-class monitoring, high availability and security.

## SwiftMQ

[SwiftMQ Universal Router](http://www.swiftmq.com/landing/router/index.html) is an enterprise message system with
integrated micro services and realtime streaming analytics platform (SwiftMQ Streams, SwiftMQ Dashboard). It supports MQTT 3.1/3.1.1, AMQP 1.0/0.9.1, JMS 1.1 and is fully interoperable between these protocols. It has a built-in Dynamic Routing Architecture to build large Federated Router Networks and Clusters. SwiftMQ High Availability Router is the High and Continuous Availability version of SwiftMQ Universal Router with active replication and transparent client failover.

## ThingScale IoT message broker

[ThingScale IoT message broker](http://thingscale.io/index_en.html) is a fully-managed IoT messaging service provided by [Sensinics,LLC](http://sensinics.co.jp).
ThingScale provides a messaging system for IoT connected devices. The API is used to retrieve events, users, devices, sessions, and channels in JSON format. ThingScale supports TLS payload encryption, scheme-less and cyclic data sampling, and trigger-based notifications. A 30days trial license is offered free of charge. MQTT is the preferred messaging protocol. [Dev Portal](https://sensinics.atlassian.net/wiki/spaces/TD/pages/76021778/Developer+Portal) & [API Portal](https://thingscale.docs.apiary.io/)

## VerneMQ

[VerneMQ](http://verne.mq) is an enterprise ready, high-performance, distributed MQTT message broker. It scales horizontally and vertically on commodity hardware to support a high number of concurrent publishers and consumers while maintaining low and predictable latency and fault tolerance. VerneMQ plugins can be developed in Erlang, Elixir, Lua, and any programming language that can implement HTTP WebHooks. VerneMQ uses modern broadcast protocols and LevelDB for state replication in a cluster. VerneMQ is Open Source and Apache2 licensed.

## Vert.x MQTT Broker
[Vert.x MQTT Broker](https://github.com/GruppoFilippetti/vertx-mqtt-broker) is an open-source implementation of MQTT server. It implements protocol versions 3.1.1 and 3.1, supports QoS 2, and uses OAuth2 for autentication.
It uses [vert.x](http://vertx.io/) as library for tcp managemnet, non-blocking / actor-model, clustering and auth plugin system.

## Yunba.io

[ Yunba](http://yunba.io/) is a backend cloud platform that provides real-time message dispatch service to mobile applications and devices and uses MQTT as a transport protocol, The services include bi-directional push for Instant-Messaging; real-time analyzing; real-time online monitoring.

## Cassandana
[Cassandana](https://github.com/mtsoleimani/cassandana/) is an open source MQTT message broker which is entirely written in Java. This project began its life as a fork of [Moquette](https://github.com/andsel/moquette) , and later underwent some cleanup, optimization and adding extra features. Now it’s ready to work as an enterprise message broker.
Features: 
    MQTT compliant broker.
    Supports QoS 0, QoS 1 and QoS 2
    TLS (SSL) Encryption
    PostgreSQL, MySQL and MongoDB Authentication and Authorization
    Supports HTTP REST API for Authentication and Authorization
    MQTT message archiver (Silo integrated in Cassandana)
    Easy configurable (YAML based)
    Supports WebSocket

