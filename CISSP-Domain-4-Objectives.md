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
        - EDR/MDR should be considered

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
    - VPN: virtual private network is a traditional remote access technology
    - WAP (local env treats as remote access)
    - VDI(virtual desktop infrastructure) / VMI (virtual mobile interface)
    - jumpbox: a jump server/jumpbox is a remote access system deployed to make accessing a specific system or network easier or more secure
        - often deployed in extranets, screened subnets, or cloud networks where a standard direct link or private channel is not available
    - RDS (Remote Desktop Service) such as RD, Teamviewer, VNC etc can provide in-office experience while remote
    - using cloud-based desktop solutions such as Amazon Workspaces, Amazon AppStream, V2 Cloud, and Microsoft Azure
    - security must be considered to provide protection for your private network against remote access complications:
        - stringent auth before granting access
        - grant permission only for specific need
        - remote comm protected via encryption
    - create a remote access security policy, addressing:
        - remote connectivity technology
        - transmission protectio
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

