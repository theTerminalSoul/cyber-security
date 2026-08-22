In the DoD model, the Internet layer has two main functions: routing data between networks and providing a common interface for upper-layer protocols. IP hides the differences between network technologies, such as wired and wireless Ethernet, so applications do not need separate versions for each technology. Therefore, all communication in the DoD model passes through IP.

1. Internet protocol
	1. 1. What is IP?
		IP (Internet Protocol) operates at the Internet Layer of the DoD/TCP-IP model.
		IP is responsible for logical addressing and routing packets between networks.
		Other protocols at this layer mainly support IP.
		Defined in RFC 791 (IPv4).
	2. IP Address
		Every host/device on a network has a logical/software address called an IP address.
		An IP address helps identify:
		Which network the device belongs to.
		Which device/host is the destination.

		Easy analogy:

		IP address → Street address → identifies the network/location.
		Hardware/MAC address → Mailbox/house identifier → identifies the specific device on that local network.
	3. Routing
		IP examines the destination IP address in every packet.
		Routers use a routing table to determine the best next hop/path.
		Every Layer 3 device (router) makes forwarding decisions using the destination IP address.

	Flow:

		Source → Router → Router → Router → Destination

	At every router:

		Destination IP → Routing Table → Best Next Hop

	4. IP vs Network Access Layer
		Internet Layer (IP)	Network Access Layer
		Sees/interconnects multiple networks	Deals with local networks
		Uses logical IP addresses	Uses hardware/MAC addresses
		Responsible for routing	Responsible for physical/local delivery
		Routers operate here	Switches/NICs operate mainly here
		Works with packets	Works with frames
	5. Packet Handling

		IP receives segments from the Host-to-Host/Transport layer.

		Sending:
			Segment → IP → Packet

		IP can fragment a packet if necessary.
		Each packet contains:
		Source IP address
		Destination IP address

			Receiving:
			Packets → IP → Segment

		IP reassembles fragmented packets at the receiving side before passing the data upward.
	6. Key Terms to Remember
		IP = Internet Protocol
		Layer = Internet Layer
		Address = Logical/software address
		IP address = Identifies network + host
		Router = Layer 3 device
		Routing table = Used to select the next/best path
		Packet = Data unit handled by IP
		Fragmentation = Breaking a packet into smaller pieces
		Reassembly = Putting fragmented packets back together
		RFC 791 = IPv4 specification
		![[Pasted image 20260822173907.png]]
		
		![[Pasted image 20260822174510.png]]



2. ICMP(Internete Cotrol Massage Protocol)
   ICMP is a Network-layer protocol used by IP to report network errors and provide diagnostic information. Its messages are carried inside IP packets.

	Common ICMP functions include:
	  Destination Unreachable: Informs the sender that a packet cannot reach its destination.
      Buffer Full: Reports congestion when a router’s buffer is full.
      Time Exceeded: Reports that a packet’s hop limit has expired.
      Ping: Uses echo requests and replies to test connectivity.
      Traceroute: Uses time-outs to identify the path packets take through a network.
3. ARP(Address Resolution Protocol):
	ARP
		ARP stands for Address Resolution Protocol. It is used to find the MAC address of a device when its IP address is known.
		Maps an IPv4 address to a MAC address.
		Works within a local network.
		The sender broadcasts an ARP request.
		The device with the matching IP address sends an ARP reply containing its MAC address.
		The sender stores this information in its ARP cache for future use.
		ARP requests use the broadcast MAC address FF:FF:FF:FF:FF:FF.
		ARP is commonly used before sending an Ethernet frame to another device on the LAN.
		Example:
			A computer knows a router’s IP address, 192.168.1.1, but not its MAC address. It uses ARP to discover the router’s MAC address.
	RARP
		RARP stands for Reverse Address Resolution Protocol. It allows a device to find its IP address when it knows only its MAC address.
		Maps a MAC address to an IPv4 address.
		A device broadcasts a RARP request.
		A RARP server checks its table and replies with the device’s IP address.
		It was mainly used by diskless workstations and devices with limited storage.
		RARP does not use IP because the device does not yet know its IP address.
		It has largely been replaced by BOOTP and DHCP.
		
![[Pasted image 20260822175929.png]]

   
   
   4. GRE(Generic ROuting Protocol)
      GRE stands for Generic Routing Encapsulation. It is a tunneling protocol used to carry one network-layer packet inside another packet across an IP network.

		How GRE Works
			A router receives the original packet, called the passenger packet.
			GRE adds a GRE header to the packet.
			An outer IP header is added with the addresses of the GRE tunnel endpoints.
			The packet travels through the network using the outer IP header.
			The receiving router removes the outer IP and GRE headers.
			The original packet is then routed to its destination.
		GRE Components
			Passenger protocol: The original packet being transported.
			Carrier protocol: GRE, which encapsulates the original packet.
			Transport or delivery protocol: IP, which carries the GRE packet across the network.
		Advantages
			Connects separate private networks through an IP network.
			Supports IPv4, IPv6, multicast, and some routing protocols.
			Can create a virtual point-to-point connection between routers.
			Helps carry packets that may not normally be supported by the underlying network
		Limitations
			GRE does not provide encryption or strong authentication.
			GRE adds extra headers and increases packet size.
			It may require MTU adjustments to prevent fragmentation.
			GRE is often combined with IPsec when security is needed.
	Important Fact
		The outer IP header is used to forward the packet through the GRE tunnel. After the packet reaches the destination router, the outer headers are removed and the original packet is forwarded using its inner IP header. GRE uses IP protocol number 47.
	Easy example:
		GRE is like placing one envelope inside another. The inner envelope contains the original packet, while the outer envelope carries it across the network to the GRE tunnel endpoint.