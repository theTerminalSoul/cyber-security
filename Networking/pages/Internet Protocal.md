TCP/IP is the model created by the US gov DARPA.
1. The first ever internet mode is DoD model with
	1. Application/Process
	2. Host-to-Host
	3. Internet
	4. Network Access

 ![[Pasted image 20260820203346.png]]
 
 #### Important Protocol
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
<mark style="background: #FFB86CA6;"></mark>


















