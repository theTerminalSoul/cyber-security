1. Data in this layer called Packets.
2. it managed the logical addressing
3. track location of device 
4. Determine best way to send the data to destination
5. Rounter are the devices that use in this layer that provides the routing services.
#### How it works
1. Data packet received to the router.
2. router then check the destination if packet destined to that router then it send data to it if not then it look up in the routing table.
3. if not found there it will drop that packet.
4. Two packets are use in network layer
	1. Data Packets: they are use to transport the user data in internetwork.
		the protocol used here are called routed protocol. eg IPv4 and IPv6
	2. Route-Update Packet : 
		1. Network Sharing: Route-update packets are messages sent via routing protocols (like OSPF or EIGRP) to share path information between neighboring routers.
		2. Map Maintenance: Routers use these updates to dynamically build and continuously maintain their routing tables so data takes the best available path.
	![[Pasted image 20260808233219.png]]

#### Network addressing 
1. It is protocol specific network addressing
2. each router should keep track for each protocol as differernt protocol can use different Network addressing scheme like IP or IPv6
#### Interface
1. this is the exit interface packet will take when destined for specific network
#### Metric
1. distance to the remote network
2. each protocol use different metric to define this eg. RIP uses the Hop Count.

#### Some key point of router
1. Blocks Broadcasts: Routers automatically stop broadcast and multicast traffic from passing through to other networks by default.
2. Uses Logical Addresses: They look at Layer 3 (Network layer) IP addresses to figure out the next hop for a packet.
3. Controls Security: Administrators can set up Access Control Lists (ACLs) to filter and block specific traffic entering or leaving an interface.
4. Supports Layer 2 & 3: They can route Layer 3 traffic and bridge Layer 2 traffic simultaneously on the same interface.
5. Connects VLANs: They act as Layer 3 gateways to allow different Virtual LANs (VLANs) to talk to each other.
6. Manages Traffic (QoS): They can prioritize critical network traffic over less urgent data using Quality of Service settings.









