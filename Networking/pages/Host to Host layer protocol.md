1. TCP(Transmisison Control Protocol):
   TCP is a reliable, connection-oriented protocol that breaks application data into numbered segments, sends them, and retransmits any lost segments. It establishes a connection using a three-way handshake and terminates it when communication ends. TCP ensures accurate, ordered, full-duplex data delivery but creates more network overhead than UDP. Therefore, TCP is commonly used for reliable communication, while UDP is preferred for real-time applications such as video streaming and VoIP.

##### TCP Segment Format
TCP divides the application data stream into segments and sends them to the Internet layer, which routes them as packets. At the destination, TCP reassembles the segments into the original data stream for the upper-layer applications. The TCP header is 24 bytes long and can be up to 60 bytes when options are included.
![[Pasted image 20260822164725.png]]


![[Pasted image 20260822165636.png]]



### UDP(User Datagram Protocol)
UDP is a lightweight, connectionless transport protocol that uses less bandwidth and has lower overhead than TCP. It does not establish a connection, sequence data, provide acknowledgments, or retransmit lost segments, making it unreliable but faster. UDP is useful for applications such as SNMP, DNS, streaming, and VoIP, especially when the application handles reliability itself. Developers choose TCP for reliable delivery and UDP for speed and efficiency.

![[Pasted image 20260822170322.png]]