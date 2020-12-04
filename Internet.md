# Internet and its Applications

## The Networking and Internet Basics

### Types of network

**Local Area Network (LAN)**
a network of computers and other devices over a geographical area smaller than WAN - a single or a group of buildings 

types of LAN:  
- Wired LAN
- Wireless LAN (WLAN)

**Wide Area Network (WAN)**
composed of LANs connected through routers over a larger geographical area - a country or the world (The Internet)

### Types of Connections
- peer-to-peer network - computers are connected to nearby computers
	- examples
		- BitTorrent
		- P2PTV
		- PDTP
	- advantages
		- resources can be accessed by other users
		- encouraging community resource sharing and cooperation
	- disadvantages
		- Intellectual property law and illegal sharing
		- Network neutrality - extra bandwith-usage
- client-server connection - all computers are connected to a server
	- examples
		- dedicated server games
		- majority of the websites on the Internet
	- advantages
		- users can be given different levels of access to the data in the server
	- disadvantages
		- require connection to the dedicated server

</empty> | Peer-to-Peer | Client-Server
--- | --- | ---
machines | server - machine(s) to provide services for clients, clients - machines requesting services from server(s) | no server, all machines request and share resources between others (peers)
installation | servers are hard to configure | easier
administration | centralized | decentralized, hard to manage
security | secure | less secure due to decentralized resources
failure | when server fails | do not
suitable in | large no. of machines | small no. of machines  
OSes | OS for networking features (for peer-to-peer) | server: network OS, control resources; client: OS allowed to be identified and communicate with server
<br>

### Hardware

**Network Interface Card (NIC)**  
	provide interface for communication over network
	has unique Media Access Control (MAC) address for identification

**Connection Devices**
- Hubs
	- can act as a repeater
	- multiple ports - connects computers
	- message received from one port is forwarded to all ports
	- cannot simultaneously transmit messages (collision will occur)
- Switches
	- multiple ports - connects computers
	- message received from one port is forward to destination port
	- can simultaneously transmit messages (less collision)
	- perform the forwarding according to MAC address of NIC of the destination
	- switch-based generally faster than hub-based network
- Repeater
	- amplify signals
	- remove noise
- Bridges
	- connect LANs of same type
- Routers
	- connect LANs of different type to form WAN
	- connect LANs and Internet
	- perform routing, i.e. find best path for packets to destination, and store routing table
	- perform forwarding according to IP address of the destination
- Access point
	- multiple devices connected to form a wireless network
	- may act as a router

**Modem**
- perform modulation - convert digital signals into analogue signals
- perform demodulation - convert analogue signals into digital signals
- examples
	- dial-up modem
	- cabble modem (cable TV)
	- Asymmetric Digital Subscriber Line (ADSL) modem

**Wires**
- telephone lines
- coaxial cables
	- electric signals
- twisted-pair wires
	- electric signals
	- twisted to reduce EM interference
	- 2 types
		- shielded twisted pair (STP) cables
		- unshielded twisted pair (UTP) cables
	- commonly used in LANs
- optical fibres
	- light signals
	- faster
	- difficult to eavesdrop
	- more expensive
	- require signal conversion device

</empty> | twisted pair cables | coaxial cables | optical fibres
--- | --- | --- | ---
price | low | medium | high
transmission rate | low | medium | very high
interference | relatively high | medium | low

**Radio Connections**
- satellite broadband
	- through satellite by microwave
	- connects to internet wirelessly
- microwave broadband
	- between microwave stations
	- coverage: ~1.5 km
	- can be obstructed (straight line)
- wireless fidelity (Wi-Fi)
	- sender convert digital signal to radio signal
	- receiver convert radio signal to digital signal
	- require wireless NIC

## Multiplexing (extra)
method to **combine multiple signals** into one signal **over shared medium**  
e.g. multiple telephone calls carried out using one wire  

Types:
- Space-division multiplexing (**SDM**)
	- use of **separate point-to-point electrical conductors** for each channel
	- faster than TDM
	- require physical connection per communication pair
- Frequency-division multiplexing (**FDM**)
	- use of several distinct **frequencies** for each channel
	- used in analogue system
	- channel allocated any time
- Time-division multiplexing (**TDM**)
	- use at different **time** for each channel
	- require precise clock synchronization
- Code-division multiplexing (**CDM**)
	- use of same frequency, distinguish by **unique codes**
	- secure
	- complex scheme
- Wavelength-division multiplexing (**WDM**)
	- use of different **wavelength** of laser light for each channel
	- distinguish by refraction
	- require optic fiber
- Other types
	- Polarization-division multiplexing
	- Orbital angular momentum multiplexing

### Internet Access
**Internet Service Providers (ISP)** provide access to the Internet  

ways to connect:  
- dial-up access
- Integrated Services Digital Network (ISDN) terminal adaptors
- leased line
- broadband connection
	- asymmetric digital subscriber line (ADSL)
	- symmetric digital subscriber line (SDSL)
	- cable modem 
- wireless Internet access
	- Wi-Fi hot spots
	- wireless application protocol (WAP)
	- general packet radio services (GPRS)
	- high speed packet access (HSPA)

</empty> | dial-up | ISDN | leased line | broadband | wireless
--- | --- | --- | --- | --- | ---
transmission speed | low (max 56 kbps) | low (basic max 128 kbps) | medium (depends on type: ~1 Mbps - ~50 Mbps) | medium (depends on DSL or modem) | medium to fast  
cost | usually low | medium | high | medium | low to high
physical security | low | medium | high | low | N/A

## Communication Software and Protocols
**communication software** is a software that provide fast and effective way for intert access or activity

typical softwares:  
- web browser
	- for surfing the Internet
	- extensions or features to enhance browsing experiences
- email programs
	- to send and receive emails
- newsgroup program
	- receive news
- instant messaging programs (IM)
	- for message communication with other devices with the same software
- file transfer program
	- to send files to other devices
- telnet program
	- to remotely control another deveice or server through CLI
- social networking software
	- to share text/image/video on the Internt
	- for browsing text/image/video shared by others on the Internet
- video conferencing software
	- to communicate through live video with others with the same software
<br>

**protocols** are a set of rules guiding communcation between computer systems through standardization

open system interconnection (OSI) model (from top to bottom):
- application layer
	- examples of protocols: FTP, HTTP
- presentation layer
- session layer
- transport layer
	- examples of protocols: TCP, UDP
- network layer
	- example of protocol: IP
- data link layer
- physical layer

**Transmission Control Protocol (TCP)**  
responsible for:
- division of messages into packets
- transmission
- verificaiton
- reassembling of packets

**Internet Protocol (IP)**  
responsible for:  
- divide packets into fragments (smaller pieces) according to the transmission rate
- routing the packets to destination

**IP Addess**
- all devices using IP will have an IP address
- IP identify destinations according to IP address
- IP address have 2 parts
	- network part - identify the network on the Internet
	- host part - identify particular device in the network

**IPv4 Address**
- consists of 4 numbers, each 8 bits (2 hex digits), total 32 bits (8 hex digits)
- each numbers value range from 0 - 255 (0 - FF)
- example: 133.23.234.66
- classes from A to D, from large network to small network

**IPv6 Address**  
- consists of 8 hex numbers, each 16 bits (4 hex digits), total 128 bits (32 hex digits)
- each number value range from 0000 - FFFF
- example: 5EAA:0162:1687:B244:0016:022C:0001:09BD

**Domain Name**
is a representation of IP address

features:  
- easier for human to read and memorize
- each parts separated by a period ('.')
- example: www.google.com.hk
- generic top-level domain (gTLD)
	- commercial - .com
	- general organization - .org
	- educational - .edu
	- governmental - .gov
	- network - .net
	- individual - .idv
- country-code top-level domain (ccTLD)
	- china - .cn
	- japan - .jp
	- hong kong - .hk
	- united kingdom - .uk
	- canada - .ca
	- united states - .us
	- australia - .au

**Uniform Resource Locator (URL)**  
a particular location of resource on the Web  
e.g. http://www.originalpress.com/main/main_page.html
- http - protocol
- www - host name
- .originalpress - second level domain
- .com - TLD
- /main - folder name
- /main_page.html - file name

**Domain Name System (DNS)**  
translates domain names into relevant IP addresses and vice versa  

**Hypertext Transfer Protocol (HTTP)**  
- transfer hypertext file to World Wide Web  
- run on top of TCP/IP  
- file is stored in web server  
- displayed on web browser upon request by a client

## Terms
- transmission rate - speed of transfering data
- bandwith - maximum rate of data transfer across a path
- coverage - the distance where the network can cover
- latency - delay due to not enough transmission rate

## Network Switching
the process of **forwarding messages or informations** in networking

Categories:
- Connectionless - no previous communication is established
- Connection Oriented - pre-established communication is established

Types of switching:
- **Circuit Switching**
	- communicate over a **dedicated** communciation path 
	- **remains connected** during the communication session
- **Message Switching**
	- data is routed in its entirety
	- data is stored in the intermediate nodes
	- **store-and-forward** technique
- **Packet Switching**
	- entire data is broken down into smaller chunks called **packets**
	- info is added to the **header**
	- packages are stored and forwarded

## Error Detection
**check the reliability** of the digital data dilivered

Types:
- Repetition codes
	- sends the data multiple times
- Vertical redundancy check (**VRC**) / **Parity check**
	- **odd parity**
	- **even parity**
- Longitudinal redundancy check (**LRC**) / 2-D parity check
	- data arranged in 2D table with fixed rows and columns
- **Checksum**
	- modular arithmetic sum of data over a fixed word length
- Cyclic redundancy check (**CRC**)
	- based on remainder of a polynomial function