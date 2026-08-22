 1. FTP(Port 21, 22):
	 1. It use to share the file over the network. Its not the protcol but the Program operating as protocol.
	 2. Even when employed by users manually as a program, FTP's functions are limited to listing and manipulating directories, typing file contents, and copying files between hosts. But it not secure as the all data is share as plain text.
	 3. so you can use SFTP.
2. SSH(Secure shell)(Port 22):
	1. it use setup the secure Telnet session over the network
	2. by this you can log into other system and run program remotely. it also maintain the nice strong encrypted connection.
3. SFTP(Secure File Transfer Protocol) (Port 22):
	1. it is the secure way of transfering file over internet. it uses the SSH tunnel to transfer the file so the file will be securely transmitted.
4. Telnet(port 23):
	1. It is the terminal emulator that we can use to run text based command on the server
	2. it share data fast on making server thing you are sitting beside it and typing the command it use the TCP.
	3. Its not secure thats why it replace by the SSH.
5. Simple Mail Trandfer protocol(Port 25):
	1. This protocol is used to transper the mail using the spooled or queued method 
	2. when massage is sent to the destination its spooled to the device-disk- and the software at the destination posts a vigil and if the massage arrived it detect them and develiverd to the destinaton
	3. POP3(port 110(unsecured) and 995(secure)) is used to received the mail
6. DNS(Domain Name Syatem)(Port TCP and UDP 53):
	1. It is use to resolve it domain name 
7. DHCP(Dynamic Host Confiuration Protocol)(UDP Port 67/68):
	1. DHCP also called as Boostrap Protocol
	2. It assign the IP address to the host
8. TFTP(Trivial File Transfer Protocol)(UDP 69)
	1. It is te striped version of FTP
	2. it does not do te file opration like FTP. It use when you know what exactly what you want and where you can can find.
	3. It require no password so it not secure thats whay very few website use this
9. HTTP(Hypertext Transfer Protocol)(TCP Port 80):
	1. When you click on any link or browse on web you get the result or page that the HTTP(HTTPS(Port 443) in todays world) doing.
10. POP3(Post Office Protocol3)(UDP Port 110)
	1. when client connects to this server the massage addressing to the client started downloading. it doesnt allow download selectively rather when the client server connection end you can download and twick as per your will. 
	2. IMAP id more use than POP3 as it is more secure and flexible.
	   <mark style="background: #FFF3A3A6;">IMAP uses two main ports: Port 993 for secure, encrypted connections (SSL/TLS) and Port 143 for unencrypted, standard connections</mark>
11. NTP(Network Time Protocol)(UDP 123):
	1. This protocol is used to syn the machin time conneted the the network with the server
	2. that server usest he atomic clock to manage the time so it is imprtant so every machine on the netwoek can have the same time. it can use for log tracking and the tiem sensitve work.
12. IMAP(Interner Massage Access Protocol)(port 143 not secure/993 secure)
	1. this protocol help us to download the email without deleting the copy fromt the server so we cna see our emails from mobile, laptop and other devices.
13. SNMP(Simple Network Management Protocol)(Port UDP 161/162):
	1. this protocol use to pull the differnet network information from the Network station.
	2. when everything is good it will send the baseline-- which is report terminator
	3. it also work as watchdog for your network clled agents. if any thing happens ageint triggers the alert called trap.
		1. ther is NMS(netwoek management system) polls the MIB(management information base:" directory of set of rule that NMS ask to the agents")
14. LDAP(Lighteight Directory Access Protocol)(Port TCP 389):
	1. This protocol is used to access and query the directory service system like microsft AD
	2. It also have secure version called LDAPS(Port 363)
15. HTTPS(Hypertext Transfer Protocol Secure)(port 443)
	1. this is the secure way of web talking to the server
	2. web uses the both SSH and HTTPS to make browser safe.
16. Transport Layer Security/Secure Socket Layer(port 995/465)
	1. It is the cryptographic protocol that is handy for enabling secure file transfer over web and server.
17. SMB(Server Message Block)(TCP 445):
	 1. Server Message Block (SMB) is used for sharing access to files and printers and other communications between hosts on a Microsoft Windows network. SMB runs mostly on TCP port 445 now, but SMB can also run on UDP port 137 and 138 and on TCP port 137 and 139 using NetBIOS.
18. SysLog(UDP 514):
19. SMTPS (TCP 587)
20. Lightweight Directory Access Protocol over SSL (TCP 636)
21. IMAP over SSL (TCP 993)
22. POP3 over SSL (TCP 995)
23. Structured Query Language (SQL) Server (TCP 1433)
24. SQLnet (TCP 1521)
25. MySQL (TCP 3306)
26. Remote Desktop Protocol (TCP 3389)
27. SIP (VoIP) (TCP or UDP 5060/TCP 5061)
28. RTP (VoIP) (UDP 5004/TCP 5005)
29. MGCP (Multimedia) (TCP 2427/2727)
30. H.323 (Video) (TCP 1720)

#### IGMP(Interner Group Management Protocol)
	Internet Group Management Protocol (IGMP) is an IPv4 network layer protocol used by devices and local routers to establish and manage multicast group memberships. It lets a device tell a router that it wants to receive a specific data stream, saving network bandwidth.\

31. NetBIOS (TCP and UDP 137–139)