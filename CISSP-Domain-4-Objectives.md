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
| 4     | Transport       | Transport (host-to-host) | Segments           | L4 firewall                                | TCP (connection oriented), UDP (connectionless)     |
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
    - Adds the source and destination hardware addresses to the frame
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
    - Know cable types & characteristics


### TCP/IP layers
- Network Access Layer: defines the protocols and hardware required to deliver data across a physical network
- Internet Layer: defines the protocols for logically transmitting packets over the network
- Transport Layer: defines protocols for setting up the level of transmission service for applications; this layer is responsible for the reliable transmission of data and the error-free delivery of packets
- Application Layer: defines protocols for node-to-node application communication and provides services to the application software running on a computer

### Secure protocols

- **Kerberos**: standards-based network authentication protocol, used in many products (most notably Microsoft Active Directory Domain Services or AD DS)     
    - Kerberos is mostly used on
LANs for organization-wide authentication, single sign-on (SSO) and authorization

- SSL and TLS: data protection used for protecting website transactions (e.g. banking, ecommerce)
    - SSL and TLS both offer data encryption, integrity and authentication 
    - TLS has suplanted SSL (the original protocol, considered legacy/insecure) 
    - TLS was initially introduced in 1999 but didn’t gain widespread use until years later
    - The original versions of TLS (1.0 and 1.1) are considered deprecated and organizations should be relying on TLS 1.2 or TLS 1.3
- **SFTP**: a version of FTP that includes encryption and is used for transferring files between two devices (often a client / server)
- **SSH**: remote management protocol, which operates over TCP/IP
    - all communications are encrypted
    - primarily used by IT administrators to manage devices such as servers and network devices
- **IPSec**: an IETF standard suite of protocols that is used to connect nodes (e.g. computers or
office locations) together
    - widely used in virtual private networks (VPNs)
    - IPSec provides encryption, authentication and data integrity

### Micro-Segmentation
- **Software-defined networks (SDN)**:
    - SDN is effectively network virtualization, and separates the infrastructure layer (aka the data or forwarding plane) - hardware and hardware-based settings, from the control layer - network services of data transmission management
        - NOTE: the **control plane**: uses protocols to decide where to send traffic, and the **data plane**: includes rules that decide whether traffic will be forwarded
    - typically ABAC-based
    - an SDN solution provides the option to handle traffic routing using simpler network devices that accept instructions from the SDN controller
    - SDN offers a network design that is directly programmable from a central location, is flexible, vendor neutral, and based on open standards
    - Allows org to mix/match hardware
- **Virtual extensible local area network (VXLAN)**:
    - an encapsulation protocol that enables VLANs to be stretched across subnets and geographic distances
    - Typically restricted to layer 2
    - Allows up to 16 million virtual networks (VLAN liit is 4096)
    - VXLAN can be used as a means to implement microsegmentation without limiting segments to local entities only
    - Defined in RFC 7348

- Encapsulation:
    - the OSI model represents a protocol stack, or a layered collection of multiple protocols, and communication between protocol layers occurs via encapsulation and deencapsulation (defined above)

- **Software-defined wide area network (SD-WAN)**:an evolution of SDN that can be used to manage the connectivity and control services between distant data centers, remote locations, and cloud services over WAN links

### Wireless Networks
- Li-Fi:
- Wi-Fi:
    - **Wired Equivalent Privacy (WEP)**:
        - WEP is defined by the original IEEE 802.11 standard
        - WEP uses a predefined shared Rivest Cipher 4 (RC4) secret key for both authenitcation (SKA) and encryption
        - Shared key is static
        - WEP is weak from RC4 flaws 
    - Wi-Fi Protected Access II: (WPA2):
        - IEEE 802.11i or Wi-Fi Protected Access 2 (WPA2) replaced WEP and WPA
        - Uses AES-CCMP (Counter Mode with Cipher Block Chaining Message Authentication Code Protocol
    - Frequency table:
    
| Amendment | Wi-Fi Alliance | Speed | Frequency |
|-----|---------------| -------------------|------------|
| 802.11    |   --   | 2 Mbps |2.4 GHz               |
| 802.11a   |  Wi-Fi 2    | 54 Mbps |2.4 GHz               |
| 802.11b   |  Wi-Fi 1    | 11 Mbps |2.4 GHz               |
| 802.11g   |  Wi-Fi 3    | 54 Mbps |2.4 GHz               |
| 802.11n   |  Wi-Fi 4    | 200+ Mbps |2.4 GHz               |
| 802.11ac   | Wi-Fi 5    | 1 Gbps |2.4 GHz               |
| 802.11ax   | Wi-Fi 6/Wi-Fi 6E     | 9.5 Gbps |2.4 GHz               |

- **Zigbee**: IoT equipment communications concept based on Bluetooth
    - Low power/low throughput
    - Requires close proximity
    - Encrypted using 128-bit symmetric algorithm
- **Satellite**: primarily uses radio waves between terrestrial locations and an orbiting artificial satellite
    - Supports telephone, tv, radio, internet, military communications
    - 3 primary orbits:
        - LEO: low Earth orbit (160-2k km)
            - have stronger signals
            - multiple devices needed to maintain coverage (e.g. Starlink)
        - MEO: medium Earth orbit (2k-35768 km)
            - above a terrestrial location longer than LEO
            - higher orbit, additional delay/weaker signal
        - GEO: geostationary orbit (35768 km)
            - maintain a fixed position above a terrestrial location, and ground stations can use fixed antennas
            - larger transmissino footprint than MEO, but higher latency

### Cellular Networks
- A cellular network or a wireless network is the primary communications technology used by many mobile devices
- Cells are primary transceiver (cell site/tower)
- Generally encrypted between mobile device and transmission tower; plaintext over wire; use encryption like TLS/VPN
- 4G
    - 4G allows for mobile devices to achieve 100 Mbps, and stationary devices can reach 1 Gbps
    - LTE and WiMAX are common transmission systems
- 5G
    - 5G uses higher frequencies than previous tech, allowing for higher transmission speeds — up to 10 Gbps, but at reduced distances
    - Orgs need to enforce secsurity requirements on 5G
- Security issues with wireless:
    - provider network (voice or data) is not necessarily secure
    - your cell phone can be intercepted
    - provider's towers can be simulated to conduct man-in-the-middle/on-path attack
    - using cell connectivity to access the internet or your office network creates a potential bridge, provider attackers with another avenue

**Content Distribution Network (CDN)**: a collection of resource services deployed in numerous data centers across the internet in order to provide low latency, high performance, and high availability of the hosted content
- CDNs provide multimedia performance quality through the concept of distributed data hosts, geographically distributed, closer to groups of customers
- Provides geographic and logical load balancing; lower-latency and higher-quality throughput
- Client-based CDN is often referred to as P2P (peer-to-peer)

[4.2](#4.2) Secure network components

[4.3](#4.3) Implement secure communication channels according to design
