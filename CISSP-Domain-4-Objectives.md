[Domain 4](#domain4-top) **Communication and Network Security**

Networking can be one of the more complex exam topics; if you have a networking background, you likely won’t find this domain difficult-- if not, spend extra time in this section and consider diving deeper into topics that are fuzzy

[4.1](#4.1) Assess and implement secure design principles in network architectures

- **OSI**: Open Systems Interconnection (OSI) Reference Model developed by ISO (International Organization for Standardization) to establish a common communication structure or standard for all computer systems; it is an abstract framework
    - Communication between layers via **encapsulation** (at each layer, the previous layer's header and payload become the payload of the current layer) and **deencapsulation** (inverse action occurring as data moves up layers)

| Layer | OSI model layer | TCP/IP model | PDU | Devices | Protocols | 
|-----|---------------| -------------------|------------| ----------------|-----------|
| 7     | Application     | Application |Data               | L7 firewall                                | HTTP/s, DNS, DHCP, FTP, S-HTTP, TPFT, Telnet, SSH, SMTP, POP3, PEM, IMAP, NTP, SNMP, TLS/SSL, GBP, RIP, SIP, S/MIME etc. |
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
            - exterior routing protocols ("far-sighted") make hop decisions based on the entire remaining path (i.e.) vector
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
    - Media Access Control (MAC) - (hardware-based) address/AKA NIC address
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
    - Allows up to 16 million virtual networks (VLAN limit is 4096)
    - VXLAN can be used as a means to implement microsegmentation without limiting segments to local entities only
    - Defined in RFC 7348

- Encapsulation:
    - the OSI model represents a protocol stack, or a layered collection of multiple protocols, and communication between protocol layers occurs via encapsulation and deencapsulation (defined above)

- **Software-defined wide area network (SD-WAN)**: an evolution of SDN that can be used to manage the connectivity and control services between distant data centers, remote locations, and cloud services over WAN links

### Wireless Networks
- Li-Fi: **light fidelity (Li-Fi)**: a form of wireless communication technology that relies on light to transmit data, with theorectical speeds up to 224Gbits/sec
- Wi-Fi:
    - **Wired Equivalent Privacy (WEP)**:
        - WEP is defined by the original IEEE 802.11 standard
        - WEP uses a predefined shared Rivest Cipher 4 (RC4) secret key for both authentication (SKA) and encryption
        - Shared key is static
        - WEP is weak from RC4 flaws 
    - Wi-Fi Protected Access II (WPA2):
        - IEEE 802.11i WPA2 replaced WEP and WPA
        - Uses AES-CCMP (Counter Mode with Cipher Block Chaining Message Authentication Code Protocol)
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
            - larger transmission footprint than MEO, but higher latency

### Cellular Networks
- A cellular network or a wireless network is the primary communications technology used by many mobile devices
- Cells are primary transceiver (cell site/tower)
- Generally encrypted between mobile device and transmission tower; plaintext over wire; use encryption like TLS/VPN
- 4G
    - 4G allows for mobile devices to achieve 100 Mbps, and stationary devices can reach 1 Gbps
    - LTE and WiMAX are common transmission systems
- 5G
    - 5G uses higher frequencies than previous tech, allowing for higher transmission speeds — up to 10 Gbps, but at reduced distances
    - Orgs need to enforce security requirements on 5G
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

The components of a network make up the backbone of the logical infrastructure for an organization. These components
are often critical to day-to-day operations, and an outage or security issue can be very costly

Here are issues to pay attention to:
- Operation of hardware (e.g. redundant power, warranty, support)
    - Modems are a type of Channel Service Unit/Data Service Unit (CSU/DSU) typically used for converting analog signals into digital; the CSU handles communication to the provider network, the DSU handles communication with the internal digital equipment (in most cases, a router)
        - Modems typically operate at Layer 2 
        - Routers operate at Layer 3, and make the connection from a modem available to multiple devices in a network, including switches, access points and endpoint devices 
        - Switches are typically connected to a router to enable multiple devices to use the connection
        - Switches help provide internal connectivity, as well as create separate broadcast domains when configured with VLANs 
        - Switches typically operate at Layer 2 of the OSI model, but many switches can operate at both Layer 2 and Layer 3
        - Access points can be configured in the network topology to provide wireless access using one of the protocols and encryption algorithms
    - Redundant power: most home equipment use a single power supply, if that supply fails, the device loses power
        - redundant power is typically used with components such as servers, routers, and firewalls
        - redundant power is usually paired with other types of redundancies to provide high availability
- Transmission Media: come in many forms, not just cables
    - Includes wireless, LiFi, Bluetooth, Zigbee, satellites
    - Most common cause of network failure (i.e. violations of availability) are cable failures or misconfigurations
    - Wired transmission media can typically be described in three categories: coaxial, Ethernet, fiber
    - Coaxial is typically used with cable modem installations to provide connectivity to an ISP, and requires a modem to convert the analog signals to digital
        - fairly resistent to EMI
        - longer lengths than twisted pair
        - requires segment terminators
        - two main types:
            - **thinnet (10Base2)**: used to connect systems to backbond trunks of thicknet cabling (185m, 10Mbps)
            - **thicknet (10Base5)**: can span 500 meters and provide up to 10Mbps
    - Ethernet can be used to describe many mediums, it is typically associated with Category 5/6 unshielded twisted-pair (UTP) or shielded twisted pair (STP), and can be plenum-rated
    - Fiber typically comes in two options: single-mode or multi-mode
        - Single-mode is typically used for long-distance communication, over several kilometers or miles
        - Multi-mode fiber is typically used for faster transmission, but with a distance limit depending on the desired speed
        - Fiber is most often used in the datacenter for backend components

    | Category | Throughput | Notes |
    |----------|------------|--------|
    | Cat 1    |   1 Mbps   |        |
    | Cat 2    |   4 Mbps   |        |
    | Cat 3    |   10 Mbps  |        |
    | Cat 4    |   16 Mbps  |        |
    | Cat 5    |   100 Mbps |        |
    | Cat 5e   |   1 Gbps   |        |
    | Cat 6    |   1 Gbps   |        |
    | Cat 6a   |   10 Gbps  |        |
    | Cat 7    |   10 Gbps  |        |
    | Cat 8    |   40 Gbps  |        |


- Network Access Control (NAC) devices
    - NAC is the concept of controlling access to an environment through strict adherence to and enforcement of security policy
    - NAC is meant to be an automated detection and response system that can react in real time to ensure that all monitored systems are patched/updated and have current security configurations, as well as keep unauthorized devices out of the network
    - NAC goals:
        - prevent/reduce known attacks directly and zero-day indirectly
        - enforce security policy throughout the network
        - use identities to perform access control
    - NAC can be implemented with a preadmission or postadmission philosophy:
        - **preadmission philosohpy**: requires a system to meet all current security requirements (such as patch application and malware scanner updates) before it is allowed to communicate with the network
        - **postadmission philosophy**: allows and denies access based on user activity, which is based on a predefined authorization matrix
    - Agent-based NAC:
        - Installed on each management system, checks config files regularly, and can quarantine for non-compliance
        - Dissolvable: usually written in a web/mobile language and is executed on each local machine when the specific management web page is accessed (such as captive portal);
        - Permanent: installed on the monitored system as a persistent background service
    - Just as you need to control physical access to equipment and wiring, you need to use logical controls to protect a network; there are a variety of devices that provide this type of protection, including:
        - Stateful and stateless firewalls can perform inspection of the network packets and use rules, signatures and patterns to determine whether the packet should be delivered
            - reasons for dropping a packet could include addresses that don’t exist on the network, ports or addresses that are blocked, or the content of the packet (e.g malicious packets blocked by administrative policy)
        - Intrusion detection and prevention devices which monitor the network for unusual network traffic and MAC or IP address spoofing, and then either alert on or actively stop this type of traffic
        - Proxy/reverse proxies: 
            - proxy servers can be used to proxy internet-bound traffic, instead of letting clients talk directly
            - reverse proxies are often deployed to a perimeter network; they proxy communication from the internet to an internal host, such as a web server
            - like a firewall, a reverse proxy can use rules and policies to block certain types of communication
- Endpoint security: each individual device must maintain local security
    - Any weakness in a network, whether border, server, or client-based presents a risk to all elements of the organization
    - Client/Server model is a distributed architecture, which means that security must be addressed everywhere instead of at a single centralized host
    - Processing, storage on clients and servers, network links, communication equipment all must be secured
    - Clients must be subjected to policies that impose safeguards on their content and users’ activities including:
        - email
        - upload/download policies and screening
        - subject to robust access controls (e.g. MFA)
        - file encryption
        - screen savers
        - isolated processes for user/supervisor modes
        - local files should be backed up
        - protection domains/network segments
        - security awareness training
        - desktop env should be included in org DR
        - Endpoint Detection and Response (EDR)/Managed Detection and Response (MDR) should be considered

[4.3](#4.3) Implement secure communication channels according to design
- Protocols that provide security services for application-specific communication channels are called secure communication protocols
- Voice
    - as more organizations switch to VoIP, protocols like SIP become more common, and introducing additional management, either via dedicated voice VLANs, or by establishing quality of service (QoS) levels to ensure voice traffic priority
    - web-based voice apps can be more difficult to manage, causing additional unplanned bandwidth consumption

- Multimedia collaboration
    - there are a variety of new technologies that allow instant organizational collaboration, including smartboards, and products that enhance on-site, hybrid, or virutal meetings
    - mobile communication apps are a huge market, and will continue to grow, increasing the complexity of mobile security
- Remote access
    - 4 main types of remote access:
        - **service specific**: gives users the ability to remotely connect to and manipulate or interact with a single service (e.g. email)
        - **remote-control**: grants a remote user the ability to fully control another system that is physically distant
        - **remote node operation**: AKA remote client connecting directly to a LAN
        - **screen scraping**: refers to 1) remote control, remote access, or remote desktop services or 2) technology that allows an automated tool to interact with a human interface
    - Virtual Private Network (VPN): virtual private network is a traditional remote access technology
    - Web Application Proxy (WAP): provides secure remote access and single sign-on.
    - Virtual Desktop Infrastructure (VDI): centralizes desktop environments on remote servers, allowing users to access virtual desktops
    - Virtual Mobile Interface (VMI): allows organizations to host mobile apps and data on a centralized server and deliver them to mobile devices over a network.
    - Jumpbox: a jump server/jumpbox is a remote access system deployed to make accessing a specific system or network easier or more secure
        - often deployed in extranets, screened subnets, or cloud networks where a standard direct link or private channel is not available
    - Remote Desktop Service (RDS) such as RD, Teamviewer, VNC etc can provide in-office experience while remote
    - using cloud-based desktop solutions such as Amazon Workspaces, Amazon AppStream, V2 Cloud, and Microsoft Azure
    - security must be considered to provide protection for your private network against remote access complications:
        - stringent auth before granting access
        - grant permission only for specific need
        - remote comm protected via encryption
    - create a remote access security policy, addressing:
        - remote connectivity technology
        - transmission protection
        - authentication protection
        - remote user assistance
- Data communications
    - whether workers are physically in an office or working remotely, communication between devices should be encrypted to prevent any unauthorized device or person from openly reading the contents of packets as they are sent across a network
    - corporate networks can be segmented into multiple VLANs to separate different types of resources
    - communications should be encrypted using TLS or IPSec
- Virtualized networks
    - allow adopting of things like software-defined networks, VLANs, virtual switches, virtual SANs, guest operating systems, port isolation etc
    - many organizations are moving to the cloud, and not continuing to build out local or on-site server infrastructure
    - however, organizations still use hypervisors to virtualize servers and desktops for increased density and reliability
        - to host multiple servers on a single hypervisor, the Ethernet and storage networks must also be virtualized 
        - VMware vSphere and Microsoft Hyper-V both use virtual network and storage switches to allow communication between virtual machines and the physical network; guest operating systems running in the VMs use a synthetic network or storage adapter, which is relayed to the physical adapter on the host
        - software-defined networking on the hypervisor can control the VLANs, port isolation, bandwidth and other aspects just as if it was a physical port
- Third-party connectivity
    - any time an org’s network is connected directly to another entity’s network, their local threats and risks affect each other
        - **memorandum of understanding (MOU)** (MOU = letter of intent) or **memorandum of agreement (MOA)**: an expression of agreement or aligned intent, will, or purpose between two entities
        - **interconnection security agreement (ISA)**: a formal declaration of the security stance, risk, and technical requirements of a link between two organizations’ IT infrastructures
    - remote workers are another form of third-party connectivity
    - vendors (like IT auditing firms) may need to connect to your network, and attackers are routinely looking for creative ways to gain organizational access -- third-party connectivity is one option
    - as organizations evaluate third-party connectivity, they need to look carefully at the principle of least privilege and at methods of monitoring use and misuse


## Key Terms
- **Acknowledgment (ACK):** An acknowledgment of a signal being received.
- **Address Resolution Protocol (ARP):** Used at the Media Access Control (MAC) layer to provide for direct communication between two devices within the same LAN segment.
- **Advanced Persistent Threat (APT):** An adversary with sophisticated levels of expertise and significant resources who is able to use multiple different attack vectors (e.g. cyber, physical, and deception) to achieve its objectives. Its objectives are typically to establish and extend footholds within the IT infrastructure of organizations in order to continually exfiltrate information and/or to undermine or impede critical aspects of a mission, program or organization, or place itself in a position to do so in the future. Moreover, the APT pursues its objectives repeatedly over an extended period of time, adapting to a defender's efforts to resist it, and with determination to maintain the level of interaction needed to execute its objectives.
- **Application Programming Interface (API):** Mobile code mechanisms that provide ways for applications to share data, methods, or functions over a network. Usually implemented either in XML or JavaScript Object Notation (JSON). A reference to a software access point or library function with a well-defined syntax and well-defined functionality.
- **Bandwidth:** The amount of information transmitted over a period of time. A process consisting of learning or education could necessitate higher bandwidth than a quick status update, which would require a lower bandwidth.
- **Bit:** Most essential representation of data (zero or one) at layer 1 or the OSI 7-Layer Model.
- **Frame:** Data represented at layer 2 of the OSI 7-Layer Model.
- **Packet:** Representation of data at layer 3 of the OSI 7-Layer Model.
- **Segment (data):** Data representation (or datagram name) at Layer 4 of the OSI 7-Layer Model. 
- **Internet Protocol (IPv4):** The dominant protocol that operates at layer 3 of the OSI 7-Layer Model. IP is responsible for addressing packets so that they can be transmitted from the source to the destination hosts.
- **Bluetooth (Wireless Personal Area Network IEEE 802.15):** Bluetooth wireless technology is an open standard for short-range RF communication used primarily to establish wireless personal area networks (WPANs). It has been integrated into many types of business and consumer devices.
- **Bound Network(s):** Network in which devices are connected at layer 1 by means of physical cables, wires, or fiver. Often referred to as wired networks, Ethernet networks, or by wiring or cable standard used, (e.g. fiber network, Cat 5 or Cat 6 network). See also Unbound (wireless) Network(s).
- **Unbound (Wireless) Network(s):** Network in which physical layer interconnections are done using radio, light or other means not confined to wires, cables or fibers. Devices on unbound networks may or may not be mobile. See also Bound Network(s).
- **Boundary Routers:** Primarily advertise routes that external hosts can use to reach internal ones.
- **Bridges:** A device that creates a single aggregate network from separate network segments. Using the OSI model, this device aggregates networks at layer 2.
- **Carrier Sense Multiple Access with Collision Avoidance (CSMA/CA):** A method of flow control in a network. To prevent more than one station from accessing the network simultaneously, the sending station announces its intent to send, and other stations wait until the sending station announces its completion.
- **Carrier Sense Multiple Access with Collision Detection (CSMA/CD):** A method of flow control in a network. If more than one station accesses the network simultaneously, the other stations detect the event and subsequently attempt retransmission.
- **Cellular Network:** A radio network distributed over land areas called cells, each served by at least one fixed-location transceiver, known as a cell site or base station.
- **Circuit-Switched Network:** A network that establishes a dedicated circuit between endpoints.
- **Code-Division Multiple Access (CDMA):** Every call's data is encoded with a unique key, then the calls are all transmitted at once.
- **Concentrators:** Multiplex connected devices into one signal to be transmitted on a network.
- **Content Distribution Network (CDN):** A large, distributed system of servers deployed in multiple data centers, which moves content to achieve QoS and availability requirements.
- **Control Plane:** Control of network functionality and programmability is directly made to devices at this layer. OpenFlow was the original framework/protocol specified to interface with devices through southbound interfaces.
- **Converged Protocols:** A protocol that combines (or converges) standard protocols (such as TCP/IP) with proprietary or other non-standard protocols. These can sometimes provide greatly enhanced functionality and security to meet the needs of specific situations or industries. Adopting them can also complicate enterprise-wide security engineering efforts by requiring additional specialist knowledge and skills to manage and secure.
- **Domain Name Service (DNS):** This acronym can be applied to three interrelated elements: a service, a physical server, and a network protocol.
- **Driver (Device Driver):** Software layer that provides an interface for accessing the functions of hardware devices. Typically used by the OS.
- **Dynamic Host Configuration Protocol (DHCP):** An industry standard protocol used to dynamically assign IP addresses to network devices.
- **Registered Ports:** Ports 1024-49151. These ports typically accompany non-system applications associated with vendors and developers.
- **Dynamic or Private Ports:** Ports 49152-65535. Whenever a service is requested that is associated with well-known or registered ports, those services will respond with a dynamic port.
- **East-West Data Flow (or Traffic):** Network data traffic that flows laterally across a set of internal systems, networks or subnetworks within an IT architecture. These can be flows within a data center or between geographically disperse locations. Contrast with north-south data flows, in which northbound data is leaving the organization and southbound is entering it. Within SDNs, east-west data flow is within a data plane, control plane or application plane. North-south data flows, in SDN terms, is data flowing up and down the stack of data/control/application planes.
- **North-South Network Data Flow (or Traffic):** Data flowing either from the organization to external destinations (northbound) or into the organization from external sources (southbound). In SDN terms, data flowing up (northbound) or down (southbound) the stack of data/control/applications planes.
- **Fiber Distributed Data Interface (FDDI):** A LAN standard, defined by ANSI X3T9.5, specifying a 100Mbps token-passing network using fiber-optic cable, with transmission distances of up to two kilometers.
- **Fibre Channel over Ethernet (FCoE):** A lightweight encapsulation protocol that lacks the reliable data transport of the TCP layer.
- **File Transfer Protocol (FTP):** The Internet protocol (and program) used to transfer files between hosts.
- **Hypertext Transfer Protocol (HTTP):** A communication protocol used to connect to servers on the World Wide Web. Its primary function is to establish a connection with a web server and transmit HTML pages to the client browser. The protocol used to transport hypertext files across the Internet.
- **Firewalls:** Devices that enforce administrative security policies by filtering incoming traffic based on a set of rules.
- **Firmware:** Computer programs and data stored in hardware typically in read-only memory (ROM) or programmable read-only memory (PROM), such that the programs and data cannot be dynamically written or modified during execution of the programs.
- **Gateway Device:** A firewall or other device sitting at the edge of a network to regulate traffic and enforce rules.
- **Internet Control Message Protocol (ICMP):** An IP network protocol standardized by the IETF through RFC 792 to determine if a particular service or host is available.
- **Internet Group Management Protocol (IGMP):** Used to manage multicasting groups that are  a set of hosts anywhere on a network that are listening for a transmission.
- **Internet of Things (IoT):** A virtual network made up of small, dedicated-use devices that are typically designed as small form factor, embedded hardware with a limited functionality OS. They may interface with the physical world and tend to be pervasively deployed where they exist.
- **Internet Protocol (IPv6):** A modernization of IPv4 that includes a much larger address field: IPv6 addresses are 128 bits that support 2128 hosts.
- **Internetworking:** Two different sets of servers and communications elements using network protocol stacks to communicate with each other and coordinate their activities with each other.
- **Intrusion Detection System (IDS):** A security service that monitors and analyzes network or system events for the purpose of finding and providing real-time or near real-time warning of attempts to access system resources in an unauthorized manner.
- **Intrusion Prevention Systems (IPS):** Uses available information to determine if an attack is underway and sends alerts but also blocks the attack from reaching its intended target.
- **Kill Chain, Cyber Kill Chain:** A generalized attack model consisting of actions on the objective and six broad, overlapping sets of operational activities: reconnaissance, weaponization, delivery, exploitation, installation, command and control. APT actors often combine these operations in complex ways to achieve their goals; such attacks may span over many months. For defenders, the kill chain model highlights the temporary gain in security that can result by improved systems and organizational hardening across any or all of these areas.
- **Lightweight Directory Access Protocol (LDAP):** Authentication is specified as simple (basic), simple using SSL/TLS, or Simple Authentication and Security Layer (SASL).
- **Logical Link Control (LLC):** One of two sub-layers that together make up the data link layer-- layer 2 of the OSI 7-Layer Model.
- **Man-in-the-Middle (MITM):** A form of active attack in which the attacker inserts themselves into the physical or logical communications flow between two parties and masquerades to each as the other, falsifying or altering the data exchanged as the attacker chooses to. Also known as MITM. Man (machine)-in-the-browser (MITB) attacks focus on layer 7 vulnerabilities to masquerade as client to the server and as server to the client.
- **Media Access Control (MAC):** The 48-bit hex number assigned to all network cards. The first 24 bits are assigned to the card manufacturer with the remaining bits being a unique value (address) for that card.
- **Microsegmented Networks, Microsegmentation:** Part of a zero trust strategy that breaks LANs into very small, highly localized zones using firewalls or similar technologies. At the limit, this places a firewall at every connection point.
- **Modem:** Provides modulation and demodulation of binary data into analog signals for transmission through telephone, cable, fiber, or other signaling systems.
- **Multiprotocol Label Switching (MPLS):** A WAN protocol that operates at both layer 2 and layer 3 (OSI) and does label switching.
- **Network Function Virtualization (NFV):** Alternately referred to as virtual network function. The objective of NFV is to decouple functions, such as firewall management, intrusion detection, NAT and name service resolution , away from specific hardware implementation and move them into software solutions. NFV's focus is to optimize distinct network services.
- **Network Management:** Monitors network performance and identifies attacks and failures. Mechanisms include components that enable network administrators to monitor and restrict resource access.
- **Open Shortest Path First (OSPF):** An interior gateway routing protocol developed for IP networks based on the shortest path first or link-state algorithm.
- **OSI Layer 1:** Physical Layer
- **OSI Layer 2:** Data Link Layer
- **OSI Layer 3:** Network Layer
- **OSI Layer 4:** Transport Layer
- **OSI Layer 5:** Session Layer
- **OSI Layer 6:** Presentation Layer
- **OSI Layer 7:** Application Layer
- **Packet Loss:** Degradation of VoIP or other streaming data caused by lost packets. A technique called packet loss concealment (PLC) is used in VoIP communications to mask the effect of dropped packets.
- **Packet-Switched Networks:** Networks that do not use a dedicated connection between endpoints.
- **Point-to-Point Protocol (PPP):** Provides a standard method for transporting multiprotocol datagrams over point-to-point links.
- **Port Address Translation (PAT):** An extension to network address translation (NAT) to translate all addresses to one routable IP address and translate the source port number in the packet to a unique value.
- **Quality of Service (QoS):** Refers to the capability of a network to provide better service to selected network traffic over various technologies, including frame relay, ATM, Ethernet and 802.1 networks, SONET, and IP-routed networks that may use any or all of these underlying technologies.
- **Remote Procedure Call (RPC):** A protocol that enables one system to execute instructions on other hosts across a network infrastructure.
- **Root of Trust (RoT):** Hardware-based mechanisms that guarantee the integrity of the hardware prior to loading the OS of a computer.
- **Segment (network):** A portion of a larger network, usually isolated by firewalls or routers at either end from other portions of the network. See also Microsegmented Networks, Microsegmentation.
- **Simple Network Management Protocol (SNMP):** An IP protocol for collecting and organizing information about managed devices on IP networks. It can be used to determine the "health" of networking devices including routers, switches, servers, workstations, printers, and modem racks.
- **Smurf:** ICMP echo request sent to the network broadcast address of a spoofed victim causing all nodes to respond to the victim with an echo reply.
- **Software-Defined Networking (SDN):** Any of a broad range of techniques that enable network management, routing, forwarding, and control functions to be directed by software. This is generally done by abstracting the control and management planes from the data plane and its forwarding functions.
- **Software-Defined Wide Area Network (SD-WAN):** An extension of the SDN practices to connect to entities spread across the Internet to support WAN architecture especially related to cloud migration.
- **Teardrop Attack:** Exploits the reassembly of fragmented IP packets in the fragment offset field that indicates the starting position, or offset, of the data contained in a fragmented packet relative to the data of the original unfragmented packet.
- **Terminal Emulation Protocol (Telnet):** A command-line protocol designed to give command-line access from one host to another.
- **Transmission Control Protocol (TCP):** The major transport protocol in the Internet suite of protocols providing reliable, connection-oriented, full-duplex streams.
- **Transmission Control Protocol over Internet Protocol (TCP/IP):** The name of the IETF's four-layer networking model, and its protocol stack.
- **Transmission Control Protocol over Internet Protocol (TCP/IP) Model:** Internetworking protocol model created by the IETF, which specifies four layers of functionality: link layer (physical communications), Internet layer (network-to-network communication), transport layer (basic channels for connections and connectionless exchange of data between hosts) and application layer, where other protocols and user applications programs make use of network services.
- **Trusted Platform Module (TPM):** A tamper-resistant integrated circuit built into some computer motherboards that can perform cryptographic operations (including key generation) and protect small amounts of sensitive information, such as passwords and cryptographic keys.
- **Virtual Local Area Networks (VLANs):** Allow network administrators to use switches to create software-based LAN segments that can be defined based on factors other than physical location.
- **Voice over Internet Protocol (VoIP):** A set of technologies that enables voice to be sent over a packet network.
- **Web Application Firewall (WAF):** A software-based firewall, which monitors and filters exchanges between an applications program and a host. WAFs usually involve inspection and filtering of HTTP and HTTPS conversations.
- **Wi-Fi (Wireless LAN IEEE 803.11x):** Primarily associated with computer networking, Wi-Fi uses the IEEE 802.11x specification to create a wireless LAN either public or private.
- **WiMAX (Broadband Wireless Access IEEE 802.16):** A well-known example of wireless broadband. WiMAX can potentially deliver data rates of more than 30 Mbps.
- **Zero Trust Model / Architecture:** Replaces trust, but verify as security design principle by asserting that all activities attempted, by all users or entities, must be subject to control, authentication, authorization, and management at the most granular level possible. NIST and others have proposed zero trust architectures as guidance frameworks for organizations to use as the combine microsegmentation, access control, behavior modeling, and threat intelligence (among other techniques) in moving toward a zero trust implementation.

