# MQTT protocol

## Specification
The current formal MQTT protocol specification can be found at:

*  [MQTT v3.1.1 specification](http://docs.oasis-open.org/mqtt/mqtt/v3.1.1/mqtt-v3.1.1.html)

The current MQTT-SN specification from IBM can be found at:

* [MQTT-SN v1.2 specification](http://mqtt.org/new/wp-content/uploads/2009/06/MQTT-SN_spec_v1.2.pdf)

## Clarifications

As questions arise around particular aspects of the specification, we are collecting clarifications:

*  [Topic Format](../topic_format)

*  [Security considerations](http://www.hivemq.com/mqtt-security-fundamentals/)

*  [Are topics dynamic](../are_topics_dynamic)?

*  [Overlapping topics](../overlapping_topics)

*  [KeepAlive for the client](../keepalive_for_the_client)

*  [Miscellaneous clarifications](../miscellaneous_clarifications)

*  [MQTT over Websockets](../mqtt_over_websockets)

*  [Duplicates on QOS 0](../duplicates_on_qos_0)

*  [Clarify UTF8 strings](../clarify_utf8_strings)

*  [Will Message UTF8 Support](../will_message_utf8_support)

*  [ClientID autogeneration](../clientid_autogeneration)

## Ideas for future enhancement

Ideas (and reasons for why they may be required) are being collected here:


*  [ClientID autogeneration](../clientid_autogeneration)

*  [Topic string enhancement](../topic_string_enhancement)

*  [Broker auto-discovery](../broker_auto-discovery)

*  [URL scheme](../URI-Scheme)

*  [Status field for acks](../status_field_for_acks)

*  [Add messageid to ping](../add_messageid_to_ping)

*  [Will Message UTF8 Support](https://github.com/mqtt/mqtt.github.io/wiki/will_message_utf8_support)

*  [Bridge protocol](../bridge_protocol)

*  [Extended CONNACK codes](../extended_connack_codes)

*  [Registered topics like MQTT-SN](https://github.com/mqtt/mqtt.github.io/wiki/registered_topics_like_mqtt_sn)

*  [MQTT for Centralised Data Collection](http://mqtt.org/wiki/lib/exe/fetch.php/cloud.pdf)

*  [Time To Live for retained message](../time_to_live_for_retained_message)
## Items fixed in the updated OASIS spec

*  [Extended ClientID](../extended_clientid)

*  [Short usernames and passwords](../short_usernames_and_passwords)

