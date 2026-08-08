1. Your Data is called Segment in this layer. 
2. It create the stream of data.
3. the multiplexing of the data from upper layer and virtuial connectinon and tearing the virtual circuit.
4. [[TCP]] and [[UDP]] protocal work in this layer
##### Connection Oriented:
	sender before transmitting the Segment to the below OSI layerd it contact to the receivers TCP proceess and create the connection this is called the Virtual circuit. and it the connection oriented.

![[Pasted image 20260808175056.png]]

1. The first “connection agreement” segment is a request for synchronization.
2. The next segments acknowledge the request and establish connection parameters—the rules—between hosts. These segments request that the receiver's sequencing is synchronized here as well so that a bidirectional connection is formed.
3. The final segment is also an acknowledgment. It notifies the destination host that the connection agreement has been accepted and that the connection has been established. Data transfer can now begin.

#### Flow Control
1. How much data the sender sendign towards the receiver.
2. Data integrity is also maintained in this layer by usig flow control and ensuring reliable connection between the two parties
3. it prevent the sender to overwhelmed the recevers buffer.
4. what if it overwhelmed the receiver


![[Pasted image 20260808201114.png]]

5. a service is considered connection-oriented if it has the following characteristics:
	(-) A virtual circuit is set up (such as a three-way handshake).
	(-) It uses sequencing.
	(-) It uses acknowledgments.
	(-) It uses flow control.

#### Windowing
Quntity of the data segments sender is allowed to send without receving acknowledgement.
![[Pasted image 20260808210104.png|521]]

#### Acknowledgement
It guarantees that the data is  not duplicated and lost. this achieved through the positive acknowkedgement with the transmission.
1. sender will wait for acknowledgement before sendig any segment to recever end. and start timer if timet is end before getting the ack it will re-transmit the segment again.
![[Pasted image 20260808211009.png]]