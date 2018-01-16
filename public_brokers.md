This page is an effort to list the publically-accessible MQTT brokers, often useful for testing and prototyping.

Note: none of these test brokers carry any guarantee of service. Be sensible when using them and don't break things for others! :-)

field | value
------|------
_address_ | `mqtt.flespi.io`
_port_ | `1883` (TCP), `80` (WebSocket), `8883` (SSL), `443` (Secure WebSockets)
_type_ | flespi
_info_ | requires signup/username, [information page](https://flespi.com/mqtt-api), free to use up to [100 persistent sessions](https://flespi.com/pricing#restrictions), [REST API](https://flespi.io/mqtt)

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
_address_ | `dev.rabbitmq.com` 
_port_ | `1883` 
_type_ | rabbitmq 
_info_ | [admin dashboard](http://dev.rabbitmq.com)

***

field | value
------|------
_address_ | `broker.mqttdashboard.com` 
_port_ | `1883`, `8000` (WebSockets) 
_type_ | HiveMQ 
_info_ | [information page](http://www.mqtt-dashboard.com/info/broker), [stastistics and dashboard](http://www.mqtt-dashboard.com/dashboard)

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
_address_ | `mqtt.simpleml.com` 
_port_ | `1883` (MQTT), `8883` (MQTT+SSL), `80` (REST), `80` (WebSockets), `5683` (CoAP)
_type_ | SimpleML
_info_ | Free MQTT service to evaluate Machine Learning models, [documentation](http://simpleml.com) 

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
_address_ | `mqttserver.com`
_port_ | `1883` (TCP), `8000` (WebSocket), `8883` (SSL), `8443` (Secure WebSockets)
_type_ | `Bevywise`
_info_ | [web page](http://bevywise.com/iot-platform). Secure. Need to sign up to view your devices. Use MQTT Authentication in your devices to connect securely.
***

field | value
------|------
_address_ | `m.thingscale.io`
_port_ | `1883` (TCP), `8083` (WebSocket), `8883` (SSL), `8084` (Secure WebSockets)
_type_ | 'thingscale.io'
_info_ | requires signup/username and password, [signup](https://m.thingscale.io/signup/index_en.php) (30days trial plan available), [Dev Portal](https://sensinics.atlassian.net/wiki/spaces/TD/pages/76021778/Developer+Portal), [API Portal](https://thingscale.docs.apiary.io)

***
