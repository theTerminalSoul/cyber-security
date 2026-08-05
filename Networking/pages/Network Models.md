#### 1. Three Tiered Model
![[Pasted image 20260805210834.png|885]]

1. This the create by te cisco 20 year ago and it still use in the current world
2. Level Of Model:
	1. Core:
		1. it is the backbone of your network where your strongest routers live.
		2. this level connects your geographical areas with WAN line.
		3. it is design for the high avaiblity and only for the routing and switching.
	2. Distribution:
		1. This layear is also known as aggregation layer cause this allows the connectivity between the multiple access layer switches.
		2. in this layer control plane is located and packet filtering, securiyt polies and routing between vLAN and defining broadcast domain is performed.
		3. you can think as distribution of switching form core level access lavel
	3. Access layer:
		1. he access layer is often referred to as the edge switching layer, and it connects the end-user hosts. 
		2. it provided the local switching and creation collision domain.
		3.
3. Collaped core model : 
	1. it is the model same as Three tired model just we merge the core and distribution layer.
	2. as the power of the switches are increase it can work for the both core and distribution layer on same piece of the network switching devices.
	3. the sole pupose of thid model is use the power of current switches to save the cost.

#### 2. Spine and Leaf (CLOS)
![[Pasted image 20260805213208.png]]

1. spine and leaf is mostly use in the Datacenter for its High speed and redundunt network.
2. the most powerfull switch work and th spine and the connected switches work as LEAF.
3. Every spine switch is connected to the all leaf switches providing the high speed datatransfer and 2 hop between the travel.
    Important rules:
    1. No same lavel connection: no spine to spine and no leaf to leaf
    2. Linear Scale-Out (Horizontal Scalability)

#### [[Traffic Flow]]
