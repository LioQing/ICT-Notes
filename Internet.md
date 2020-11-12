# Internet and its Applications

some temporary notes:

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