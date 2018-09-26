> Note: although there are a range of options available for developers interested in MQTT,
not all of the client APIs listed below are current. Some are at an early or experimental stage of
development, whilst others are stable and mature. Additionally, some may not provide full support 
for all of the features of the latest MQTT specification – for example, some may only support QoS 0, 
not include authentication, etc.


Check with the provider for the current status of your preferred language implementation; and remember to respect the licenses that different implementations are published under.

#### Device-Specific

*  [Arduino](https://github.com/knolleary/pubsubclient) ([more information](http://pubsubclient.knolleary.net/))

*  [Espduino](https://github.com/tuanpmt/espduino) (tailored Arduino library for the ESP8266)

*  [mbed](https://github.com/yilun/MQTT-client-on-mbed) ([more information](http://ceit.uq.edu.au/content/mqttclient-mbed-version-20))

*  [mbed (simple port of the Arduino pubsubclient)](http://mbed.org/users/jwende/code/MQTT/)

*  [mbed (native implementation)](http://mbed.org/users/Nim65s/code/niMQTT/)

*  [mbed (Paho Embedded C++ port)](http://developer.mbed.org/teams/mqtt/code/MQTT/) ([more information](https://www.eclipse.org/paho/clients/c/embedded/))
*  [mbed (Paho Embedded C port)](http://developer.mbed.org/teams/mqtt/code/MQTTPacket/) ([more information](https://www.eclipse.org/paho/clients/c/embedded/))

*  [Nanode](http://github.com/njh/NanodeMQTT/)

*  [Netduino](https://github.com/danielan/NetduinoMQTT)

*  [M2MQTT (works with .Net Micro Framework)](https://github.com/eclipse/paho.mqtt.m2mqtt)

(see also [devices](things) page for more on hardware with built-in support)

#### Actionscript

*  [as3MQTT](https://github.com/yangboz/as3MQTT)

#### Bash

* see [Shell Script](#shell-script), below

#### C

*  [Eclipse Paho C](https://www.eclipse.org/paho/clients/c/)

*  [Eclipse Paho Embedded C](https://www.eclipse.org/paho/clients/c/embedded/)

*  [libmosquitto](http://mosquitto.org)

*  [libemqtt](https://github.com/menudoproblema/libemqtt) - an embedded C client

*  [MQTT-C](https://github.com/LiamBindle/MQTT-C) - A portable MQTT C client for embedded systems and PCs alike. 

*  [wolfMQTT](https://github.com/wolfSSL/wolfMQTT) - Embedded C client
*  [MQTT over lwIP](https://gitlab.com/rts_nepal/embedded/lwIP_mbedtls_mqtt_c) - MQTT C client for embedded systems using FreeRTOS, lwIP and mbedtls

#### C++

*  [Eclipse Paho C++](https://www.eclipse.org/paho/clients/cpp/)

*  [libmosquittopp](http://mosquitto.org)

*  [Eclipse Paho Embedded C++](https://www.eclipse.org/paho/clients/c/embedded/)

#### Clojure

*  [Machine Head](http://clojuremqtt.info)

*  [Clojure MQTT Codec for Netty](https://github.com/xively/clj-mqtt/)

#### Dart

*  [mqtt.dart](http://pub.dartlang.org/packages/mqtt)

#### Delphi

*  [TMQTTClient](http://jamiei.com/code/TMQTTClient.zip) ([more information](http://jamiei.com/blog/code/mqtt-client-library-for-delphi/))

#### Erlang

*  [erlmqtt](https://github.com/squaremo/erlmqtt)

*  [emqttc](https://github.com/emqtt/emqttc) - Erlang MQTT Client

*  [mqtt4erl](http://code.google.com/p/mqtt4erl/)

*  [my-mqtt4erl](http://code.google.com/p/my-mqtt4erl/) - updated fork of mqtt4erl

#### Elixir

*  [hulaaki](https://github.com/suvash/hulaaki) - An Elixir library (driver) for clients communicating with MQTT brokers(via the MQTT 3.1.1 protocol).

*  [Exmqttc](https://github.com/timbuchwaldt/exmqttc) - Elixir wrapper for the emqttc library.

#### Go

*  [Eclipse Paho Go](https://github.com/eclipse/paho.mqtt.golang)
*  [mqtt by jeffallen](https://github.com/jeffallen/mqtt)

#### Haskell

* [mqtt-hs](http://hackage.haskell.org/package/mqtt-hs)

#### Java

*  [Eclipse Paho Java](https://www.eclipse.org/paho/clients/java/)

*  [Xenqtt](https://github.com/TwoGuysFromKabul/xenqtt)[documentation](http://xenqtt.sf.net/) Includes a client library, mock broker for unit/integration testing, and applications to support enterprise needs like using a cluster of servers as a single client, an HTTP gateway, etc.

*  [MeQanTT](https://github.com/AlbinTheander/MeQanTT)

*  [Fusesource mqtt-client](https://github.com/fusesource/mqtt-client)

*  [moquette](https://github.com/andsel/moquette)

*  [ "MA9B" zip of 1/2 dozen mobile clients source code. Includes Android-optimized Java source that works with Android notifications, based on Paho](http://www-933.ibm.com/support/fixcentral/swg/selectFix?product=ibm%2FWebSphere%2FWebSphere+MQ&fixids=1.0.0.1-WS-MQCP-MA9B&source=dbluesearch&function=fixId&parent=ibm/WebSphere )

*  [IA92](http://www-01.ibm.com/support/docview.wss?rs=171&uid=swg24006006&loc=en_US&cs=utf-8&lang=en) - *deprecated* IBM IA92 support pack, use Eclipse Paho GUI client instead. A useful MQTT Java swing GUI for publishing & subscribing. The Eclipse Paho GUI is identical but uses newer client code

* [vertx-mqtt-client](https://github.com/vert-x3/vertx-mqtt-client) is an open-source, high performance, non-blocking MQTT client built as a part of vert.x's jvm toolkit.

* [Qatja](https://github.com/Qatja) is a Java client library for MQTT 3.1.1 with specific implementation for Android and Processing

#### Javascript / Node.js

*  [Eclipse Paho HTML5 JavaScript over WebSocket.](https://github.com/eclipse/paho.mqtt.javascript)

*  [mqtt.js](https://github.com/adamvr/MQTT.js)

*  [node_mqtt_client](https://github.com/yilun/node_mqtt_client) ([more information](http://ceit.uq.edu.au/content/simple-mqtt-cient-nodejs))

*  [IBM-provided PhoneGap / Apache Cordova MQTT plug-in for Android](http://www-01.ibm.com/support/docview.wss?rs=171&uid=swg24033580&loc=en_US&cs=utf-8&lang=en) - JavaScript API is identical to Eclipse Paho HTML5 JavaScript

*  [Ascoltatori](https://github.com/mcollina/ascoltatori) - a node.js pub/sub library that allows access to Redis, AMQP, MQTT and ZeroMQ with the same API.

#### LotusScript

*  [MQTT From LotusScript](https://tingenek.wordpress.com/2011/11/30/mqtt-with-lotus-notes/)

#### Lua

*  [Eclipse Paho Lua](http://git.eclipse.org/c/paho/org.eclipse.paho.mqtt.lua.git/)

#### .NET / dotNET

*  [Paho.MqttDotnet](https://github.com/xljiulang/Paho.MqttDotnet/)

*  [MQTTnet](https://github.com/chkr1011/MQTTnet)

*  [MqttDotNet](http://sourceforge.net/projects/mqttdotnet/)

*  [nMQTT](https://github.com/markallanson/nmqtt)

*  [M2MQTT](https://github.com/eclipse/paho.mqtt.m2mqtt)

*  [KittyHawkMQ](https://github.com/mFourLabs/KittyHawkMQ)

*  [StriderMqtt](https://github.com/ericvoid/StriderMqtt)

*  [xamarin mqtt](https://github.com/xamarin/mqtt)

#### Objective-C

*  [mqttIO-objC](https://github.com/GrayWang/mqttIO-objC)

*  [libmosquitto](https://mosquitto.org) - via wrappers ([example](https:///github.com/njh/marquette))

*  [MQTTKit](https://github.com/jmesnil/MQTTKit) ([sample app](https:///github.com/jmesnil/MQTTExample))

*  ["MA9B" zip of 1/2 dozen mobile clients source code including Objective-C](http://www-933.ibm.com/support/fixcentral/swg/selectFix?product=ibm%2FWebSphere%2FWebSphere+MQ&fixids=1.0.0.1-WS-MQCP-MA9B&source=dbluesearch&function=fixId&parent=ibm/WebSphere)

#### OCaml

* [ocaml-mqtt](https://github.com/j0sh/ocaml-mqtt)

* [mqtt_client](https://github.com/philtomson/mqtt_client)

#### Perl

*  [net-mqtt-perl](https://github.com/beanz/net-mqtt-perl)

*  [anyevent-mqtt-perl](https://github.com/beanz/anyevent-mqtt-perl)

*  [WebSphere-MQTT-Client](http://search.cpan.org/dist/WebSphere-MQTT-Client/)

*  Net::MQTT::Simple [cpan](https://metacpan.org/pod/Net::MQTT::Simple) [github](https://github.com/Juerd/Net-MQTT-Simple)

#### PHP

*  [phpMQTT](http://github.com/bluerhinos/phpMQTT)

*  [Mosquitto-PHP](https://github.com/mgdm/Mosquitto-PHP)

*  [sskaje's MQTT library](http://github.com/sskaje/mqtt)

#### Python

*  [Eclipse Paho Python](https://github.com/eclipse/paho.mqtt.python) - originally the mosquitto Python client

* [gmqtt](https://github.com/wialon/gmqtt)

*  [nyamuk](https://github.com/iwanbk/nyamuk)

*  [MQTT for twisted python](https://github.com/adamvr/MQTT-For-Twisted-Python)

*  [HBMQTT](https://github.com/beerfactory/hbmqtt)

#### REXX

*  [REXX MQTT](https://github.com/DougieLawson/REXX_MQTT)

#### Prolog

*  [MQTT Pack](https://github.com/olsky/swi-mqtt-pack) - Mosquitto library as a SWI-Prolog pack

#### Ruby

*  [ruby-mqtt](https://github.com/njh/ruby-mqtt)

*  [em-mqtt](https://rubygems.org/gems/em-mqtt)

*  [mosquitto](https://github.com/xively/mosquitto)

#### Qt

* [qmqtt](https://github.com/emqtt/qmqtt) - MQTT Client for Qt

#### Shell Script

*  [bish-bosh](https://github.com/raphaelcohn/bish-bosh), supports bash, ash (including BusyBox), pdksh and mksh.

#### Smalltalk

* [MQTT client for Squeak](http://www.squeaksource.com/MQTTClient.html), for Squeak 5.1

#### Swift

* [CocoaMQTT](https://github.com/emqtt/CocoaMQTT) - An MQTT client for iOS and OS X written with Swift

#### Tcl

*  [tcl-mqtt](https://github.com/Tingenek/tcl-mqtt)