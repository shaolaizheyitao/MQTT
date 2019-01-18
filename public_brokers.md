This page is an effort to list the publically-accessible MQTT brokers, often useful for testing and prototyping.

Note: none of these test brokers (except mqtt.flespi.io and myqtthub.com) carry any guarantee of service. Be sensible when using them and don't break things for others! :-)

field | value
------|------
_address_ | `mqtt.flespi.io`
_port_ | `1883` (TCP), `80` (WebSocket), `8883` (SSL), `443` (Secure WebSockets)
_type_ | flespi
_info_ | requires signup/username, [information page](https://flespi.com/mqtt-broker), [REST API](https://flespi.io/mqtt), MQTT 5.0 [compliant](https://flespi.com/mqtt-broker#mqtt-checklist)

***

field | value
------|------
_address_ | `iot.eclipse.org`
_port_ | `1883`, `80` (WebSockets), `443`(WebSockets+SSL)
_type_ | mosquitto
_info_ | [web page](http://iot.eclipse.org/sandbox.html), [Xively statistics](https://xively.com/feeds/59871), [topics and HTTP bridge](http://eclipse.mqttbridge.com)

***

field | value
------|------
_address_ | `test.mosquitto.org`
_port_ | `1883`, `8883` (SSL), `8884` (SSL), `80` (WebSockets)
_type_ | mosquitto
_info_ | [web page](http://test.mosquitto.org), [Xively statistics](https://xively.com/feeds/43810), [topics and HTTP bridge](http://test-mosquitto.heroku.com)


***

field | value
------|------
_address_ | `broker.hivemq.com` 
_port_ | `1883`, `8000` (WebSockets) 
_type_ | HiveMQ 
_info_ | [information page](https://www.hivemq.com/try-out/), [stastistics and dashboard](http://www.mqtt-dashboard.com/dashboard)

***

field | value
------|------
_address_ | `www.cloudmqtt.com` (Note: actual host varies, see dashboard)
_port_ | `18443`, `28443` (SSL)
_type_ | mosquitto
_info_ | requires signup/username and password, [pricing](http://www.cloudmqtt.com/plans.html) (free plan available), [documentation](http://www.cloudmqtt.com/docs.html)

***

field | value
------|------
_address_ | `mqtt.dioty.co` 
_port_ | `1883` (MQTT), `8883` (MQTT+SSL), `8080` (WebSockets), `8880` (WebSockets+SSL)
_type_ | `mosca`
_info_ | Free - requires signup/username and password, [documentation](http://www.dioty.co), includes [mobile IoT app](http://www.dioty.co/mobile) (iOS and Android)

***

field | value
------|------
_address_ | `mqtt.swifitch.cz` 
_port_ | `1883` (MQTT)
_type_ | `mosquitto`
_info_ | Free, it is mostly running for [Swifitch project](http://www.swifitch.cz), but you can use it too for testing your IoT or whatever ;), it is running on ~~Raspberry Pi~~ profesional VPS.

***

field | value
------|------
_address_ | `broker.bevywise.com`
_port_ | `1883` (TCP), `8443` (WebSockets)
_type_ | `Bevywise`
_info_ | [web page](http://bevywise.com/iot-platform). Secure. Need to sign up to view your devices. Use MQTT Authentication in your devices to connect securely. Free trial with unsecure ports (see https://devicemanager.bevywise.com/help)

***

field | value
------|------
_address_ | `mqtt.fluux.io`
_port_ | `1883` (TCP), `8883` (TLS)
_type_ | ejabberd
_info_ | Free - no registration required, MQTT 5.0 compliant

***

field | value
------|------
_address_ | [`console.solace.cloud`](https://console.solace.cloud) (MQTT hostname varies, see dashboard)
_port_ | TCP, TLS, WS, WSS: varies per instance
_type_ | solace
_info_ | requires sign-up, free plan available (50 connections), [getting started](https://cloud.solace.com/learn/), [docs](https://docs.solace.com/)

***

field | value
------|------
_address_ | [`node02.myqtthub.com`](https://node02.myqtthub.com)
_port_ | `1883` (TCP), `8883` (SSL), `443` (Web, REST and API interface)
_type_ | MyQtthub
_info_ | requires signup/username, [information page](https://myqtthub.com), [REST API](https://www.asplhosting.com/portal/en/rest-api-to-manage-mqtt-service)