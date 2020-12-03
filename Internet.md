# Internet and its Applications

## The Networking and Internet Basics

### Local Area Network (LAN)
a network of personal computers or workstations which covers a geographical area smaller than WAN - a single or a group of buildings 

### Wide Area Network (WAN)
composed of LANs connected through routers, covers a larger geographical area - a country or the world

### Types of Connections
- Peer-to-Peer network - computers are connected to nearby computers
- Client-Server connection - all computers are connected to a server

</empty> | Peer-to-Peer | Client-Server
--- | --- | ---
machines | server - machine(s) to provide services for clients, clients - machines requesting services from server(s) | no server, all machines request and share resources between others (peers)
installation | servers are hard to configure | easier
administration | centralized | decentralized, hard to manage
security | secure | less secure due to decentralized resources
failure | when server fails | do not
suitable in | large no. of machines | small no. of machines
<br>

### Hardware

**Network Interface Card (NIC)**
	provide interface for communication over network
	has unique Media Access Control (MAC) address for identification

**Connection Devices**
- Hubs
	- connect server and computers
	- message received from one port is forwarded to all ports
	- cannot simultaneously transmit messages
- Switches
	- message received from one port is forward to destination port
	- can simultaneously transmit messages
	- perform the forwarding according to MAC address of the destination
- Repeater
	- amplify signals
	- remove noise
- Bridges
	- connect LANs of same type
- Routers
	- can connect LANs of different type
	- connect LANs and Internet
	- perform routing, i.e. find best path for packets to destination
	- perform forwarding according to IP address of the destination
- Access point
	- multiple devices connected to form a wireless network
	- may act as a router

some temporary notes:

## Terms
- transmission rate - speed of transferring files
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

## Multiplexing
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

## Peer-to-peer Network (P2P)
an architecture that partition tasks or workload between peers  

Peers:
- equipotent in the network
- **share part of their resources** (e.g. processing power) to other peers
- are both the consumer and the supplier

Usage:
- **File sharing**
	- BitTorrent
- **Multimedia**
	- P2PTV
	- PDTP

Advantages:
- Encouraging community resource sharing and cooperation

Disadvantages:
- Intellectual property law and **illegal sharing**
- Network neutrality - extra bandwith-usage
