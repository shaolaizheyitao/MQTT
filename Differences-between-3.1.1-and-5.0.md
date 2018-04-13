Differences between versions 3.1.1 and 5.0 of the MQTT specification:

3.1.1 specification: hhttp://docs.oasis-open.org/mqtt/mqtt/v3.1.1/mqtt-v3.1.1.html

5.0 specification: http://docs.oasis-open.org/mqtt/mqtt/v5.0/mqtt-v5.0.html (pages 135/ 136)

1. Session expiry:
Split the Clean Session flag into a Clean Start flag which indicates that the session should start without using an existing session, and a Session Expiry interval which says how long to retain the session after a disconnect. The session expiry interval can be modified at disconnect. Setting of Clean Start to 1 and Session Expiry Interval to 0 is equivalent in MQTT v3.1.1 of setting Clean Session to 1.

2. Message expiry:
Allow an expiry interval to be set when a message is published.

3. Reason code on all ACKs:
Change all response packets to contain a reason code. This include CONNACK, PUBACK, PUBREC, PUBREL, PUBCOMP, SUBACK, UNSUBACK, DISCONNECT, and AUTH. This allows the invoker to determine whether the requested function succeeded.

4. Reason string on all ACKs:
Change most packets with a reason code to also allow an optional reason string. This is designed for problem determination and is not intended to be parsed by the receiver.

5. Server disconnect:
Allow DISCONNECT to be sent by the Server to indicate the reason the connection is closed. 

6. Payload format and content type:
Allow the payload format (binary, text) and a MIME style content type to be specified when a message is published. These are forwarded on to the receiver of the message.

7. Request / Response:
Formalize the request/response pattern within MQTT and provide the Response Topic and Correlation Data properties to allow response messages to be routed back to the publisher of a request. Also, add the ability for the Client to get configuration information from the Server about how to construct the response topics.

8. Shared Subscriptions:
Add shared subscription support allowing for load balanced consumers of a subscription

9. Subscription ID:
Allow a numeric subscription identifier to be specified on a SUBSCRIBE, and returned on the message when it is delivered. This allows the Client to determine which subscription or subscriptions caused the message to be delivered.

10. Topic Alias:
Decrease the size of the MQTT packet overhead by allowing the topic name to be abbreviated to a small integer. The Client and Server independently specify how many topic aliases they allow.

11. Flow control:
Allow the Client and Server to independently specify the number of outstanding reliable messages (QoS>0) they allow. The sender pauses sending such messages to stay below this quota. This is used to limit the rate of reliable messages, and to limit how many are in flight at one time.

12. User properties:
Add User Properties to most packets. User properties on PUBLISH are included with the message and are defined by the Client applications. The user properties on PUBLISH and Will Properties are forwarded by the Server to the receiver of the message. User properties on the CONNECT, SUBSCRIBE, and UNSUBSCRIBE packets are defined by the Server implementation. The user properties on CONNACK PUBACK, PUBREC, PUBREL, PUBCOMP, SUBACK, UNSUBACK and AUTH packets are defined by the sender, and are unique to the sender implementation. The meaning of user properties is not defined by MQTT.

13. Maximum Packet Size:
Allow the Client and Server to independently specify the maximum packet size they support. It is an error for the session partner to send a larger packet.

14. Optional Server feature availability:
Define a set of features which the Server does not allow and provide a mechanism for the Server to specify this to the Client. The features which can be specified in this way are: Maximum QoS, Retain Available, Wildcard Subscription Available, Subscription Identifier Available, and Shared Subscription Available. It is an error for the Client to use features that the Server has declared are not available. 

It is possible in earlier versions of MQTT for a Server to not implement a feature by declaring that the Client is not authorized for that function. This feature allows such optional behavior to be declared and adds specific Reason Codes when the Client uses one of these features anyway.

15. Enhanced authentication:
Provide a mechanism to enable challenge/response style authentication including mutual authentication. This allows SASL style authentication to be used if supported by both Client and Server, and includes the ability for a Client to re-authenticate within a connection.

16. Subscription options:
Provide subscription options primarily defined to allow for message bridge applications. These include an option to not send messages originating on this Client (noLocal), and options for handling retained messages on subscribe.

17. Will delay:
Add the ability to specify a delay between the end of the connection and sending the will message. This is designed so that if a connection to the session is re-established then the will message is not sent. This allows for brief interruptions of the connection without notification to others.

18. Server Keep Alive:
Allow the Server to specify the value it wishes the Client to use as a keep alive. This allows the Server to set a maximum allowed keepalive and still have the Client honor it.

19. Assigned ClientID:
In cases where the ClientID is assigned by the Server, return the assigned ClientID. This also lifts the restriction that Server assigned ClientIDs can only be used with Clean Session=1 connections.

20. Server reference:
Allow the Server to specify an alternate Server to use on CONNACK or DISCONNECT. This can be used as a redirect or to do provisioning.
