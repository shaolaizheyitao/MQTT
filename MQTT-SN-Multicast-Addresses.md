This is a proposal, the addresses have not be peer-reviewed or registered with IANA.


| Scope Name         | MQTT-SN Radius | IPv6 Address         | IPv4 Address                |
|--------------------|----------------|----------------------|-----------------------------|
| Node-Local         | 0              | FF00:0:0:0:0:0:0:75B | 239.255.255.72 (with TTL=0) |
| Link-Local         | 1              | FF01:0:0:0:0:0:0:75B | 239.255.255.72 (with TTL=1) |
| Realm-Local        | 3              | FF03:0:0:0:0:0:0:75B |                             |
| Admin-Local        | 4              | FF04:0:0:0:0:0:0:75B |                             |
| Site-Local         | 5              | FF05:0:0:0:0:0:0:75B |                             |
| Organization-Local | 8              | FF08:0:0:0:0:0:0:75B | 239.195.255.72              |
| Global             | 14             | FF0E:0:0:0:0:0:0:75B |                             |

Notes:
* Addresses use scope relative addressing
* For IPv6: 0x75B = 1883 in decimal
* For IPv4: 72 = 255 - 183


## Scope Descriptions

The scope descriptions are taken from [RFC4291](http://tools.ietf.org/html/rfc4291).

* **Node-Local**: spans only a single interface on a node and is useful only for loopback transmission of multicast.
* **Link-Local**: spans the same topological region as the corresponding unicast scope.
* **Admin-Local**: is the smallest scope that must be administratively configured, i.e., not automatically derived from physical connectivity or other, non-multicast-related configuration.
* **Site-Local**: is intended to span a single site.
* **Organisation-Local**: is intended to span multiple sites belonging to a single organisation.
* **Global**: the whole of the internet
