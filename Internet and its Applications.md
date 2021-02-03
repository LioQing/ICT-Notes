# Internet and its Applications

## The Networking and Internet Basics

## Types of network

**Local Area Network (LAN)**  
a network of computers and other devices over a geographical area **smaller** than WAN - a single or a group of buildings 

types of LAN:  

* Wired LAN
* Wireless LAN (WLAN)

**Wide Area Network (WAN)**  
composed of LANs connected through routers over a **larger** geographical area - a country or the world (**The Internet**)

### Types of Connections

* **peer-to-peer network** - computers are connected to nearby computers
  + examples
    - BitTorrent
    - P2PTV
    - PDTP
  + advantages
    - resources can be accessed by other users
    - encouraging community resource sharing and cooperation
  + disadvantages
    - Intellectual property law and illegal sharing
    - Network neutrality - extra bandwith-usage
* **client-server connection** - all computers are connected to a server
  + examples
    - dedicated server games
    - majority of the websites on the Internet
  + advantages
    - users can be given different levels of access to the data in the server
  + disadvantages
    - require connection to the dedicated server

| </empty>       | Client-Server                                                                                              | Peer-to-Peer                                                                                           |
|----------------|------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| machines       | server - machine(s) to provide services for clients, clients - machines requesting services from server(s) | no server, all machines request and share resources between others (peers)                             |
| installation   | servers are hard to configure                                                                              | easier                                                                                                 |
| administration | centralized                                                                                                | decentralized, hard to manage                                                                          |
| security       | secure                                                                                                     | less secure due to decentralized resources                                                             |
| failure        | when server fails                                                                                          | do not                                                                                                 |
| suitable in    | large no. of machines                                                                                      | small no. of machines                                                                                  |
| OSes           | OS for networking features (for peer-to-peer)                                                              | server: network OS, control resources; client: OS allowed to be identified and communicate with server |

<br>

**centralized data management**
with all data centralized in one network server, all authorized users are able to share the *latest and identical* information all the time.

## Hardware

**Network Interface Card (NIC)**  
provide interface for communication over network
has unique **Media Access Control (MAC)** address for identification

**Connection Devices**

* Hubs
  + can act as a repeater
  + multiple ports - connects computers
  + message received from one port is forwarded to all ports
  + cannot simultaneously transmit messages (collision will occur)
* Switches
  + multiple ports - connects computers
  + message received from one port is forward to destination port
  + can simultaneously transmit messages (less collision)
  + perform the forwarding according to MAC address of NIC of the destination
  + switch-based generally faster than hub-based network
* Repeater
  + amplify signals
  + remove noise
* Bridges
  + connect LANs of same type
* Routers
  + connect LANs of different type to form WAN
  + connect LANs and Internet
  + perform routing, i.e. find best path for packets to destination, and store routing table
  + perform forwarding according to IP address of the destination
* Access point
  + multiple devices connected to form a wireless network
  + may act as a router

**Modem**

* perform modulation - convert digital signals into analogue signals
* perform demodulation - convert analogue signals into digital signals
* examples
  + dial-up modem
  + cabble modem (cable TV)
  + Asymmetric Digital Subscriber Line (ADSL) modem

**Wires**

* telephone lines
* **coaxial cables**
  + electric signals
* **twisted-pair wires**
  + electric signals
  + twisted to reduce EM interference
  + 2 types
    - shielded twisted pair (**STP**) cables
    - unshielded twisted pair (**UTP**) cables
  + commonly used in LANs
* **optical fibres**
  + light signals
  + faster
  + difficult to eavesdrop
  + more expensive
  + require signal conversion device

| </empty>     | twisted pair cables | coaxial cables | optical fibres |
|--------------|---------------------|----------------|----------------|
| interference | relatively high     | medium         | low            |
| distance     | short               | medium         | very long      |

**Radio Connections**

* satellite broadband
  + through satellite by microwave
  + connects to internet wirelessly
* microwave broadband
  + between microwave stations
  + coverage: ~1.5 km
  + can be obstructed (straight line)
* wireless fidelity (Wi-Fi)
  + sender convert digital signal to radio signal
  + receiver convert radio signal to digital signal
  + require wireless NIC

## Network Switching (extra)

the process of **forwarding messages or informations** in networking

Categories:

* Connectionless - no previous communication is established
* Connection Oriented - pre-established communication is established

Types of switching:

* **Circuit Switching**
  + communicate over a **dedicated** communciation path 
  + **remains connected** during the communication session
* **Message Switching**
  + data is routed in its entirety
  + data is stored in the intermediate nodes
  + **store-and-forward** technique
* **Packet Switching**
  + entire data is broken down into smaller chunks called **packets**
  + info is added to the **header**
  + packages are stored and forwarded

## Multiplexing (extra)

method to **combine multiple signals** into one signal **over shared medium**  
e.g. multiple telephone calls carried out using one wire  

Types:

* Space-division multiplexing (**SDM**)
  + use of **separate point-to-point electrical conductors** for each channel
  + faster than TDM
  + require physical connection per communication pair
* Frequency-division multiplexing (**FDM**)
  + use of several distinct **frequencies** for each channel
  + used in analogue system
  + channel allocated any time
* Time-division multiplexing (**TDM**)
  + use at different **time** for each channel
  + require precise clock synchronization
* Code-division multiplexing (**CDM**)
  + use of same frequency, distinguish by **unique codes**
  + secure
  + complex scheme
* Wavelength-division multiplexing (**WDM**)
  + use of different **wavelength** of laser light for each channel
  + distinguish by refraction
  + require optic fiber
* Other types
  + Polarization-division multiplexing
  + Orbital angular momentum multiplexing

## Internet Access

**Internet Service Providers (ISP)** provide access to the Internet  

ways to connect:  

* dial-up access
  + requires dial-up modem & telephone line to connect to Internt via ISP
* Integrated Services Digital Network (ISDN)
  + requires a terminal adapter (TA) connected to a telephone line
* leased line
  + dedicated line that provide digital comminication services
  + example:  
    - T-carriers
* broadband connection
  + by any means (optical fibre, coaxial, twisted-pair) faster than dial-up access
  + example:
    - asymmetric digital subscriber line (ADSL)
    - symmetric digital subscriber line (SDSL)
    - cable modem 
* wireless Internet access
  + by not using any wired connection, generally by microwave or radiowave connections
  + example:
    - Wi-Fi hot spots
    - mobile broadband
    - wireless application protocol (WAP)
    - general packet radio services (GPRS)
    - high speed packet access (HSPA) and HSPA+

| </empty>           | dial-up           | ISDN                     | leased line                                  | broadband                        | wireless       |
|--------------------|-------------------|--------------------------|----------------------------------------------|----------------------------------|----------------|
| transmission speed | low (max 56 kbps) | low (basic max 128 kbps) | medium (depends on type: ~1 Mbps - ~50 Mbps) | medium (depends on DSL or modem) | medium to fast |
| cost               | usually low       | medium                   | high                                         | medium                           | low to high    |
| physical security  | low               | medium                   | high                                         | low                              | N/A            |

## Communication Software and Protocols

**communication software** is a software that provide fast and effective way for intert access or activity

typical softwares:  

* web browser
  + for surfing the Internet
  + extensions or features to enhance browsing experiences
* email programs
  + to send and receive emails
* newsgroup program
  + receive news
* instant messaging programs (IM)
  + for message communication with other devices with the same software
* file transfer program
  + to send files to other devices
* telnet program
  + to remotely control another deveice or server through CLI
* social networking software
  + to share text/image/video on the Internt
  + for browsing text/image/video shared by others on the Internet
* video conferencing software
  + to communicate through live video with others with the same software

<br>

**protocols** are a set of rules guiding communcation between computer systems through standardization

open system interconnection (OSI) mode:

1. Physical layer
2. Data link layer (Frame)
3. Network layer (Packet)
  + IP
4. Transport layer (Datagram)
  + TCP, UDP
5. Session layer
6. Presentation layer
7. Application layer (Data)
  + FTP, HTTP

**Transmission Control Protocol (TCP)**  
responsible for:

* division of messages into packets
* transmission
* verificaiton
* reassembling of packets

**Internet Protocol (IP)**  
responsible for:  

* divide packets into fragments (smaller pieces) according to the transmission rate
* routing the packets to destination

**IP Addess**

* for identifying the device with the network interface
* all devices using IP will have an IP address
* IP identify destinations according to IP address
* IP address have 2 parts
  + network part - identify the network on the Internet
  + host part - identify particular device in the network

**IPv4 Address**

* consists of 4 numbers, each 8 bits (2 hex digits), total 32 bits (8 hex digits)
* each numbers value range from 0 - 255 (0 - FF)
* example: 133.23.234.66
* classes for networks of different sizes

**IPv6 Address**  

* consists of 8 hex numbers, each 16 bits (4 hex digits), total 128 bits (32 hex digits)
* each number value range from 0000 - FFFF
* example: 5EAA:0162:1687: B244:0016:022C:0001:09BD

**Domain Name**
is a representation of IP address

features:  

* easier for human to read and memorize
* each parts separated by a period ('.')
* example: www.google.com.hk
* generic top-level domain (gTLD)
  + commercial - .com
  + general organization - .org
  + educational - .edu
  + governmental - .gov
  + network - .net
  + individual - .idv
* country-code top-level domain (ccTLD)
  + china - .cn
  + japan - .jp
  + hong kong - .hk
  + united kingdom - .uk
  + canada - .ca
  + united states - .us
  + australia - .au

**Uniform Resource Locator (URL)**  
a particular location of resource on the Web  
e.g. http://www.originalpress.com/main/main_page.html

* http - protocol
* www - host name
* .originalpress - second level domain
* .com - TLD
* /main - folder name
* /main_page.html - file name

**Domain Name System (DNS)**  
translates domain names into relevant IP addresses and vice versa, the process is called **name resolution**  

**Hypertext Transfer Protocol (HTTP)**  

* transfer hypertext file to World Wide Web  
* run on top of TCP/IP  
* file is stored in web server  
* displayed on web browser upon request by a client

## Terms for Answering Questions

* transmission rate - amount of data transfer per unit time
* bandwith - maximum rate of data transfer across a path
* coverage - the distance where the network can cover
* latency - delay due to not enough transmission rate

## Internet Services and Applications

## Search Engine

def: a set of program allowing user to find information on WWW with keywords

types:

* general searches
  + Google
  + Yahoo!
* specialized searches
  + Medlin Plus
  + Bloomberg
  + Business.com
* general searches using natural languages
  + Ask Jeeves!

techiniques:

* use precise keyword
* use "+" in front of a word for finding the exact term
* use "-" in front of a word for eliminating the exact term
* use double quotation ("") at a phrase for finding the exact phrase
* using wildcard (*) for searching part of a word (e.g. comput\* for computer, computing, etc.)
* using boolean searching

**Quality of Information**  

* completeness
* accuracy
* authority
* objectivity
* timeliness
* legality

## Internet Services

graphics:

* bitmaps
  + bmp
  + jps/jpeg
  + gif
  + png
* vector graphics
  + swf
  + svf
  + wmf
  + eps

audio:

* wav
* wma
* mp3
* aac
* ogg

video:  

* wmv
* rm
* mov
* flv
* mpeg
* avi

**plug-ins**  
def: an add-on program for playing a particular multimedia element

example:  

* Flash Player *(RIP)* for flash content (.flv)  
* Acrobat Reader for Acrobat documents (.pdf)
* QuickTime for QuickTime audio and video files (.mov)

advantages:  

* keep web browser efficient & small file size
* keep browser up-to-date to handle latest multimedia elements

***E-mails***  
format of an e-mail address:  
userid@domain.com

userid: User ID  
domain.com: mail server domain name  

features:  

* To
* From
* Subject
* Content/Body

optional features:  

* CC (Carbon copy) - one or more addresses of recipients to receive a copy
* BCC (Blind Carbon Copy) - destination e-mail addresses are not listed in the header
* Signature - pice of text at the end of the message to identify the sender

protocols:  
**Simple Mail Transfer Protocol (SMTP)**  
used for: 

* from sender's PC to sender's mail server
* from sender's mail server to receiver's mail server

**Post Office Proticol (POP)**  
currently POP3 is the standard  

used for:

* from receiver's server to receiver's PC
* the e-mails on the server are usually deleted after download to save space

**Internet Message Access Protocol (IMAP)**  
currently IMAP4 is the standard  

used for:

* from receiver's server to receiver's PC
* stores all read and unread e-mails on the mail server

complete process:  
sender's computer   
=SMTP=> sender's mail server  
=SMTP=> Internet  
=SMTP=> receiver's mail server  
=POP/IMAP=> receiver's computer

extension:  
**Multipurpose Internet Mail Extension**  
used for:  

* send non-text e-mail attachments (e.g. photos, video, audio, word documents)
* included in the e-mail header

***File Transfer Protocol (FTP)***
feature:  

* client-server network model => user authentication
* anonymous FTP servers  

file transfer mode:  

* ASCII transfer mode - sent as plain text
* binary mode - sent bit by bit and receiver's computer reassemble the bit stream

***Remote Logon***  
feature:

* for remote control of a computer through Internet
* telnet was the first protocol for this purpose (CLI interface)
* telnet was replaced by newer protocol, Secure Sheel (SSH)

***Newsgroup***  
feature:

* threaded disuccion/categorized
* newsreader program/web browser for reading, posting, browsing messages
* largely replaced by forums and blogs now

***Discussion Forums***  
feature:  

* consists of subforums, which may have several different topics
* informations kept on specific servers by the owner
* user authentication

***Online Chat***  
refers to one-to-one or one-to-many dicussion over Internet

feature:

* can be text-based or voice based
* some program support video with voice-chat
* examples such as Skype, Yahoo!, Discord

## Streaming Technology

the client start decoding and playing the file after *a small portion of file is received*  

types:

* webcasting
* voice mail
* video conferencing

## Applications

* E-commerce
  + models
    - Business-to-Business (B2B)
    - Business-to-Consumer (B2C)
    - Consumer-to-Consumer (C2C)
* E-government
* E-learning
* E-entertainment

## HTML

name: HyperText Markup Language  
extension: .htm/.html  
usage: display web page contents including text, images, and other multimedia elements  
structure:  

* tags usually in pairs
* standard source file with a head and a body
* each tag can have attributes  

``` html
<html>

<head>
  <h1>Header Here</h1>
</head>

<body>
  <p>This is a paragraph</p>
</body>

</html>
```

tags: https://www.w3schools.com/tags/ref_byfunc.asp

## Elementary Web Authoring

**website**  
definition: a collection of web pages of the same theme  

3 stages of establishing a website:  

1. planning
  + determine objectives
  + determine theme
  + collect information on intended users
  + collect relevant contents
  + design structure
    - linear structure
    - hierarchical structure
    - cyclic structure
2. construction
  + design the layout for arrangement of multimedia elements
  + consider issues like use of frames, location of menu for navigation, etc.
  + organize files and folders
  + conduct testing  and upload web page to server
3. maintenance
  + update website contents
  + replace broken/out-dated links

factors:

* font
  + font face
  + font style
  + font size
* color
  + text color
  + background color
* arrangement of information
  + table
  + list
* multimedia elements
  + video
  + images
  + audio
* navigation
  + a frame for menu
* links
  + meaningful text for the hyperlink for user to understand
* updates
  + provide information on the update of the website
* languages
* site map for navigation
* testing in various web browsers
* use of e-mail, discussion forum, form to collect feedback

tools:

* web authoring tool
  + do not directly require HTML
  + effects of 'what-you-see-is-what-you-get'
* text editor
  + for editing HTML
