[Domain 4](#domain4-top) **Communication and Network Security**

Networking can be one of the more complex exam topics; if you have a networking background, you likely won’t find this domain difficult-- if not, spend extra time in this section and consider diving deeper into topics that are fuzzy

[4.1](#4.1) Assess and implement secure design principles in network architectures

- **OSI**: Open Systems Interconnection (OSI) Reference Model developed by ISO (International Organization for Standardization) to establish a common communication structure or standard for all computer systems; it is an abstract framework
    - Communication between layers via **encapsulation** (at each layer, the previous layer's header and payload become the payload of the current layer) and **deencapsulation** (inverse action occurring as data moves up layers)

| Layer | OSI model layer | TCP/IP model | PDU | Devices | Protocols | 
|-----|---------------| -------------------|------------| ----------------|-----------|
| 7     | Application     | Application |Data               | L7 firewall                                | HTTP/s, DNS, DHCP, FTP,S-HTTP, TPFT, Telnet, SSH, SMTP, POP3, PEM, IMAP, NTP, SNMP, TLS/SSL, GBP, RIP, SIP, S/MIME etc. |
| 6     | Presentation    | Application |Data               | L7 firewall                                | All the above                                                |
| 5     | Session         | Application| Data               | L7 firewall                                | All the above                                                |
| 4     | Transport       | Transport (host-to-host) | Segments           | L4 firewall                                | TCP (connection oriented), UDP (connectionless oriented)     |
| 3     | Network         | Internet/IP | Packets            | Router, Multiplayer Switch, Router         | IPv4, IPv6, IPSec, OSPF, EIGRP                               |
| 2     | Data Link       | Network Access | Frames             | Switch, Bridge, NIC, Wireless Access Point | MAC, ARP Ethernet 802.3 (Wired), CDP, LLDP, HDLC, PPP, DSL, L2TP, IEEE 802.11 (Wireless), SONET/SDH |
| 1     | Physical        | Network Access | Bits               | All the above                              | Electrical signal (copper wire), Light signal (optical fibre), Radio signal (air) |

### OSI layers in details
- Mnemonics:
    - from top: All People Seem To Need Delicious Pizza
    - from bottom: Please Do Not Throw Sausage Pizza Away
- Application Layer (7)
    - Responsible for:
        - interfacing user applications, network services, or the operating system with the protocol stack 
        - identifying and establishing availability of communication partners 
        - determining resource availability and 
        - synchronizing communication
- Presentation Layer (6)
    - Responsible for transforming data into the format that any system following the OSI model can understand
    - Associated tasks:
        - data representation
        - character conversion
        - data compression
        - data encryption
- Session Layer (5)
    - Responsible for establishing, maintaining, and terminating communication sessions between two computers
    - Three communication session phases: 
        - connection establishment
            - **simplex**: one-way
            - **half-duplex**: both comm devices can transmit/receive, but not at the same time
            - **full-duplex**: both comm devices can transmit/receive at same time
        - data transfer
        - connection release
- Transport Layer (4)
    - Responsible for managing the integrity of a connection and controlling the session; providing transparent data transport and end-to-end transmission control
    - Defines session rules like how much data each segment can contain, how to verify message integrity, and how to determine whether data has been lost
    - Protocols that operate at the Transport layer:
        - Transmission Control Protocol (TCP)
            - full-duplex, connection-oriented protocol
            - uses three-way handshake
        - User Datagram Protocol (UDP)
            - connectionless protocol that provides fast, best-effort delivery of **datagrams** (self-container unit of data)
        - Transport Layer Security (TLS)
- Network Layer (3)
    - Responsible for logical addressing, and providing routing or delivery guidance (but not necessarily verifying guaranteed delivery), manages error detection and traffic control
    - **routing protocols**: move routed protocol messages across a network
        - includes RIP, OSPF, IS-IS, IGRP, and BGP
        - routing protocols are defined at the Network Layer and specify how routers communicate
        - routing protocols can be static or dynamic, and categorized as interior or exterior
        - **static routing protocol**: requires an admin to create/update routes on the router
        - **dynamic**: can discover routers and determine best route to a given destination; routing table is periodically updated
        - **distance-vector**: (interior) makes routing decisions based on distance (e.g. hop count), and vector (router egress interface); examples:
            - **Routing Information Protocol (RIP)**: a distance-vector protocol that uses hop count as its routing metric
            - Interior Gateway Routing Protocol (IGRP)
            - Enhanced Interior Gateway Routing Protocol (EIGRP)
        - **link state**: (interior) uses router characteristics (e.g. speed, latency, error rates) to make next hop routing decisions; examples:
            - Open Shortest Path First (OSPF)
            - Intermediate System to Intermediate System (IS-IS)
        - interior vs exterior:
            - interior routing protocols ("myopic") make next hop decisions based only on info related to the next immediate hop
            - exterior routing protocols ("far-sighted")make hop decisions based on the entire remaining path (i.e.) vector
            - **Border Gateway Protocol (BGP)**: an exterior/path vector protocol
    - Routed protocols include Internetwork Package Exchange (IPX) and Internet Protocol (IP)
     - IP is part of the TCP/IP (Transmission Control Protocol/Internet Protocol) suite
        - IP provides the foundation for other protocols to be able to communicate; IP itself is a connectionless protocol
        - IPv4 uses 32-bit addresses
        - IPv6 uses 128-bit addresses
        - TCP or UDP is used to communicate over IP 
        - IPSec provides data authentication, integrity and confidentiality
    - **logical address**: occurs when an address is assigned and used by software or a protocol rather than being provided/controlled by hardware
    - Network layer’s packet header includes the source and destination IP addresses
    
- Data Link Layer (2)
    - Responsible for formatting a packet for transmission
    - adds the source and destination hardware addresses to the frame
    - Media Access Control (MAC)(hardware-based) address/AKA NIC address
        - MAC address is a 6-byte (48-bit) binary address written in hex
            - first 6b/48-bits: Organizationally Unique Identifier (OUI) - denotes manufacturer
            - last 3b/24-bits: unique to that interface
    - **Address Resolution Protocol (ARP)**: operates at layer 2
    - Switches & bridges function at this layer

- Physical Layer (1)
    - Converts a frame into bits for transmission/receiving over the physical connection medium
    - Network hardware devices that function at layer 1 include NICs, hubs, repeaters, concentrators, amplifiers
    - Know four basic network topologies:
        - **star**: each individual node on the network is directly connect to a switch/hub/concentrator
        - **mesh**: all systems are interconnected; partial mesh can be created by adding multiple NICs or server clustering
        - **ring**: closed loop that connects end devices in a continuous ring (all communication travels in a single direction around the ring);
            - **Multistation Access Unit** (MSAU or MAU) connects individual devices
            - used in token ring and FDDI networks
        - **bus**: all devices are connected to a single cable (backbone) terminated on both ends
    - Know commonly used twisted-pair cable categories
    - Know Cable types & characteristics


### TCP/IP layers
- Network Access Layer: defines the protocols and hardware required to deliver data across a physical network
- Internet Layer: defines the protocols for logically transmitting packets over the network
- Transport Layer: defines protocols for setting up the level of transmission service for applications; this layer is responsible for the reliable transmission of data and the error-free delivery of packets
- Application Layer: defines protocols for node-to-node application communication and provides services to the application software running on a computer

Secure protocols

- **Kerberos**: standards-based network authentication protocol, used in many products (most notably Microsoft Active Directory (Active Directory Domain Services or AD DS)     
    - Kerberos is mostly used on
LANs for organization-wide authentication, single sign-on (SSO) and authorization

- SSL and TLS: data protection used for protecting website transactions (e.g. banking, ecommerce)
    - SSL and TLS both offer data encryption, integrity and authentication. 
    - TLS has suplanted SSL (the original protocol, considered a legacy/insecure) 
    - TLS was initially introduced in 1999 but didn’t gain widespread use until years later
    - The original versions of TLS (1.0 and 1.1) are considered deprecated and organizations should be relying on TLS 1.2 or TLS 1.3
- **SFTP**: a version of FTP that includes encryption and is used for transferring files between two devices (often a client / server).
- **SSH**: remote management protocol, which operates over TCP/IP
    - all communications are encrypted
    - primarily used by IT administrators to manage devices such as servers and network devices
- **IPSec**: an IETF standard suite of protocols that is used to connect nodes (e.g. computers or
office locations) together
    - widely used in virtual private networks (VPNs)
    - IPSec provides encryption, authentication and data integrity

Micro-Segmentation
- Software-defined networks:
- Virtual extensible local area network (VXLAN):
- Encapsulation:
- Software-defined wide area network (SD-WAN):

Wireless Networks
- Li-Fi:
- Wi-Fi:
    - Wired Equivalent Privacy (WEP):
    - Wi-Fi Protected Access II: (WPA2):
    - Frequency table:
- Zigbee:
- Satellite:

Cellular Networks

Content Distribution Network (CDN)

[4.2](#4.2) Secure network components

[4.3](#4.3) Implement secure communication channels according to design
