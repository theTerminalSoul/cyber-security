It is the special characteristic of the Network it shows the hwo the devices, cables and server are connected with each other

#### Different Type of topology
1. Bus
	1. This the kind the network where the devices the connected with using the cable(BUS). 
	2. each device can communicate with ecach other through this BUS. it has the terminator at both end.
	3. It is very simple and less expensive also it required the less cable than other topologies.
	4. the drawback is. if the cable fails it can lead all netwoek to down and it is hard to troubleshoot and also lack fauld tolerance.
	   ![[Pasted image 20260804214004.png|513]]

2.  Star(Hub and spoke) 
	1. this the widly use topology it connets all the devices, printers, host to the central Hub.
	2. it also called Hub and Spoke where the central device is called HUB and all the connected Devices are SPOKE.
	3. it required more cable than the bus topology but this can provide the better fault tolerense as if one link or cable fails it affect only that device only other will still working.
	4. the disadvantage of this is ther is single point of failure, if central HUB down all the netweok goes down.
	5. ![[Pasted image 20260805202041.png|491]]

3. Ring
	1. this is similar like bus topology as it will connect all the diveces with the single bus creating the ring like structure.
	2. if ring get damage the whole network goes down.
	3. ring topology is not use in LAN network but you can find this in the WAN network. e.g SONET(it id fault tolerant fiber optic network use the rign topology)
	![[Pasted image 20260805202636.png|376]]

4. Mesh
	1. In this topology every node is connected with each ohter creating the mesh like structure.
	2. providing the highest level of redunduncy. but it will required the lots of cables to connect device with each other 
	3. you can use the n*(n-1)/2 formula to find the number of cable required to create the full mesh.
	4. Half Mesh
		1. in this you dont connet the all deviece with each other rather you only connect the critical devices with each other making it consume less resources.
	![[Pasted image 20260805203204.png]]

Honorable Mention 
1. Point to Point
2. Point to Multipoint
3. Hybrid 
	1. ir is the Combination of 2 or more physical and logical topology.
	![[Pasted image 20260805203619.png]]



#### [[Network Models]]