[Domain 4](#domain4-top) **Communication and Network Security**

Networking can be one of the more complex exam topics; if you have a networking background, you likely won’t find this domain difficult-- if not, spend extra time in this section and consider diving deeper into topics that are fuzzy

- **ACK**: an acknowledgement of a signal being received
- **Active-active, active-passive clustering**: a data resiliency architecture in which client workloads are distributed across two or more nodes in a cluster to keep data safe and available in the event of an unexpected component failure; active-active can use the full throughput capability of both devices; active-passive can only handle throughput of a single device allowing the secondary device to remain ready (but not passing traffic) until needed
- **ARP**: Address Resolution Protocol; used to resolve IP addresses into Media Access Control (MAC) addresses; provides for direct communication between two devices within the same LAN segment
- **ARP poisoning**: AKA ARP spoofing, where an attacker sends malicious ARP messages to a local network with the goal of associating the attacker’s MAC address with the IP address of another device (typically the default gateway or another trusted device) in the network; once successful, the attacker can intercept, modify, or block data intended for that IP address, facilitating attacks like man-in-the-middle (MITM), eavesdropping, or denial of service (DoS)
- **APT**: Advanced Persistent Threat is an agent/org that plans, organizes, and carries out highly sophisticated attacks against a target person, org, or industry over a period of time (months or even years); usually with a strategic goal in mind
- **API**: Application Programming Interface; code mechanisms that provide ways for apps to share data, emthods, or functions over a network (usually implemented in XML or JavaScript Object Notation (JSON))
- **Bandwidth**: amount of information transmitted over a period of time; can be applied to moving bits over a medium, or human processes like learning or education
- **Bound networks**: AKA wired/Ethernet networks, where devices are connected by physical cables
- **Boundary routers**: they advertise routes that external hosts can use to reach internal hosts
- **Bridge**: device that aggregates separate network segments into a single network segment, operating at OSI layer 2
**CAM Table Flooding**: attack where switches don't know where to send traffic; prevented by enabling switch port security
- **CHAP**: Challenge-Handshake Authentication Protocol, used by PPP servers to authenticate remote clients; encrypts both username and password, and performs periodic session reauthentication to prevent replay attacks
- **CSMA/CA**: Carrier Sense Multiple Access with Collission Avoidance is a method of network flow control
- **CSMA/CD**: Carrier Sense Multiple Access with Colliion Detection is a method of network flow control, where if > 1 station accesses the network at the same time, other stations detect and re-try their transmission
- **Circuit-switched network**: network that uses a dedicated circuit between endpoints
- **CDMA**: Code-Division Multiple Access: a method of encoding several sources of data so they can all be transmitted over a single RF carrier by one transmitter, or by using a single RF carrier frequency with multiple transmitters; the data from each call is encoded with a unique key, and calls are transmitted at once
- **Collision Domain**: set of systems that can cause a sollision if they transmitted at the same time; note that broadcast domain is the set of systems that can receive a breadcast from each other
- **Concentrator**: provides communication capability between many low-speed, usually asynchronous channels and one or more high-speed, usually synchronous channels. Usually different speeds, codes, and protocols can be accommodated on the low-speed side; multiplexed into one signal
- **CDN**: Content Distribution Network is a large distributed system of servers deploye in multiple data centers, with a goal of Quality of Service (QoS) and availability requirements
- **Control plane**: part of a network that controls how data packets are forwarded — meaning how data is sent from one place to another; e.g. the process of creating a routing table is considered part of the control plane; control of network functionality and programmability is directly made to devices at this layer
- **Northbound/Southbound interface**: A northbound interface lets a specific component communicate with a higher-level component in the same network; a southbound interface is the opposite — enabling a specific component to communicate with a lower-level component
- **East/West traffic**: network traffic that is within a data, control, or application plane; within a data center or between geo dispersed locations
- **North/South traffic**: in SDN terms, data flowing up (northbound) and down (southbound) the stack of data/control/application planes; data flowing from the organization to external distinations (northbound), or into the org from external sources (southbound)
- **Converged protocol**: combines/converges standard protcols (such as TCP/IP) with proprietary/non-standard ones; they can complicate enterprise-wide security engineering efforts requiring specialist knowledge
- **DNS**: Domain Name Service is three interrelated elements: a service, a physical server, and a network protocol
    - **DNS poisoning**: act of falsifying DNS info used by clients to reach a system; can be accomplished via a rogue DNS server, pharming, altering a hosts file, corrupting IP config, DNS query spoofing, and proxy falsification; examples:
        - HOSTS poisoning
        - authorized DNS server attack
        - caching DNS server attack
        - changing a DNS server address
        - DNS query spoofing
- **DHCP**: Dynamic Host Configuration Protocol is an industry standard used to dynamically assign IP addresses to network devices
- **Domain hijacking**: or domain theft, is the malicious action of changing the registration of a domain name without the authorization of the owner
- **FDDI**: Fiber Distributed Data Interface is an ANSI X3T9.5 LAN standard; 100Mbps, token-passing using fiber-optic, up to 2 kilometers
- **FCoE**: Fibre Channel over Ethernet is a lightweight encapulsation protocol without the reliable data transport of TCP
- **Gateway device**: a firewall or other device that sits at the edge of the network to regulate traffic and enforce rules
- **Generic Routing Encapsulation (GRE)**: a protocol for encapsulating data packets that use one routing protocol inside the packets of another protocol; "encapsulating" means wrapping one data packet within another data packet, like putting a box inside another box; encapsulation is the addition of a header, possibly footer, to the data received by each layer from the layer above before handing it off to the layer below; the inverse action is deencapsulation; note that when using IPv4, the GRE header is inserted between the delivery and payload headers
- **Hypervisor**: aka virtual machine monitor/manager (VMM); the virtualization component that creates, manages, and operates VMs
- **Hypervisor Type I**: a native or bare-metal hypervisor; there is no host OS, the hypervisor installs directly onto the hardware instead of the host OS
- **Hypervisor Type II**: a hosted hypervisor; the hypervisor is installed as another app in the OS
- **ICMP**: Internet Control Message Protocol, standardized by IETF via RFC 792 to determine if a particular host is available
- **IGMP**: Internet Group Management Protocol, used to manage multicasting groups
- **Internetworking**: two different sets of servers/communication elements using network protocol stacks to communicate and coordinate activities
- **LDAP**: lightweight directory access protocol uses simple (basic) authentication such as SSL/TLS, or SASL (Simple Authentication and Security Layer)
- **MAC filtering**: a list of authorized wireless client interface MAC addresses used by a WAP to block access to all nonauthoried devices
- **Microsegmentation**: part of a zero trust strategy that breaks or divides up an internal network into very small (sometimes as small as a single device or important server/end-point), highly localized zones; each zone is separated from others by internal segmentation firewalls (ISFWs), subnets, or VLANs; note that at the limit, this places a firewall at every connection point
- **Network container names**: network containers are OSI layers 7-5: protocol data unit (PDU); layer 4: segment (TCP) or datagram (UDP); layer 3: packet; layer 2: frame; layer 1: bits
- **NFV**: Network Function Virtualization (AKA Virtual Network Function) that seeks to decouple functions, such as firewall management, intrusion detection, NAT and name service resolution, from specific hardware solutions, and make them virtual/software; the focus is to optimize distinct network services
- **Nonroutable IP addresses**: from RFC 1918; 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16
- **PLC**: Packet Loss Concealment used in VoIP communications to mask the effect of dropped packets
- **Packet-Switched Network**: a network that doesn't use a dedicated connection between endpoints
- **Point-to-Point Protocol**: a standard method for transporting multiprotocol datagrams over point-to-point links
- **Ports 1024-4951**: registered ports used with non-system applications associated with vendors and devs
- **Ports 49152-65535**: dynamic ports (AKA private or non-reserved ports) used as temporary ports, often in association when a service is requested via a well-known port
- **Port Address Translation**: an extension of NAT (Network Address Translation) translating all addresses to one routable IP address and translate the source port number in the packet to a unique value
- **Proximity device/reader**: proximity devices can be passive, field-powered, or transponder; when a device passes near a proximity reader, the reader is able to determine the identity and authorization status of the bearer
- **Race condition (RCE)**: AKA race hazard is the condition of an electronics, software, or other system where the system's substantive behavior is dependent on the sequence or timing of other uncontrollable events, leading to unexpected or inconsistent results
- **RPC**: Remote Procedure Call is a protocol that enables one system to execute instructions on other hosts across a network infrastructure
- **Root of Trust**: a source that can always be trusted within a cryptographic system; because cryptographic security is dependent on keys to encrypt and decrypt data and perform functions such as generating digital signatures and verifying signatures, RoT schemes generally include a hardened hardware module; a RoT guarantees the integrity of the hardware prior to loading the OS of a computer
- **SIPS**: secure version of the Session Initialization Protocol for VoIP, adds TLS encryption to keep the session initialization process secure
- **Smartcard**: credit card-sized IDs, badges, or security passes with a magnetic stripe, bar code, or integrated circuit chip, containing info about the authorized bearer; used for identification or auth purposes
- **S/MIME**: provides the following cryptographic security services for electronic messaging applications:
        - Authentication
        - Message integrity
        - Non-repudiation of origin (using digital signatures)
        - Privacy
        - Data security (using encryption)
    - S/MIME specifies the MIME type application/pkcs7-mime (smime-type "enveloped-data") for data enveloping (encrypting) where the whole (prepared) MIME entity to be enveloped is encrypted and packed into an object which subsequently is inserted into an application/pkcs7-mime MIME entity
    - S/MIME is the emerging standard for secure email / encrypted messages
- **SNMP**: Simple Network Management Protocol, is a protocol for collecting and organizing info about managed devices on IP networks; it can be used to determine the health of devices such as routers, switches, servers, workstations, etc
- **Smurf attack**: ICMP echo request sent to the network broadcast address of a spoofed victim causing all nodes to respond to the victim with an echo reply
- **SPML**: Service Provisioning Markup Language is XML-based and designed to allow platforms to generate and respond to provisioning requests; uses the concept of requesting authority, a provisioning service point, and a provisioning service target; requesting authorities issue SPML requests to a provisioning service point; provisioning service targets are often user accounts and are required to be allowed unique identification of the data in its implementaion
- **STRP**: Secure Real-time Transport Protocol is an extension of Real-time Transport Protocol (RTP) that features encryption, confidentiality, message authentication, and replay protection to audio and video traffic
- **Multi-tiered firewall**: tiers are not the number of firewalls but the number of zones protected by the firewall; 2-tier protects two zones
- **Teardrop attack**: exploits reassembly of fragmented IP packets in the fragment offset field (indicating the start position or offset of data contained in a fragemented packet)
- **Terminal Emulation Protocol**: designed to provide access between hosts; allows a computer to act like a traditional terminal and send commands/receive output from a remote system via a graphical interface; examples include Telnet, SSH, and Kermit
- **Unbound (Wireless) Network**: network where the physical layer interconnections are done using radio, light, or some other means (not confined to wires, cables, or fibers); may or may not be mobile
- **VLAN hopping**: a method of attacking the network resources of a VLAN by sending packets to a port not usually accessible from an end system; the goal of this form of attack is to gain access to other VLANs on the same network
- **WAF**: Web Application Firewall is a software-based app that monitors and filters exchanges between applications and a host; usually inspect and filter conversations like HTTP/S

[4.1](#4.1) Assess and implement secure design principles in network architectures (OSG-9 Chpts 11,12)

- 4.1.1 Open System Interconnection (OSI) and Transmission Control Protocol/Internet Protocol (TCP/IP) models
    - **TCP/IP**: AKA DARPA or DOD model has four layers: Application (AKA Process), Transport (AKA Host-to-Host), Internet (AKA Internetworking), and Link (AKA Network Interface or Network Access) 
    - **OSI**: Open Systems Interconnection (OSI) Reference Model developed by ISO (International Organization for Standardization) to establish a common communication structure or standard for all computer systems; it is an abstract framework
        - Communication between layers via **encapsulation** (at each layer, the previous layer's header and payload become the payload of the current layer) and **deencapsulation** (inverse action occurring as data moves up layers)

    | Layer | OSI model layer | TCP/IP model | PDU | Devices | Protocols | 
    |-----|---------------| -------------------|------------| ----------------|-----------|
    | 7     | Application     | Application |Data               | L7 firewall                                | HTTP/s, DNS, DHCP, FTP, LPD, S-HTTP, TPFT, Telnet, SSH, SMTP, POP3, PEM, IMAP, NTP, SNMP, TLS/SSL, GBP, SIP, S/MIME, X Window, NFS etc. |
    | 6     | Presentation    | Application |Data   | L7 firewall  | JPEG, ASCII, MIDI etc
    | 5     | Session         | Application| Data               | L7 firewall                                | All the above                                                |
    | 4     | Transport       | Transport (host-to-host) | Segments           | L4 firewall                                | TCP (connection oriented), UDP (connectionless)     |
    | 3     | Network         | Internet/IP | Packets            | Router, Multilayer Switch, Router         | IPv4, IPv6, IPSec, OSPF, EIGRP; ICMP, RIP, NAT                              |
    | 2     | Data Link       | Network Access | Frames             | Switch, Bridge, NIC, Wireless Access Point | MAC, ARP, Ethernet 802.3 (Wired), CDP, LLDP, HDLC, PPP, DSL, L2TP, IEEE 802.11 (Wireless), SONET/SDH, VLANs |
    | 1     | Physical        | Network Access | Bits               | All the above                              | Electrical signal (copper wire), Light signal (optical fibre), Radio signal (air) |

    ### OSI layers in detail
    - Mnemonics:
        - from top: All People Seem To Need Delicious Pizza
        - from bottom: Please Do Not Throw Sausage Pizza Away
    - Application Layer (7)
        - Responsible for:
            - interfacing user applications, network services, or the operating system with the protocol stack 
            - identifying and establishing availability of communication partners 
            - determining resource availability and 
            - synchronizing communication
        - Uses data streams
    - Presentation Layer (6)
        - Responsible for transforming data into the format that any system following the OSI model can understand
        - JPEG, ASCII, MIDI etc are used at the presentation lay
        - Associated tasks:
            - data representation
            - character conversion
            - data compression
            - data encryption
         - Uses data streams
    - Session Layer (5)
        - Responsible for establishing, maintaining, and terminating communication sessions between two computers
        - Three communication session phases: 
            - connection establishment
                - **simplex**: one-way
                - **half-duplex**: both comm devices can transmit/receive, but not at the same time
                - **full-duplex**: both comm devices can transmit/receive at same time
            - data transfer
            - connection release
         - Uses data streams
    - Transport Layer (4)
        - Responsible for managing the integrity of a connection and controlling the session; providing transparent data transport and end-to-end transmission control
        - Defines session rules like how much data each segment can contain, how to verify message integrity, and how to determine whether data has been lost
        - Protocols that operate at the Transport layer:
            - Transmission Control Protocol (TCP)
                - the major transport protocol in the internet suite of protocols providing reliable, connection-oriented, full-duplex streams
                - emphasizing: full-duplex, connection-oriented protocol
                - uses three-way handshake: involves the following three steps: synchronize (SYN), synchronize-acknowledge (SYN-ACK), and acknowledge (ACK)
                - TCP header flags:
                    - URG ACK PSH RST SYN FIN (mnemonic: Unskilled Attackers Pester Real Security Folks)
            - User Datagram Protocol (UDP)
                - connectionless protocol that provides fast, best-effort delivery of **datagrams** (self-container unit of data)
            - Transport Layer Security (TLS)
                - note: in the OSI model, TLS operates on four layers: Application, Presentation, Session, and Transport; in the TCP/IP model, it operates only on the Transport layer
        - Segmentation, sequencing, and error checking occur at the Transport layer
        
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
                - **Open Shortest Path First (OSPF)**: an interior gateway routing protocol developed for IP networks based on shortest path first or link-state algorithm
                - Intermediate System to Intermediate System (IS-IS)
            - **path vector**: (exterior) a type of routing protocol used to determine the best path for data to travel across networks, particularly in scenarios involving multiple autonomous systems (AS); most commonly associated with **Border Gateway Protocol (BGP)**: the primary exterior routing protocol used on the internet
            - interior vs exterior:
                - interior routing protocols ("myopic") make next hop decisions based only on info related to the next immediate hop
                - exterior routing protocols ("far-sighted") make hop decisions based on the entire remaining path (i.e.) vector
            - [dive in further](https://community.cisco.com/t5/networking-knowledge-base/dynamic-routing-protocols-ospf-eigrp-ripv2-is-is-bgp/ta-p/4511577)
        - Routed protocols include Internetwork Package Exchange (IPX) and Internet Protocol (IP)  
    - Data Link Layer (2)
        - Responsible for formatting a packet for transmission
        - Adds the source and destination hardware addresses to the frame
        - **Media Access Control (MAC)**: a 6-byte (48-bit) binary address written in hex (hexidecimal notation); AKA hardware, physical, or NIC address; 
            - first 3b/24-bits: Organizationally Unique Identifier (OUI) which denotes manufacturer
            - last 3b/24-bits: unique to that interface
        - ARP, switches and bridges operates at layer 2
        - Logical Link Control (LLC) is one of two sublayers that make up the Data Link Layer

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
    - Common TCP Protocols
      | Port | Protocol | 
        |-----|---------------|
        | 20,21    | FTP | 
        | 22    | SSH | 
        | 23    | Telnet |
        | 25    | SMTP | 
        | 53    | DNS | 
        | 80    | HTTP | 
        | 110    | POP3 |
        | 143    | IMAP |
        | 389    | LDAP | 
        | 443    | HTTPS |
        | 445    | AD, SMB |
        | 636    | Secure LDAP |
        | 1433    | MS SQL Server |
        | 3389    | RDP |
        | 137-139 | NETBIOS |

- 4.1.2 Internet Protocol (IP) networking (e.g., Internet Protocol Security (IPSec), Internet Protocol (IP) v4/6)
     - IP is part of the TCP/IP (Transmission Control Protocol/Internet Protocol) suite
        - TCP/IP is the name of IETF's four-layer networking model, and its protocol stack; the four layers are link (physical), internet (network-to-network), transport (channels for connection/connectionless data exchange) and application (where apps make use of network services)
        - IP provides the foundation for other protocols to be able to communicate; IP itself is a connectionless protocol
        - IPv4: dominant protocol that operates at layer 3; IP is responsible for addressing packets, using 32-bit addresses
        - IPv6: modernization of IPv4, uses 128-bit addresses, supporting 2^128 total addresses
        - TCP or UDP is used to communicate over IP
        - **IP Subnetting**: method used to divide a large network into smaller, manageable pieces, called subnets
            - IP addresses: like a street address that identifies a device on a network in two parts:
                - network: identifies the "neighborhood" or network of the device
                - host: specifies the device (or "house") in that neighborhood
            - subnet masK: tool to divide the IP address into its network and host parts; e.g. 192.168.1.15 with subnet mast of 255.255.255.0 tells us that 192.168.1 is the network, and 15 is the host or device part
        - **CIDR notation**: a compact way of representing IP addresses and their associated network masks
            - example: 192.168.1.0/24
                - consists of two parts:
                    - IP address: 192.168.1.0 - the network or starting address
                    - /24 - specifies how many bits of the IP address are used for the network part; here /24 means the first 24 bits (out of 32 for IPv4) are used for the network part, and the remaining bits are used for the host addresses in that network
                - /24 is the same as 255.255.255.0 (where again 24 bits represented by 255.255.255 define the network, and .0 defines the host range)
                - IP address range: 192.168.1.0/24 represents the network 192.168.1.0 and all IPs from 192.168.1.1 to 192.168.1.254; 2^8=256 IP address, but 254 are usable (excludes network and broadcast addresses)
            - Other examples:
                - 10.0.0.0/16: where /16 means the first 16 bits are reserved for the network, leaving 16 bits for hosts; allows 2^16 or 65,536 IP addresses, with 65,534 usable addresses
                - 172.16.0.0/12: /12 means 12 bits are for the network, leaving 20 bits for hosts; providing 2^20 = 1,048,576 IP addresses

        - IPSec provides data authentication, integrity and confidentiality
            - specifically, IPsec provides encryption, access control, nonrepudiation, and message authentication using public key cryptography
    - **Logical address**: occurs when an address is assigned and used by software or a protocol rather than being provided/controlled by hardware
    - Network layer’s packet header includes the source and destination IP addresses
    - Network Access Layer: defines the protocols and hardware required to deliver data across a physical network
    - Internet Layer: defines the protocols for logically transmitting packets over the network
    - Transport Layer: defines protocols for setting up the level of transmission service for applications; this layer is responsible for the reliable transmission of data and the error-free delivery of packets
    - Application Layer: defines protocols for node-to-node application communication and provides services to the application software running on a computer

- 4.1.3 Secure protocols
    - **Kerberos**: standards-based network authentication protocol, used in many products (most notably Microsoft Active Directory Domain Services or AD DS)     
        - Kerberos is mostly used on LANs for organization-wide authentication, single sign-on (SSO) and authorization

    - SSL and TLS: data protection used for protecting website transactions (e.g. banking, ecommerce)
        - SSL and TLS both offer data encryption, integrity and authentication 
        - TLS has supplanted SSL (the original protocol, considered legacy/insecure) 
        - TLS was initially introduced in 1999 but didn’t gain widespread use until years later
        - The original versions of TLS (1.0 and 1.1) are considered deprecated and organizations should be relying on TLS 1.2 or TLS 1.3
        - The defacto standard for secure web traffic is HTTP over TLS, which relies on hybrid cryptography: using asymmetric cryptography to exchange an ephemeral session key, which is then used to carry on symmetric cryptography for the remainder of the session
    - **SFTP**: a version of FTP that includes encryption and is used for transferring files between two devices (often a client / server)
    - **SSH**: remote management protocol, which operates over TCP/IP
        - all communications are encrypted
        - primarily used by IT administrators to manage devices such as servers and network devices
    - **IPSec**: an IETF standard suite of protocols that is used to connect nodes (e.g. computers or office locations) together
        - IPsec protocol standard provides a common framework for encrypting network traffic and is built into a number of common OSs
        - IPsec establishes a secure channel in either transport or tunnel mode
        - IPsec uses two protocols: Authentication Header (AH) and Encapsulating Security Payload (ESP) -- see below 
        - widely used in virtual private networks (VPNs)
        - IPSec provides encryption, authentication and data integrity
        - **transport mode**: only packet payload is encrypted for peer-to-peer communication
        - **tunnel mode**: the entire packet (including header) is encrypted for gateway-to-gateway communication
        - **security association (SA)**: represents a simplex communication connection/session, recording any config and status info
        - **authentication header (AH)**: provides assurance of message integrity and nonrepudiation; also provides authentication and access control, preventing replay attacks; does not provide encryption; like an official authentication stamp, but it's not encrypted so anyone can read it
        - **encapsulating security payload (ESP)**: provides encryption of the payload which provides confidentiality and integrity of packet content; works with tunnel or transport mode; provides limited authentication and preventing replay attacks (not to the degree of AH)
    - **Internet Key Exchange (IKE)**: a standard protocol used to set up a secure and authenticated communication channel between two parties via a virtual private network (VPN); the protocol ensures security for VPN negotiation, remote host and network access

- 4.1.4 Implications of multilayer protocols
    - TCP/IP is a multilayer protocol, and derives several associated benefits
        - this means that protocols can be encapsulated within others (e.g. HTTP is encapsulated within TCP, which is in turn encapsulated in IP, which is in Ethernet), and additional security protocols can also be encapsulated in this chain (e.g. TLS between HTTP and TCP, which is HTTPS)
        - note that VPNs use encapsulation to enclose (or tunnel) one protocol inside another
    - Multilayer benefits:
        - many different protocols can be used at higher layers
        - encryption can be incorporated (at various layers)
        - it provides flexibility and resiliiency in complex networks
    Multilayer disadvantages:
        - nothing stops an added layer from being covert
        - encapsulating can be used to bypass filters
        - logical network segments can be traversed

- 4.1.5 Converged protocols (e.g., Fiber Channel Over Ethernet (FCoE), Internet Small Computer Sysetms Interface (iSCSI), Voice over Internet Protocol (VoIP))
    - **Converged protocols**: merged specialty or proprietary with standard protocols, such as those from the TCP/IP suite
        - converged protocols provide the ability to use existing TCP/IP supporting network infrastructure to host special or proprietary services without the need to deploy different hardware
    - Examples of converged protocols:
        - **Storage Area Network (SAN)**: a secondary network (distinct from the primary network) used to consolidate/manage various storage devices into single network-accessible storage
        - **Fibre Channel over Ethernet (FCoE)**: operating at layer 2, Fibre Channel is a network data-storage solution (SAN or network-attached storage (NAS)) that allows for high-speed file transfers of (up to) 128 Gbps
            - FCoE can be used over existing network infrastructure
            - FCoE used to encapsulate Fibre Channel over Ethernet networks
            - with this technology, Fibre Channel operates as a Network layer (OSI layer 3) protocol, replacing IP as the payload of a standard Ethernet network
        - **Internet Small Computer Sysetms Interface (iSCSI)**: operating at layer 3, iSCSI is a converged protocol, network storage standard based on IP, used to enable location-independent file storage, transmission, and retrieval over LAN, WAN, or public internet connections
        - **Multiprotocol Label Switching (MPLS)**: a WAN protocol that operates at both layer 2 and 3 and does label switching; MPLS is a high-throughput/high-performance network technology that directs data across a network based on short path labels rather than longer network addresses
        - **Voice over Internet Protocol (VoIP)**: a tunneling mechanism that encapsulates audio, video, and other data into IP packets to support voice calls and multimedia collab
            - VoIP is considered a converged protocol because it combines audio and video encapsulation technology (operating as application layer protocols) with the protocol stack of TCP/IP
            - SIPS and SRTP are used to secure VoIP
            - **Secure Real-Time Transport Protocol (SRTP)**: an extension profile of RTP (Real-Time Transport Protocol) which adds further security features, such as message authentication, confidentiality and replay protection mostly intended for VoIP communications
            - SIPS: see definition above
        Other converged protocols:
            - SDN (see definition above)
            - cloud
            - virtualization (see definition in [Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-Objectives.md))
            - SOA (see definition in [Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-Objectives.md))
            - microservices (see definition in [Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-Objectives.md))
            - IaC (see definition in [Domain 8](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-8-Objectives.md))
            - serverless architecture (see definition in [Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-Objectives.md))

- 4.1.6 Micro-segmentation (e.g., Software Defined Networks (SDN), Virtual eXtensible Local Area Network (VXLAN),Encapsulation, Software-Defined Wide Area Network (SD-WAN))
    - **Software-defined networks (SDN)**:
        - SDN is a broad range of techniques enabling network management, routing, forwarding, and control functions to be directed by software
        - SDN is effectively network virtualization, and separates the infrastructure layer (aka the data or forwarding plane) - hardware and hardware-based settings, from the control layer - network services of data transmission management
            - NOTE: 
                - **control plane**: receives instructions and sends them to the network; uses protocols to decide where to send traffic
                - **data plane**: includes rules that decide whether traffic will be forwarded
                - **application plane**: where applications run that use APIs to communicate with the SDN about needed resources
        - typically ABAC-based
        - an SDN solution provides the option to handle traffic routing using simpler network devices that accept instructions from the SDN controller
        - SDN offers a network design that is directly programmable from a central location, is flexible, vendor neutral, and based on open standards
        - Allows org to mix/match hardware
    - **Virtual extensible local area network (VXLAN)**:
        - an encapsulation protocol that enables VLANs to be stretched across subnets and geographic distances
            - VLANs allow network admins to use switches to create software-based LAN segments that can be defined based on factors other than physical location
        - VLANs are typically restricted to layer 2, but VXLAN tunnels layer 2 connections over a layer 3 network, stretching them across the underlying layer 2 network
        - Allows up to 16 million virtual networks (VLAN limit is 4096)
        - VXLAN can be used as a means to implement microsegmentation without limiting segments to local entities only
        - Defined in RFC 7348

    - Encapsulation:
        - the OSI model represents a protocol stack, or a layered collection of multiple protocols, and communication between protocol layers occurs via encapsulation and deencapsulation (defined above)

    - **Software-defined wide area network (SD-WAN/SDWAN)**: an evolution of SDN that can be used to manage the connectivity and control services between distant data centers, remote locations, and cloud services over WAN links; put another way, SDN-WAN is an extension of SDN practices to connect entities spread across the internet, supporing WAN architecture; espcially related to cloud migration
    - SDWANs are commonly used to manage multiple ISP, and other connectivity options for speed, reliability, and bandwidth design goals
    - **Software-defined Visibility (SDV)**: a framework to automate the processes of network monitoring and response; the goal is to enable the analysis of every packet and make deep intelligence-based decisions on forwarding, dropping, or otherwise responding to threats

- 4.1.7 Wireless networks (e.g. LiFi, Wi-Fi, Zigbee, satellite)
    - **Narrowband**: refers to a communication channel or system that operates with a small bandwidth, meaning it uses a limited range of frequencies to transmit data; in contrast to broadband, which can carry large amounts of data over a wide frequency range, narrowband systems focus on efficient transmission of smaller amounts of data, often over long distances, by using lower data rates and narrower frequency bands
    - **light fidelity (Li-Fi)**: a form of wireless communication technology that relies on light to transmit data, with theorectical speeds up to 224Gbits/sec
    - **Radio Frequency Identification (RFID)**: a technology used to identify and track objects or individuals using radio waves, with two main components: an RFID tag (or transponder) and an RFID reader; the tag contains a small microchip and an antenna, and the reader emits a signal that communicates with the tag to retrieve the stored information
        - Passive Tags don't have their own power source, relying instead on the energy from the RFID reader's signal to transmit data
        - Active Tags have a battery and can broadcast signals over longer distances
    - **Near Field Communicatio (NFC)**: a wireless communication technology that allows devices to exchange data over short distances, usually within a range of about 4 centimeters (1.5 inches); it operates on the same principle as RFID but is designed for closer proximity communication and is commonly used in mobile devices for tasks like contactless payments and data sharing; unlike RFID, where only the reader actively sends signals, NFC enables two-way communication
        - Active Mode: both devices generate their own radio frequency signals to communicate
        - Passive Mode: one device (like an NFC tag) is passive and only transmits data when powered by the active device's signal, similar to how passive RFID tags work
    - **Bluetooth**: wireless personal area network, IEEE 802.15; an open standard for short-range RF communication used primarily with wireless personal area networks (WPANs); secure guidelines: 
        - use Bluetooth only for non-confidential activities
        - change default PIN
        - turn off discovery mode
        - turn off Bluetooth when not in active use
    - **Wi-Fi**: Wireless LAN IEEE 802.11x; associated with computer networking, Wi-Fi uses 802.11x spec to create a public or private wireless LAN
        - **Wired Equivalent Privacy (WEP)**:
            - WEP is defined by the original IEEE 802.11 standard
            - WEP uses a predefined shared Rivest Cipher 4 (RC4) secret key for both authentication (SKA) and encryption
            - Shared key is static
            - WEP is weak from RC4 flaws 
        - Wi-Fi Protected Access II (WPA2):
            - IEEE 802.11i WPA2 replaced WEP and WPA
            - Uses AES-CCMP (Counter Mode with Cipher Block Chaining Message Authentication Code Protocol)
            - WPA2 operates in two modes, personal and enterprise 
                - personal mode or the Pre-Shared Key (PSK) relies on a shared passcode or key known to both the access point and the client device; typically used for home network security
                - enterprise mode uses the more advanced Extensible Authentication Protocol (EAP) and an authentication server and individual credentials for each user or device; enterprise mode is best suited to companies and businesses
        - Wi-Fi Protected Access 3 (WPA3):
            - WPA3-ENT uses 192-bit AES CCMP encryption
            - WPA3-PER remains at 128-bit AES CCMP
            - WPA3 **simultaneous authentication of equals (SAE)**: a mode improves on WPA2's PSK mode by allowing for secure authentication between clients and the wireless network without enterprise user accounts; SAE performs a zero-knowledge proof process known as **Dragonfly Key Exchange** (which is a derivative of Diffie-Hellman); SAE uses a preset password and the MAC addresses of the client and AP to perform authentication and session key exchange
        - 802.1X / EAP
            - WPA, WPA2, and WPA3 support the enterprise (ENT) authentication known as 802.1X/EAP (requires user accounts)
            - Extensible Authentication Protocol (EAP) is not a specific mechanism of authentication, rather an authentication framework
            - 802.1X/EAP is a standard port-based network access control that ensures that clients cannot communicate with a resource until proper authentication has taken place
            - Through the use of 802.1X Remote Authentication Dial-In User Service (RADIUS), Terminal Access Control Access Control System (TACACS), certificates, smartcards, token devices and biometrics can be integrated into wireless networks
            - Don’t forget about ports related to common AAA services:
                - UDP 1812 for RADIUS
                - TCP 49 for TACACS+
        - **Service Set Identifier (SSID)**: the name of a wireless network that is broadcast by a Wi-Fi router or access point, and used to uniquely identify a wireless network, so devices can recognize and connect to it; when you search for Wi-Fi networks on your phone or computer, the list of available networks you see consists of their SSIDs
            - **Extended Service Set Identifier (ESSID)**: the name of a wireless network (Wi-Fi network) that users see when they search for available networks, identifying the extended service set, which is essentially a group of one or more access points (APs) that form a wireless network; multiple APs in the same network can share the same ESSID, allowing seamless roaming for users within the network coverage area
            - **Basic Service Set Identifier (BSSID)**: a unique identifier for each AP in a Wi-Fi network; it’s the MAC address of the individual wireless access point or router within the network; while multiple APs in a network can share the same ESSID, each AP will have its own unique BSSID to distinguish it from other APs
        - **Site survey**: a formal assessment of wireles signal strnegth, quality, and interference using an RF signal detector
        - **Wi-Fi Protected Setup (WPS)**: intended to simplify the effort of setting up/adding new clients to a secured wireless network; operates by automatically connecting the first new wireless client to seek the network once WPS is triggered
            - WPS allows users to easily connect devices to a Wi-Fi network by:
                - pressing a physical WPS button on the router
                - entering an 8-digit PIN found on the router
                - using NFC or Push-Button Connect for quick device pairing
                - the 8-digit PIN method is vulnerable to attacks, particularly brute-force, due to the structure of the WPS protocol, since the PIN is validated in two halves; also many routers do not implement rate limiting allowing repeated PIN attempts without lock out
            - Best WPS protection is to turn it off
        - Lightweight Extensible Authentication Protocol (LEAP) is a Cisco proprietary alternative to TKIP for WPA
            - Avoid using LEAP, use EAP-TLS as an alternative; if LEAP must be used a complex password is recommended
        - Protected Extensible Authentication Protocol (PEAP): a security protocol used to better secure WiFi networks; PEAP is protected EAP, and it comes with enhanced security protections by providing encryption for EAP methods, and can also provide autentication; PEAP encapsulates EAP within an encrypted TLS (Transport Layer Security) tunnel, thus encrypting any EAP traffic that is being sent across a network
        
        
        - EAP Methods

        | Method | Type | Auth | Creds | When to Use |
        |--------|------------|-------|-----|---------------|
        | EAP-MD5  | Non-Tunnel | Challenge/response with hashing | Passwords for client auth | Avoid |
        | EAP-MSCHAP | Non-Tunnel | Challenge/response with hashing| Passwords for client auth | Avoid |
        | EAP-TLS | Non-Tunnel | Challenge/response with public key cryptography| Digital certificates for client/server auth | To support digitial certs as client/server creds |
        | EAP-GTC | Non-Tunnel | Cleartext pass | Passwords/OTP for client auth | Only use inside PEAP or EAP-FAST |
        | PEAP | Tunnel | Challenge/response with public key cryptography | Digital certificates for server auth | Digital certs as server creds, and TLS secure channel for inner EAP methods |
        | EAP-FAST | Tunnel | Challenge/response with symmetric cryptography (PAC) | DS, PAC for auth, other inside EAP tunnel | To support digital certs as server creds, and TLS secure channel for inner EAP; to support EAP chaining |

        - Speed and frequency table:
            
        | Amendment | Wi-Fi Alliance | Speed | Frequency |
        |-----|---------------| -------------------|------------|
        | 802.11  |   --   | 2 Mbps |2.4 GHz               |
        | 802.11a | Wi-Fi 2    | 54 Mbps |5 GHz              |
        | 802.11b | Wi-Fi 1    | 11 Mbps |2.4 GHz              |
        | 802.11g | Wi-Fi 3    | 54 Mbps |2.4 GHz              |
        | 802.11n | Wi-Fi 4    | 200+ Mbps |2.4,5 GHz            |
        | 802.11ac| Wi-Fi 5    | 1 Gbps |5 GHz               |
        | 802.11ax| Wi-Fi 6/Wi-Fi 6E     | 9.5 Gbps |2.4,5,6 GHz   |
        | 802.11be| Wi-Fi 7 | 46 Gbps | 2.4,5,6 GHz |

    - Modes:
        - Ad hoc: directly connects two clients
        - Standalone: connects clients using a WAP, but not to wired resources
        - Infrastructure: connects endpoints to a central network, not to each other
        - Wired extension: uses a wireless access point to link wireless clients to a wired network
    - **Zigbee**: IoT equipment communications concept based on Bluetooth
        - Low power/low throughput
        - Requires close proximity
        - Encrypted using 128-bit symmetric algorithm
        - Zigbee uses AES to protect network traffic, providing integrity and confidentiality controls
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

- 4.1.8 Cellular networks (e.g. 4G, 5G)

    - A cellular network or a wireless network is the primary communications technology used by many mobile devices
    - Cells are primary transceiver (cell site/tower)
    - Generally encrypted between mobile device and transmission tower; plaintext over wire; use encryption like TLS/VPN
    - 4G
        - 4G allows for mobile devices to achieve 100 Mbps, and stationary devices can reach 1 Gbps
        - LTE and WiMAX are common transmission systems
        - **WiMAX**: Broadband Wireless Access IEEE 802.16 is a well-known example of wireless broadband; WiMAX can potentially deliver data rates of > 30 Mbps
    - 5G
        - 5G uses higher frequencies than previous tech, allowing for higher transmission speeds up to 10 Gbps, but at reduced distances
        - Orgs need to enforce security requirements on 5G
        - 5G advantages over 4G
            - enhanced subscriber identity protection
            - mutual authentication capabilities
    - Security issues with wireless:
        - provider network (voice or data) is not necessarily secure
        - your cell phone can be intercepted
        - provider's towers can be simulated to conduct man-in-the-middle/on-path attack
        - using cell connectivity to access the internet or your office network creates a potential bridge, provider attackers with another avenue

- 4.1.9 Content Distribution Networks (CDN)

    - **Content Distribution Network (CDN)**: a collection of resource services deployed in numerous data centers across the internet in order to provide low latency, high performance, and high availability of the hosted content
        - CDNs provide multimedia performance quality through the concept of distributed data hosts, geographically distributed, closer to groups of customers
        - Provides geographic and logical load balancing; lower-latency and higher-quality throughput
    - Client-based CDN is often referred to as P2P (peer-to-peer)

[4.2](#4.2) Secure network components (OSG-9 Chpt 11)

The components of a network make up the backbone of the logical infrastructure for an organization; these components are often critical to day-to-day operations, and an outage or security issue can be very costly

- 4.2.1 Operation of hardware (e.g. redundant, power, warranty, support)
    - Modems provide modulation/demodulation of binary data into analog signals for transmission; modems are a type of Channel Service Unit/Data Service Unit (CSU/DSU) typically used for converting analog signals into digital;  the CSU handles communication to the provider network, the DSU handles communication with the internal digital equipment (in most cases, a router)
        - modems typically operate at Layer 2 
        - routers operate at Layer 3, and make the connection from a modem available to multiple devices in a network, including switches, access points and endpoint devices 
        - switches are typically connected to a router to enable multiple devices to use the connection
        - switches help provide internal connectivity, as well as create separate broadcast domains when configured with VLANs 
        - switches typically operate at Layer 2 of the OSI model, but many switches can operate at both Layer 2 and Layer 3
        - access points can be configured in the network topology to provide wireless access using one of the protocols and encryption algorithms
    
    - Redundant power: most home equipment use a single power supply, if that supply fails, the device loses power
        - redundant power is typically used with components such as servers, routers, and firewalls
        - redundant power is usually paired with other types of redundancies to provide high availability

- 4.2.2 Transmission media
    - Transmission Media: comes in many forms, not just cables
        - includes wireless, LiFi, Bluetooth, Zigbee, satellites
        - most common cause of network failure (i.e. violations of availability) are cable failures or misconfigurations
        - wired transmission media can typically be described in three categories: coaxial, Ethernet, fiber
        - coaxial is typically used with cable modem installations to provide connectivity to an ISP, and requires a modem to convert the analog signals to digital
            - fairly resistent to EMI
            - longer lengths than twisted pair
            - requires segment terminators
            - two main types:
                - **thinnet (10Base2)**: used to connect systems to backbond trunks of thicknet cabling (185m, 10Mbps)
                - **thicknet (10Base5)**: can span 500 meters and provide up to 10Mbps
        - ethernet can be used to describe many mediums, it is typically associated with Category 5/6 unshielded twisted-pair (UTP) or shielded twisted pair (STP), and can be plenum-rated
        - fiber typically comes in two options: single-mode or multi-mode
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

- 4.2.3 Network Access Control (NAC) devices

    - **Network Access Control (NAC)**: the concept of controlling access to an environment through strict adherence to and enforcement of security policy
    - NAC is meant to be an automated detection and response system that can react in real time, ensuring all monitored systems are patched/updated and have current security configurations, as well as keep unauthorized devices out of the network
    - NAC goals:
        - prevent/reduce known attacks directly (and zero-day indirectly)
        - enforce security policy throughout the network
        - use identities to perform access control
    - NAC can be implemented with a preadmission or postadmission philosophy:
        - **preadmission philosohpy**: requires a system to meet all current security requirements (such as patch application and malware scanner updates) before it is allowed to communicate with the network
        - **postadmission philosophy**: allows and denies access based on user activity, which is based on a predefined authorization matrix
    - Agent-based NAC:
        - installed on each management system, checks config files regularly, and can quarantine for non-compliance
        - dissolvable: usually written in a web/mobile language and is executed on each local machine when the specific management web page is accessed (such as captive portal)
        - permanent: installed on the monitored system as a persistent background service
    - NAC posture assessment capability determines if a system is sufficiently suecre and complaint to conntect to the network; this is a form of risk-based access control
    - Just as you need to control physical access to equipment and wiring, you need to use logical controls to protect a network; there are a variety of devices that provide this type of protection, including:
        - stateful and stateless firewalls can perform inspection of the network packets and use rules, signatures and patterns to determine whether the packet should be delivered
            - reasons for dropping a packet could include addresses that don’t exist on the network, ports or addresses that are blocked, or the content of the packet (e.g malicious packets blocked by admin policy)
        - IDP devices, which monitor the network for unusual network traffic and MAC or IP address spoofing, and then either alert on or actively stop this type of traffic
        - proxy/reverse proxies: 
            - proxy servers can be used to proxy internet-bound traffic, instead of letting clients talk directly
            - reverse proxies are often deployed to a perimeter network; they proxy communication from the internet to an internal host, such as a web server
            - like a firewall, a reverse proxy can use rules and policies to block certain types of communication
- 4.2.4 Endpoint security
    - **Endpoint security**: each individual device must maintain local security
        - any weakness in a network, whether border, server, or client-based presents a risk to all elements of the org
        - client/Server model is distributed architecture, meaning that security must be addressed everywhere instead of at a single centralized host
        - processing, storage on clients and servers, network links, communication equipment all must be secured
        - clients must be subjected to policies that impose safeguards on their content and users’ activities including:
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

[4.3](#4.3) Implement secure communication channels according to design ((OSG-9 Chpt 12))
- Protocols that provide security services for application-specific communication channels are called secure communication protocols
    - examples of secure communication protocols include: IPsec, Kerberos, SSH, Signal protocol, S-RPC, and TLS 
- 4.3.1 Voice
    - **Voice over Internet Protocol (VoIP)**: set of technologies that enables voice to be sent over a packet network
    - As more orgs switch to VoIP, protocols like SIP become more common, and introducing additional management, either via dedicated voice VLANs, or by establishing quality of service (QoS) levels to ensure voice traffic priority
    - Web-based voice apps can be more difficult to manage, causing additional unplanned bandwidth consumption
- 4.3.2 Multimedia collaboration
    - There are a variety of new technologies that allow instant organizational collaboration, including smartboards, and products that enhance on-site, hybrid, or virutal meetings
    - Mobile communication apps are a huge market, and will continue to grow, increasing the complexity of mobile security
- 4.3.3 Remote access
    - 4 main types of remote access:
        - **service specific**: gives users the ability to remotely connect to and manipulate or interact with a single service (e.g. email)
        - **remote-control**: grants a remote user the ability to fully control another system that is physically distant
        - **remote node operation**: AKA remote client connecting directly to a LAN
        - **screen scraping**: refers to 1) remote control, remote access, or remote desktop services or 2) technology that allows an automated tool to interact with a human interface
    - VPN (virtual private network) is a traditional remote access technology
        - most common VPN protocols: PPTP, L2F, L2TP, and IPsec
    - WAP (wireless access point) - local env treats as remote access
    - **VDI (virtual desktop infrastructure)**: means of reducing the security risks and performance requirements of end devices by hosting desktop/workstation VMs on servers that are remotely accessible by users
    - **VMI (virtual mobile interface)**: virtual mobile device OS is hosted on a central server
    - **Jumpbox**: a jump server/jumpbox is a remote access system deployed to make accessing a specific system or network easier or more secure; often deployed in extranets, screened subnets, or cloud networks where a standard direct link or private channel is not available
    - RDS (Remote Desktop Service) such as RD, Teamviewer, VNC etc can provide in-office experience while remote
    - Using cloud-based desktop solutions such as Amazon Workspaces, Amazon AppStream, V2 Cloud, and Microsoft Azure
    - Security must be considered to provide protection for your private network against remote access complications:
        - stringent auth before granting access
        - grant permission only for specific need
        - remote comm protected via encryption
    - Create a remote access security policy, addressing:
        - remote connectivity technology
        - transmission protection
        - authentication protection
        - remote user assistance
- 4.3.4 Data communications   
    - Whether workers are physically in an office or working remotely, communication between devices should be encrypted to prevent any unauthorized device or person from openly reading the contents of packets as they are sent across a network
    - Corporate networks can be segmented into multiple VLANs to separate different types of resources
    - Communications should be encrypted using TLS or IPSec
- 4.3.5 Virtualized networks
    - **Virtualized network**: is the combination of hardware and software networking components into a single integrated solution; allows for software control over network functions such as management, traffic shaping, address assignment etc
    - Allows for adoptiong of things like software-defined networks (SDNs), VLANs, virtual switches, virtual SANs, guest OSs, port isolation etc
    - Many orgs are moving to the cloud, and not continuing to build out local or on-site server infrastructure
        - however, organizations still use hypervisors to virtualize servers and desktops for increased density and reliability
            - to host multiple servers on a single hypervisor, the Ethernet and storage networks must also be virtualized 
            - VMware vSphere and Microsoft Hyper-V both use virtual network and storage switches to allow communication between virtual machines and the physical network; guest OSs running in the VMs use a synthetic network or storage adapter, which is relayed to the physical adapter on the host
            - SDN on the hypervisor can control the VLANs, port isolation, bandwidth and other aspects just as if it was a physical port
- 4.3.6 Third-party connectivity
    - Any time an org’s network is connected directly to another entity’s network, their local threats and risks affect each other
        - **memorandum of understanding (MOU)** or **memorandum of agreement (MOA)**: (Note: MOU = letter of intent) an expression of agreement or aligned intent, will, or purpose between two entities
        - **interconnection security agreement (ISA)**: a formal declaration of the security stance, risk, and technical requirements of a link between two organizations’ IT infrastructures
    - Remote workers are another form of third-party connectivity
    - Vendors (like IT auditing firms) may need to connect to your network, and attackers are routinely looking for creative ways to gain organizational access -- third-party connectivity is one option
    - As organizations evaluate third-party connectivity, they need to look carefully at the principle of least privilege and at methods of monitoring use and misuse