# MQTT on iOS

There are a couple of options for using MQTT on iOS. Facebook are doing so (they credit libmosquitto in their native Facebook iOS app, and in the Facebook Messenger app).

* It is possible to use libmosquitto on iOS. [Marquette](https://github.com/njh/marquette) is an example iOS app (with source) to control a Nanode.

~~There is also an [Objective-C implementation of a client](https://github.com/m2mIO/mqttIO-objC) from the m2m.io team. This ships with an Xcode project which contains a simple iOS publish/subscribe client, HelloMQTT.~~

* Yet another IOS simple example. https://github.com/tipih/Simple_MQTT
This is working on IOS7 with ARC. It also works with TLS.


*  [mqtt-prowl](https://github.com/jpmens/mqtt-prowl) - Subscribe to topics on an MQTT broker and notify via Prowl

* [MQTT-Client-Framework](https://github.com/ckrey/MQTT-Client-Framework) a native Objective-C (works with Swift too), fully featured MQTT client for iOS, macOS and tvOS. There is a demo application [MQTTChat](https://github.com/ckrey/MQTTChat) and an [Introduction](http://www.hivemq.com/blog/mqtt-client-library-encyclopedia-mqtt-client-framework)
