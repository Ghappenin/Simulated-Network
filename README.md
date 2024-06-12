<h1>Simulated Network With Cisco Packet Trackers </h1>

<h2>Description</h2>
By the end of this project, you will create a small simulated network from scratch using Cisco Packet Tracer. You will be able to identify the basic fundamentals of computer networking and the very basic architecture behind the network devices (Routers and Switches). Moreover, you will learn and practice how to get all these devices and components connected together.  Finally, you will be able to troubleshoot the issues and write some basic commands to get the network fully functioning :



<br />


<h2>Operating System Used<h2>

- <b>WIndows 11 Home 13th Gen Intel(R) Core(TM) i7-1360P 2.20 GHz</b>

<h2>Downloads<h2>
 
- <b>[Wireshark 4.2.5](https://www.wireshark.org/)</b>

<h2>Project walk-through:</h2>

<p align="center">
Download Wireshark: <br/>
<img src="https://i.imgur.com/FVWrYiX.png" height="80%" width="80%" />
<br />
<br />
Select source of capture: Wireless, Ethernet etc: <br/>
<img src="https://i.imgur.com/00SfRUR.png" height="80%" width="80%" />
<br />
<br />
Upper left click -green- "sharkfin" to begin your capture: <br/>
<img src="https://i.imgur.com/lbyR5hY.png" height="80%" width="80%" />
<br />
<br />
Stop your capture with -red- box and save to your file of choosing:  <br/>
<img src="https://i.imgur.com/UN55BQU.png" height="80%" width="80%" />
<br />
<br />
Use a display filter to detect HTTPS packets:  <br/>
 ●To display certain packets in an existing packet capture, use a display filter <br/>
 ●To display only HTTPS traffic, use a filter on TCP port 443: tcp.port == 443 <br/>
<img src="https://i.imgur.com/W2nbWQN.png" height=80%" width="80%" />
<br />
<br />
Use a display filter to detect DNS (Domain Name System)if websites and subsites visited:  <br/>
<img src="https://i.imgur.com/2xEq9cr.png" height="80%" width="80%" />
<br />
 - <b>https://wiki.wireshark.org/DisplayFilters
<br />
<br />
Visit a web page and detect its IP address using a display filter. A TLS handshake display filter: tls.handshake.type ==1 <br/>
<img src="https://i.imgur.com/LoPi1bu.png" height="80%" width="80%" />
<br />
<br />
●A Conditional statement may be used to include and eliminate packets from a Wireshark capture: !(ip.addr == 8.43.85.97) and tcp.port == 443

●A compound conditional should include parentheses to avoid order of execution errors: !(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)
