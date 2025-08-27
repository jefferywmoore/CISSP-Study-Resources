# [Domain-4](#domain-4-communication-and-network-security) **Communication and Network Security**

Networking can be one of the more complex exam topics; if you have a networking background, you likely won’t find this domain difficult; if not, spend extra time in this section and consider diving deeper into topics that are fuzzy; domain 4 comprises ~13% of the exam

- **ACK**: an acknowledgement of a signal being received
- **Active-active**: a data resiliency architecture and a form of load balancing, that uses all available pathways or systems during normal operations; for instance, client workloads are distributed across two or more nodes in a cluster to keep data safe and available in the event of an unexpected component failure; active-active can use the full throughput capability of all devices during normal operations, but has reduced capacity in adverse conditions
- **Active-passive**: active-passive system is a form of load balancing that keeps some pathways or system in an unused dormant state during normal operations; can only handle throughput of a single device allowing the secondary device to remain ready (but not passing traffic) until needed; can maintain consistent capacity during abnormal conditions
- **ARP**: Address Resolution Protocol; used to resolve IP addresses into Media Access Control (MAC) addresses; provides for direct communication between two devices within the same LAN segment
- **ARP poisoning**: AKA ARP spoofing, where an attacker sends malicious ARP messages to a local network with the goal of associating the attacker’s MAC address with the IP address of another device (typically the default gateway or another trusted device) in the network; once successful, the attacker can intercept, modify, or block data intended for that IP address, facilitating attacks like man-in-the-middle (MITM), eavesdropping, or denial of service (DoS)
- **APT**: Advanced Persistent Threat is an agent/org that plans, organizes, and carries out highly sophisticated attacks against a target person, org, or industry over a period of time (months or even years); usually with a strategic goal in mind
- **API**: Application Programming Interface; code mechanisms that provide ways for apps to share data, methods, or functions over a network (usually implemented in XML or JavaScript Object Notation (JSON))
- **Automatic Private IP Addressing (APIPA)**: acts as a failover mechanism for DHCP servers and makes it easier to configure and support small LANs; primarily used in situations where a DHCP server is not available or is not responding; APIPA address range is 169.254.0.0–169.254.255.255, with the subnet mask of 255.255.0.0 (/16)
- **Bandwidth**: amount of information transmitted over a period of time; can be applied to moving bits over a medium, or human processes like learning or education
- **Baseband Communication**: refers to the transmission of a single signal over a medium using its original frequencies (without modulation), and the entire bandwidth of the medium is used to carry the signal; ethernet networks (like 10BASE-T) operate using baseband signaling, where the entire cable is dedicated to a single communication channel
- **Bluebugging**: a type of Bluetooth attack where an attacker exploits vulnerabilities in a device's Bluetooth connection to gain unauthorized access and control over it; the attacker can then use this access to listen to phone calls, read or send messages, steal data, or even manipulate the device’s settings, all without the victim's knowledge; to combat this attack, turn off Bluetooth when not in use, set to "non-discoverable", and use strong authentication
- **Bluejacking**: a relatively harmless Bluetooth-based attack where an attacker sends unsolicited messages to nearby Bluetooth-enabled devices, such as mobile phones, tablets, or laptops; it exploits the Bluetooth feature that allows devices to communicate over short distances (typically up to 10 meters) and works by pushing messages to any device with Bluetooth set to "discoverable" mode
- **Bluesnarfing**: Bluesnarfing is a Bluetooth-based attack where an attacker gains unauthorized access to data on a victim's Bluetooth-enabled device; unlike Bluejacking (which only sends unsolicited messages), bluesnarfing is a serious security threat because it involves stealing or retrieving sensitive data without the user's knowledge or consent
- **Bluesniffing**: Bluesniffing is a type of Bluetooth attack that involves eavesdropping on Bluetooth communications to intercept data being exchanged between devices; it’s a form of passive Bluetooth reconnaissance where the attacker attempts to listen in on Bluetooth signals to gather information, much like Wi-Fi sniffing attacks on wireless networks
- **Bound networks**: AKA wired/Ethernet networks, where devices are connected by physical cables
- **Boundary routers**: they advertise routes that external hosts can use to reach internal hosts
- **Broadband**: refers to the transmission of multiple signals over a single communication medium using different frequency ranges (via modulation); it allows simultaneous transmission of multiple channels or services; examples include cable tv and DSL internet services
- **Bridge**: device that aggregates separate network segments into a single network segment, operating at OSI layer 2
- **CAM Table Flooding**: attack where switches don't know where to send traffic; prevented by enabling switch port security
- **Captive portal**: an authentication mechanism that redirects a newly-connected client to a web-based portal access control page
- **Challenge-Handshake Authentication Protocol (CHAP)**: used by PPP servers to authenticate remote clients; performs authentication using a challenge-response dialogue that cannot be replayed; encrypts both username and password, and performs periodic session reauthentication to prevent replay attacks
- **CSMA/CA**: Carrier Sense Multiple Access with Collision Avoidance is a method of network flow control
- **CSMA/CD**: Carrier Sense Multiple Access with Collision Detection is a method of network flow control, where if > 1 station accesses the network at the same time, other stations detect and re-try their transmission
- **Circuit-switched network**: network that uses a dedicated circuit between endpoints
- **CDMA**: Code-Division Multiple Access: a method of encoding several sources of data so they can all be transmitted over a single RF carrier by one transmitter, or by using a single RF carrier frequency with multiple transmitters; the data from each call is encoded with a unique key, and calls are transmitted at once; wireless radio protocol used to provide 2G and 3G voice and data services; replaced by 4G / LTE
- **Collision Domain**: set of systems that can cause a collision if they transmitted at the same time; note that broadcast domain is the set of systems that can receive a broadcast from each other
- **Concentrator**: provides communication capability between many low-speed, usually asynchronous channels and one or more high-speed, usually synchronous channels; usually different speeds, codes, and protocols can be accommodated on the low-speed side; multiplexed into one signal
- **CDN**: Content Distribution Network is a large distributed system of servers deployed in multiple data centers, with a goal of Quality of Service (QoS) and availability requirements
- **Control plane**: part of a network that controls how data packets are forwarded — meaning how data is sent from one place to another; e.g. the process of creating a routing table is considered part of the control plane; control of network functionality and programmability is directly made to devices at this layer
- **Converged protocol**: combines/converges standard protocols (such as TCP/IP) with proprietary/non-standard ones; they can complicate enterprise-wide security engineering efforts requiring specialist knowledge
- **Dense Wavelength Division Multiplexing (DWDM)**: by enabling multiple data streams or channels to be simultaneously transmitted over a single optical fiber, DWDM increases capacity and efficiency of the network
- **DHCP**: Dynamic Host Configuration Protocol is an industry standard used to dynamically assign IP addresses to network devices
- **Disassociation attack**: AKA deauthentication attack, is a type of denial-of-service (DoS) attack targeting Wi-Fi networks; it exploits the management frames used in the Wi-Fi protocol to forcibly disconnect (disassociate) a user’s device from a wireless access point (AP); these attacks can cause disruptions in network availability and can be used as part of a larger attack, such as a man-in-the-middle (MITM) attack
- **Domain-based Message Authentication, Reporting, and Conformance (DMARC)**: an email authentication protocol that builds on SPF and DKIM to prevent email spoofing; DMARC allows domain owners to specify a policy for handling unauthenticated emails, such as quarantine or reject, and to receive reports on email authentication results; DMARC works by checking that the "From" address matches the domain in the SPF and DKIM checks (alignment)
- **DomainKeys Identified Mail (DKIM)**: an email authentication protocol that helps verify the authenticity of an email sender and ensure message integrity; DKIM works by attaching a digital signature to the email header, which is created using a private key known only to the sender's email server; the recipient’s email server uses the sender’s public key, stored in DNS records, to verify this signature; if the signature is valid, it confirms the email was sent from an authorized source and hasn't been altered in transit helping prevent email spoofing and phishing by allowing recipients to verify that emails truly come from trusted domains
- **DNS**: Domain Name Service is three interrelated elements: a service, a physical server, and a network protocol
- **DNS poisoning**: act of falsifying DNS info used by clients to reach a system; can be accomplished via a rogue DNS server, pharming, altering a hosts file, corrupting IP config, DNS query spoofing, and proxy falsification; examples:
  - HOSTS poisoning
  - authorized DNS server attack
  - caching DNS server attack
  - changing a DNS server address
  - DNS query spoofing
- **Domain hijacking**: or domain theft, is the malicious action of changing the registration of a domain name without the authorization of the owner
- **Extranet**: a private network similar to an intranet, but typically open to external parties, such as business partners, suppliers, key customers, etc; main purpose of an extranet is to allow users to exchange data and applications, and share information
- **Extensible Authentication Protocol (EAP)**: a framework that allows for various authentication methods to be used for secure network access, including wireless networks, by providing a standardized way to exchange authentication information between a client and an authentication server; it's not a specific authentication method itself, but a platform to support multiple methods like passwords, certificates, or smart cards depending on the chosen "EAP method"; EAP allows customized authentication security solutions
- **Email bombing**: AKA "mail-bombing" - when email itself is used as an attack mechanism by flooding a system with messages, causing a denial of service
- **Email security**: internet email is based on SMTP, POP3, and IMAP, and is inherently insecure; email can be secured, and the methods used must be addressed in a security policy; email security solutions include using S/MIME, PGP, DKIM, SPF, DMARC, STARTTLS, and Implicit SMTPS
- **EPP**: endpoint protection platform (EPP) is a variation of EDR; EPP focuses on four main security functions: predict, prevent, detect, and respond; EPP is the more active predict and prevent variation of the more passive EDR
- **Evil twin**: a type of Wi-Fi attack where a malicious actor sets up a fake wireless access point (AP) that mimics a legitimate one, with the goal of tricking users into connecting to the rogue access point, allowing the attacker to intercept, monitor, and manipulate the victim’s network traffic, potentially capturing sensitive data such as login credentials, financial info, and personal communications
- **FDDI**: Fiber Distributed Data Interface is an ANSI X3T9.5 LAN standard; 100 Mbps, token-passing using fiber-optic, up to 2 kilometers
- **FCoE**: Fibre Channel over Ethernet is a lightweight encapsulations protocol without the reliable data transport of TCP
- **Gateway device**: a firewall or other device that sits at the edge of the network to regulate traffic and enforce rules
- **Generic Routing Encapsulation (GRE)**: a protocol for encapsulating data packets that use one routing protocol inside the packets of another protocol; "encapsulating" means wrapping one data packet within another data packet, like putting a box inside another box; encapsulation is the addition of a header, possibly footer, to the data received by each layer from the layer above before handing it off to the layer below; the inverse action is de-encapsulation; note that when using IPv4, the GRE header is inserted between the delivery and payload headers
- **Host-based IDS (HIDS)**: monitor activity on a single system; one drawback of a HIDS is that attackers can discover and disable them (compare to NIDS)
- **Hypervisor**: aka virtual machine monitor/manager (VMM); the virtualization component that creates, manages, and operates VMs
- **Hypervisor Type I**: a native or bare-metal hypervisor; there is no host OS, the hypervisor installs directly onto the hardware instead of the host OS
- **Hypervisor Type II**: a hosted hypervisor; the hypervisor is installed as another app in the OS
- **ICMP**: Internet Control Message Protocol, standardized by IETF via RFC 792 to determine if a particular host is available
- **IGMP**: Internet Group Management Protocol, used to manage multicasting groups
- **Implicit SMTPS**: a method of securing email transmission by establishing a dedicated, encrypted connection using TLS (Transport Layer Security) from the start, typically over port 465; unlike STARTTLS, which begins as an unencrypted connection and then upgrades, Implicit SMTPS immediately initiates a secure connection, making it less vulnerable to interception or downgrade attacks
- **Internetworking**: two different sets of servers/communication elements using network protocol stacks to communicate and coordinate activities
- **International Telecommunication Union Telecommunication Standardization Sector (ITU-T)**: responsible for setting international standards for telecommunications and Information Communication Technology (ICT); standards include X.509, Y.3172 and Y.3173 (machine learning), H.264/MPEG-4 AVC (video compression), and ITU-T G.651.1 (multimode fiber)
**IV (Initialization Vector) attack**: occurs when attackers exploit weaknesses in how an IV is generated or used in cryptographic systems, particularly in stream ciphers and certain modes of block ciphers; the Initialization Vector (IV) is a random or pseudo-random value used to ensure that even if the same data is encrypted multiple times, the resulting ciphertext is different each time; if the IV is predictable, reused, or improperly managed, it can lead to security vulnerabilities, enabling attackers to decrypt data, tamper with messages, or perform replay attacks
- **Layer 2 Tunneling Protocol (L2TP)**: a VPN tunneling protocol used to establish secure connections over public networks by creating a virtual tunnel for data; L2TP itself does not provide encryption, so it is often paired with IPsec (L2TP/IPsec) to provide confidentiality, integrity, and authentication; it operates at Layer 2 (Data Link Layer) of the OSI model, encapsulating data for secure transmission, commonly used for remote access VPNs and site-to-site connections
- **LDAP**: lightweight directory access protocol uses simple (basic) authentication such as SSL/TLS, or SASL (Simple Authentication and Security Layer)
- **Load balancers**: used to spread or distribute network traffic load across several network links or devices, with the purpose of optimizing infrastructure utilization, minimize response time, maximize throughput, reduce overloading, and remove bottlenecks
- **MAC filtering**: a list of authorized wireless client interface MAC addresses used by a WAP to block access to all nonauthoried devices
- **Managed Detection and Response (MDR)**: a service that monitors an IT environment in real-time to detect and resolve threats; not limited to endpoints, MDR focuses on threat detection and mediation; often a combination and integration of numerous technologies, such as SIEM, network traffic analysis (NTA), EDR, and IDS
- **Microsegmentation**: part of a zero trust strategy that breaks or divides up an internal network into very small (sometimes as small as a single device or important server/end-point), highly localized zones; each zone is separated from others by internal segmentation firewalls (ISFWs), subnets, or VLANs; note that at the limit, this places a firewall at every connection point
- **MSSP**: managed security service provider (MSSP) provides centrally-controlled and managed XDR solutions; can be fully deployed on-premise, in the cloud, or hybrid; MSSP solutions can be overseen through a SOC which is itself local or remote; orgs working with an MSSP to provide EDR, MDR, EPP, or XDR leverages the experience and expertise of the MSSP's staff
- **Network Address Translation (NAT)**: NAT translates IP addresses without changing port information, via one-to-one (static NAT) or many-to-one (dynamic NAT); NAT protects the addressing scheme of a private network, allowing the use of private IP addresses, and enables multiple internal clients to obtain internet access through a few public IP addresses; NAT is supported by many security border devices, such as firewalls, routers, gateways, WAPs, and proxies; NAT is useful when specific devices need to be accessible from outside the network, like servers that host websites; also see PAT; The main difference between NAT and PAT is that PAT uses port numbers to map private IP addresses to a public IP address, while NAT does not
- **Network-based IDS (NIDS)**: a network based IDS can monitor activity on a network, and isn't necessarily visible to an attacker
- **Network container names**: network containers by OSI layer: 7,6,5: protocol data unit (PDU); layer 4: segment (TCP) or datagram (UDP); layer 3: packet; layer 2: frame; layer 1: bit
- **NFV**: Network Function Virtualization (AKA Virtual Network Function) goal is to decouple functions, such as firewall management, intrusion detection, NAT and name service resolution from specific hardware solutions, and make them virtual/software; the focus is to optimize distinct network services
- **Nonroutable IP addresses**: from RFC 1918; 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16

- **Northbound/Southbound interface**: A northbound interface lets a specific component communicate with a higher-level component in the same network; a southbound interface is the opposite — enabling a specific component to communicate with a lower-level component
- **Online Certificate Status Protocol(OCSP)**: a real-time method for verifying the status of an X.509 (e.g. SSL/TLS) digital certificate
- **Packet-Switched Network**: a network that doesn't use a dedicated connection between endpoints; packet switching occurs when the message or communication is broken up into small segments and sent across intermediary networks to the destination; within packet-switching systems are two types of communication paths (or virtual circuits): permanent virtual circuits (PVCs) and switched virtual circuits (SVCs)
- **Password Authentication Protocol (PAP)**: a password-based protocol that verifies users for Point-to-Point Protocol (PPP); PAP transmits usernames and passwords in cleartext
- **Peering**: a method for two or more networks to exchange data directly with each other without going through a third party; a cost-effective way for networks to connect and improve performance; peering can be public (e.g. connection through an internet exchange point) or private (e.g. colocation)
- **Phreaking**: type of attack using various types of tech to circumvent the telephone system to make long-distance calls, alter the phone service function, steal services, or cause service disruptions; a phreaker is the phreaking attacker
- **Ping of Death (ping-of-death)**: an attack that sends numerous oversized ping packets to the victim, causing a freeze, crash, or reboot
**Plain Old Telephone Service (POTS)**: refers to the traditional, analog voice telephone service that has been in use since the late 19th century; it operates over copper twisted-pair wires and provides basic telephone functions like voice calling and fax transmission; POTS uses circuit-switched technology, establishing a dedicated connection for the duration of a call; known for its reliability and simplicity, offering standard features such as dial tone, ring tone, and support for analog devices like modems and fax machines
- **PLC**: Packet Loss Concealment used in VoIP communications to mask the effect of dropped packets
- **Point-to-Point Protocol (PPP)**: an encapsulation protocol designed to support the transmission of IP traffic over dial-up or point-to-point links; a standard method for transporting multiprotocol datagrams over point-to-point links; original PPP options for authentication were PAP, CHAP, and EAP
**Point-to-Point Tunneling Protocol (PPTP)**: an outdated VPN protocol that creates a secure tunnel for data over IP networks, primarily for remote access; operates at Layer 2 (Data Link Layer) of the OSI model, PPTP encapsulates data within IP packets but provides only basic encryption, making it relatively fast but less secure by modern standards; due to its weaker security, PPTP has largely been replaced by more robust VPN protocols, such as L2TP/IPsec and OpenVPN
- **Ports**: associated with services on network architectures; 65,535 ports in total
- **Ports 0-1023**: associated with common services
- **Ports 1024-4951**: registered ports used with non-system applications associated with vendors and devs
- **Ports 49152-65535**: dynamic ports (AKA private or non-reserved ports) used as temporary ports, often in association when a service is requested via a well-known port
- **Port Address Translation (PAT)**: a type of NAT which allows multiple devices on a private network to use the same public IP address by assigning each device a unique port number; PAT is useful when multiple devices need internet access but there aren't many public IP addresses available; an extension of NAT translating all addresses to one routable IP address and translating the source port number in the packet to a unique value
- **Private Branch Exchange (PBX)**: a private telephone network used within an org or enterprise, allowing internal users to communicate with each other and share a certain number of external phone lines for making outgoing calls; a PBX system manages incoming and outgoing calls, offering features such as call routing, voicemail, call conferencing, extension dialing, and automated attendants; modern PBX systems can be hardware-based, software-based, or hosted in the cloud, and they often support both traditional analog lines and digital communication methods like VoIP (Voice over Internet Protocol); countermeasures to PBX fraud include many of the same controls you would employ to protect a network (e.g. logical or technical, administrative and physical controls)
- **Proximity device/reader**: proximity devices can be passive, field-powered, or transponder; when a device passes near a proximity reader, the reader is able to determine the identity and authorization status of the bearer
- **Public Switched Telephone Network (PSTN)**: the global network of interconnected voice-oriented public telephone systems; encompasses the world's circuit-switched telephone networks operated by national, regional, and local telephony operators; the PSTN enables landline telephony and is responsible for routing calls between different telephone networks, both domestically and internationally; uses a combination of copper wires, fiber optics, microwave transmission, and undersea cables to facilitate voice communication across vast distances
- **Race condition (RCE)**: AKA race hazard is the condition of an electronics, software, or other system where the system's substantive behavior is dependent on the sequence or timing of other uncontrollable events, leading to unexpected or inconsistent results
- **RPC**: Remote Procedure Call is a protocol that enables one system to execute instructions on other hosts across a network infrastructure
- **Root of Trust**: a source that can always be trusted within a cryptographic system; because cryptographic security is dependent on keys to encrypt and decrypt data and perform functions such as generating digital signatures and verifying signatures, RoT schemes generally include a hardened hardware module; a RoT guarantees the integrity of the hardware prior to loading the OS of a computer
- **Screened subnet**: AKA DMZ (or demilitarized zone) is a network security architecture that uses firewalls to create a barrier between the public internet and the internal network, allowing only controlled access to external-facing servers while protecting the internal network from potential attacks
- **Sender Policy Framework (SPF)**: an email authentication protocol that helps verify if an email claiming to come from a specific domain is sent by an authorized mail server; SPF works by allowing domain owners to publish a list of approved sending IP addresses in their DNS records; when an email is received, the recipient's server checks the SPF record to ensure the email was sent from an authorized IP; if the IP is listed, the email is more likely to be legitimate and if not, it may be flagged as spam or rejected, helping to prevent email spoofing and phishing
- **SIPS**: secure version of the Session Initialization Protocol for VoIP, adds TLS encryption to keep the session initialization process secure
- **Stateless Address Autoconfiguration (SLAAC)**: a method in IPv6 where devices automatically configure their IP addresses without relying on a DHCP server, using Router Advertisements (RAs) to obtain network prefixes and their own interface identifiers to create unique addresses
- **Smartcard**: credit card-sized IDs, badges, or security passes with a magnetic stripe, bar code, or integrated circuit chip, containing info about the authorized bearer; used for identification or auth purposes; smartcards can include microprocessors and cryptographic certificates
- **S/MIME**: provides the following cryptographic security services for electronic messaging applications:
        - Authentication
        - Message integrity
        - Non-repudiation of origin (using digital signatures)
        - Privacy
        - Data security (using encryption)
  - S/MIME specifies the MIME type application/pkcs7-mime (smime-type "enveloped-data") for data enveloping (encrypting) where the whole (prepared) MIME entity to be enveloped is encrypted and packed into an object which subsequently is inserted into an application/pkcs7-mime MIME entity
  - S/MIME is a standard for public key encryption, providing security services for digital messaging apps
  - S/MIME requires the use of a PKI in order to work properly
  - S/MIME is the emerging standard for secure email / encrypted messages
- **SNMP**: Simple Network Management Protocol, is a protocol for collecting and organizing info about managed devices on IP networks; it can be used to determine the health of devices such as routers, switches, servers, workstations, etc
- **Smurf attack**: ICMP echo request sent to the network broadcast address of a spoofed victim causing all nodes to respond to the victim with an echo reply; a smurf attack is a form of DoS employing an amplification network to send numerous response packets to the victim
- **SPML**: Service Provisioning Markup Language is XML-based and designed to allow platforms to generate and respond to provisioning requests; uses the concept of requesting authority, a provisioning service point, and a provisioning service target; requesting authorities issue SPML requests to a provisioning service point; provisioning service targets are often user accounts and are required to be allowed unique identification of the data in its implementation
- **STARTTLS**: an email protocol command that upgrades an existing, insecure connection to a secure, encrypted connection using TLS (Transport Layer Security); commonly used in SMTP (Simple Mail Transfer Protocol), as well as IMAP and POP3 for email retrieval; when STARTTLS is enabled, email servers negotiate encryption with each other, protecting the email content and credentials from interception during transmission
- **STRP**: Secure Real-time Transport Protocol is an extension of Real-time Transport Protocol (RTP) that features encryption, confidentiality, message authentication, and replay protection to audio and video traffic
- **Multi-tiered firewall**: tiers are not the number of firewalls but the number of zones protected by the firewall; 2-tier protects two zones
- **Network Polling**: a communication method used in network systems where a central controller or master device periodically checks, or "polls," each connected device (node) to determine if it has data to transmit or to monitor its status; method ensures orderly communication by controlling when devices can send data, preventing data collisions and efficiently managing network traffic
- **TCP ACK scan**: type of network discovery scan, attempting to simulate an already-opened network connection; sending an ACK packet, simulating a packet from the middle of an already established connection
- **Teardrop attack**: exploits reassembly of fragmented IP packets in the fragment offset field (indicating the start position or offset of data contained in a fragmented packet)
- **Terminal Emulation Protocol**: designed to provide access between hosts; allows a computer to act like a traditional terminal and send commands/receive output from a remote system via a graphical interface; examples include Telnet, SSH, and Kermit
- **Token Passing**: a network access method used to control which devices can transmit data at any given time; a special data packet called a "token" circulates among the connected devices (nodes), and only the device that holds the token is permitted to send data over the network
- **Tunneling**: the encapsulation of protocol-deliverable message within a second protocol; the second protocol often performs encryption to protect the message contents
- **Unbound (Wireless) Network**: network where the physical layer interconnections are done using radio, light, or some other means (not confined to wires, cables, or fibers); may or may not be mobile
- **VLAN hopping**: a method of attacking the network resources of a VLAN by sending packets to a port not usually accessible from an end system; the goal of this form of attack is to gain access to other VLANs on the same network

- **Virtual Routing and Forwarding (VRF)**: allows multiple routing tables to be used on the same device simultaneously, similar to the concept of a VLAN (which is layer 2), but operating at layer 3; because routing instances operate independently, VRF allows IP addresses to overlap without conflict which supports segmentation and permits flexibility for zero trust implementations
- **WAF**: Web Application Firewall is a software-based app that monitors and filters exchanges between applications and a host; usually inspect and filter conversations like HTTP/S
- **X.509**: an ITU standard defining the format of public key certificates; X.509 certificates are used in many Internet protocols, including TLS/SSL, which is the basis for HTTPS; they are also used in offline applications, like electronic signatures
- **XDR**: extended detection and response (XDR) components usually include EDR, MDR, and EPP elements; XDR is not solely focused on endpoints, often including NTA, NIDS, and NIPS functionality

## [4.1](#41-apply-secure-design-principles-in-network-architectures-osg-10-chpts-1112) Apply secure design principles in network architectures (OSG-10 Chpts 11,12)

- 4.1.1 Open System Interconnection (OSI) and Transmission Control Protocol/Internet Protocol (TCP/IP) models
  - **TCP/IP**: AKA DARPA or DOD model has four layers: Application (AKA Process), Transport (AKA Host-to-Host), Internet (AKA Internetworking), and Link (AKA Network Interface or Network Access)
  - **OSI**: Open Systems Interconnection (OSI) Reference Model developed by ISO (International Organization for Standardization) to establish a common communication structure or standard for all computer systems; it is an abstract framework
        - Communication between layers via **encapsulation** (at each layer, the previous layer's header and payload become the payload of the current layer) and **de-encapsulation** (inverse action occurring as data moves up layers)

    | Layer | OSI model layer | TCP/IP model | PDU | Devices | Protocols |
    |-----|---------------| -------------------|------------| ----------------|-----------|
    | 7     | Application     | Application |Data               | Application Firewall                                | HTTP/s, DNS, DHCP, FTP, LPD, S-HTTP, TPFT, Telnet, SSH, SMTP, POP3, PEM, IMAP, NTP, SNMP, TLS/SSL, GBP, SIP, S/MIME, X Window, NFS etc. |
    | 6     | Presentation    | Application |Data   |   | JPEG, ASCII, MIDI etc |
    | 5     | Session         | Application| Data               | Circuit Proxy Firewall | NetBIOS, RPC|
    | 4     | Transport       | Transport (host-to-host) | Segments (TCP) / Datagrams (UDP)         |                              | TCP (connection oriented), UDP (connectionless), TLS, BGP     |
    | 3     | Network         | Internet/IP | Packets            | Router, Multilayer Switch, Packet Filtering Firewall         | IPv4, IPv6, IPSec, OSPF, EIGRP, ICMP, IGMP, RIP, NAT                              |
    | 2     | Data Link       | Network Access (Link) | Frames             | Switch, Bridge, NIC, Wireless Access Point | MAC, ARP, Ethernet 802.3 (Wired), CDP, LLDP, HDLC, PPP, PPTP, DSL, L2TP, IEEE 802.11 (Wireless), SONET/SDH, VLANs, Auth protocols (PAP, CHAP, EAP) |
    | 1     | Physical        | Network Access (Link) | Bits               | Hubs, Repeaters, Concentrators                              | Electrical signal (copper wire), Light signal (optical fibre), Radio signal (air) |

    ### OSI layers in detail

    - Mnemonics:
      - from top: All People Seem To Need Delicious Pizza
      - from bottom: Please Do Not Throw Sausage Pizza Away
    - Application Layer (7)
      - Responsible for:
        - interfacing user applications, network services, or the operating system with the protocol stack
        - identifying and establishing availability of communication partners
        - determining resource availability
        - synchronizing communication
      - Uses data streams
    - Presentation Layer (6)
      - Responsible for transforming data into the format that any system following the OSI model can understand
        - JPEG, ASCII, MIDI etc are used at the presentation layer
        - Associated tasks:
          - data representation
          - character conversion
          - data compression
          - data encryption
      - Uses data streams
      - Protocols at layer 7 include:
        - **Session Initiation Protocol (SIP)**: signalling protocol used to init, maintain, modify, and terminate real-time communication session between IP devices; used to establish voice and video calls
        - Hypertext Transfer Protocol (HTTP)
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
      - Protocols at layer 5 include NetBIOS, and RPC
    - Transport Layer (4)
      - Responsible for managing the integrity of a connection and controlling the session; providing transparent data transport and end-to-end transmission control
      - Defines session rules like how much data each segment can contain, how to verify message integrity, and how to determine whether data has been lost
      - Protocols that operate at the Transport layer:
        - Transmission Control Protocol (TCP)
          - the major transport protocol in the internet suite of protocols providing reliable, connection-oriented, full-duplex streams
          - emphasizing: full-duplex, connection-oriented protocol
          - uses three-way handshake using following three steps: synchronize (SYN), synchronize-acknowledge (SYN-ACK), and acknowledge (ACK)
          - TCP header flags:
            - URG ACK PSH RST SYN FIN (mnemonic: Unskilled Attackers Pester Real Security Folks)
          - TCP Packet Header: 10 fields, 160 bits, including source port, destination port, sequence number, acknowledgement number, checksum etc
        - User Datagram Protocol (UDP)
          - connectionless protocol that provides fast, best-effort delivery of **datagrams** (self-container unit of data)
          - UDP Datagram Header: 4 fields, 64 bits, including source port, destination port, length of data, checksum
        - Transport Layer Security (TLS)
          - note: in the OSI model, TLS operates on four layers: Application, Presentation, Session, and Transport; in the TCP/IP model, it operates only on the Transport layer
        - BGP: Border Gateway Protocol - used to exchange routing and reachability information between routers (looking at available paths, picking the best)
        - Segmentation, sequencing, and error checking occur at the Transport layer
    - Network Layer (3)
      - Responsible for logical addressing, and providing routing or delivery guidance (but not necessarily verifying guaranteed delivery), manages error detection and traffic control
      - **Internet Control Message Protocol (ICMP)**: allows network devices to send error and control messages and provides Ping and Traceroute utilities
      - **Internet Group Management Protocol (IGMP)**: allows hosts and adjacent routers on IP networks to establish multicast group memberships
      - **routing protocols**: move routed protocol messages across a network
        - includes RIP, OSPF, IS-IS, IGRP, IGMP, and BGP
        - routing protocols are defined at the Network Layer and specify how routers communicate
        - routing protocols can be static or dynamic, and categorized as interior or exterior
        - **static routing protocol**: requires an admin to create/update routes on the router
        - **dynamic**: can discover routers and determine best route to a given destination; routing table is periodically updated
        - **distance-vector**: (interior) makes routing decisions based on distance (e.g. hop count), and vector (router egress interface); examples:
          - **Routing Information Protocol (RIP)**: a distance-vector protocol that uses hop count as its routing metric; prevents routing loops by limiting the number of hops allowed by a packet in a path between source to destination; outdated and less scalable than protocols like OSPF
          - Interior Gateway Routing Protocol (IGRP): note that IGRP is proprietary and outdated
          - Enhanced Interior Gateway Routing Protocol (EIGRP)
        - **link state**: (interior) uses router characteristics (e.g. speed, latency, error rates) to make next hop routing decisions; examples:
          - **Open Shortest Path First (OSPF)**: an interior gateway routing protocol developed for IP networks based on shortest path first or link-state algorithm; calculates the shortest route to a destination through a network based on an algorithm
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
      - **Media Access Control (MAC)**: a 6-byte (48-bit) binary address written in hex (hexidecimal notation); AKA hardware, physical, or NIC address
        - first 3b/24-bits: Organizationally Unique Identifier (OUI) which denotes manufacturer
        - last 3b/24-bits: unique to that interface
      - ARP, switches and bridges operate at layer 2
      - Bridges: connect two physical network segments together
      - Switches: layer 2 switches interconnect multiple devices, forwarding data to intended recipient based on MAC address
      - Logical Link Control (LLC) is one of two sublayers that make up the Data Link Layer; provides flow and error control, and interfaces to layer 3
      - Protocols:
        - 802.1x: used for authenticating network devices to a network (network access control)
        - ARP: Address Resolution Protocol - translates a (layer 3) IP address to a MAC address
        - L2F: Layer 2 Forwarding - (Cisco) layer 2 tunneling protocol used to establish VPN connections; doesn't provide encryption
        - L2TP: Layer 2 tunneling protocol - used to establish VPN connections
        - PPTP: Point-to-Point Tunneling Protocol - used for creating VPNs; does not include encryption/authentication and considered obsolete
        - PPP: Point-to-Point Protocol - encapsulates IP traffic so that it can be transmitted over analog connections and provides authentication, encryption, and compression; replaced SLIP; authentication protocols include Password Authentication Protocol (PAP), Challenge-Handshake Authentication protocol (CHAP), and Extensible Authentication Protocol (EAP)
        - RARP: Reverse Address Resolution Protocol - translates a MAC address to an IP address
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
      - Protocols:
        - 802.11: a family of protocols for wireless local area networks including 802.11a, b, g, n, ac, ax
    - Common TCP Ports

      | Port | Protocol |
        |-----|---------------|
        | 20,21    | FTP |
        | 22    | SSH |
        | 23    | Telnet |
        | 25    | SMTP |
        | 53    | DNS |
        | 80    | HTTP |
        | 110    | POP3 |
        | 137-139 | NETBIOS |
        | 143    | IMAP |
        | 389    | LDAP |
        | 443    | HTTPS |
        | 445    | AD, SMB |
        | 636    | Secure LDAP |
        | 1433    | MS SQL Server |
        | 3389    | RDP |

- 4.1.2 Internet Protocol (IP) version 4 and 6 (IPv6) (e.g., unicast, broadcast, multicast, anycast)
  - IP is part of the TCP/IP (Transmission Control Protocol/Internet Protocol) suite
    - TCP/IP is the name of IETF's four-layer networking model, and its protocol stack; the four layers are: link (physical), internet (network-to-network), transport (channels for connection/connectionless data exchange) and application (where apps make use of network services)
    - IP provides the foundation for other protocols to be able to communicate; IP itself is a connectionless protocol
    - IPv4: dominant protocol that operates at layer 3; IP is responsible for addressing packets, using 32-bit addresses
    - IPv6: modernization of IPv4, uses 128-bit (16-byte) addresses, supporting 2^128 total addresses; makes IPSec mandatory
    - TCP or UDP is used to communicate over IP
    - **IP Subnetting**: method used to divide a large network into smaller, manageable pieces, called subnets
      - IP addresses: like a street address that identifies a device on a network in two parts:
        - network: identifies the "neighborhood" or network of the device
        - host: specifies the device (or "house") in that neighborhood
      - subnet mask: tool to divide the IP address into its network and host parts; e.g. 192.168.1.15 with subnet mast of 255.255.255.0 tells us that 192.168.1 is the network, and 15 is the host or device part
    - **CIDR notation**: a compact way of representing IP addresses and their associated network masks
      - example: 192.168.1.0/24
        - consists of two parts:
          - IP address: 192.168.1.0 - the network or starting address
          - /24 - specifies how many bits of the IP address are used for the network part; here /24 means the first 24 bits (out of 32 for IPv4) are used for the network part, and the remaining bits are used for the host addresses in that network
        - /24 is the same as 255.255.255.0 (where again 24 bits represented by 255.255.255 define the network, and .0 defines the host range)
        - IP address range: 192.168.1.0/24 represents the network 192.168.1.0 and all IPs from 192.168.1.1 to 192.168.1.254; 2^8=256 IP address, but 254 are usable (excludes network and broadcast addresses)
      - other examples:
        - 10.0.0.0/16: where /16 means the first 16 bits are reserved for the network, leaving 16 bits for hosts; allows 2^16 or 65,536 IP addresses, with 65,534 usable addresses
        - 172.16.0.0/12: /12 means 12 bits are for the network, leaving 20 bits for hosts; providing 2^20 = 1,048,576 IP addresses
    - Network Classes: IPv4 class A network contains 16,777,216 addresses; class B contains 65,534; Class C contains 254

    - IPSec provides data authentication, integrity and confidentiality
      - specifically, IPsec provides encryption, access control, nonrepudiation, and message authentication using public key cryptography
  - **Anycast**: nearest or best; helpful when using CDN (content distribution network), which is about getting data as physically close to the user as possible; anycast will ensure that I'm connected to the source that will provide the best/fastest source
  - **Application Layer**: defines protocols for node-to-node application communication and provides services to the application software running on a computer
  - **Broadcast**: a one-to-all communication method where data is sent from one sender to all possible receivers within a network segment; in broadcasting, a single data packet is transmitted, and all devices on the network receive it, regardless of whether they need the information
  - **Internet Layer**: defines the protocols for logically transmitting packets over the network
  - **Logical address**: occurs when an address is assigned and used by software or a protocol rather than being provided/controlled by hardware
  - Network layer’s packet header includes the source and destination IP addresses
  - **Multicast**: is a one-to-many communication method where data is transmitted from one sender to multiple specific receivers who are part of a multicast group; unlike broadcast, multicast only targets devices that have expressed interest in receiving the data, making it more efficient by conserving bandwidth and reducing unnecessary network load; used for live video streaming, online gaming, and conferencing
  - **Network Access Layer**: defines the protocols and hardware required to deliver data across a physical network
  - **Unicast**: a one-to-one communication method where data is transmitted from a single sender to a single receiver; in unicast, each data packet is sent directly to a specific destination address, and is the most common form of internet communication, where data is exchanged between individual devices
  
  - **Transport Layer**: defines protocols for setting up the level of transmission service for applications; this layer is responsible for the reliable transmission of data and the error-free delivery of packets
  
- 4.1.3 Secure protocols (e.g., Internet Protocol Security (IPSec), Secure Shell (SSH), Secure Sockets Layer (SSL)/Transport Layer Security (TLS))
  - **Kerberos**: standards-based network authentication protocol, used in many products (most notably Microsoft Active Directory Domain Services or AD DS)
    - Kerberos is mostly used on LANs for organization-wide authentication, single sign-on (SSO) and authorization; Kerberos provides three primary functions: accounting, authentication, and auditing
  - SSL and TLS: data protection; used for protecting website transactions (e.g. banking, e-commerce)
    - SSL and TLS both offer data encryption, integrity and authentication
    - TLS has supplanted SSL (the original protocol, considered legacy/insecure)
    - TLS was initially introduced in 1999 but didn’t gain widespread use until years later
    - The original versions of TLS (1.0 and 1.1) are considered deprecated and organizations should be relying on TLS 1.2 or 1.3
    - The defacto standard for secure web traffic is HTTP over TLS, which relies on hybrid cryptography: using asymmetric cryptography to exchange an ephemeral session key, which is then used to carry on symmetric cryptography for the remainder of the session
  - **Secure File Transfer Protocol (SFTP)**: a version of FTP that includes encryption and is used for transferring files between two devices (often a client / server)
  - **Secure Shell (SSH)**: remote management protocol, which operates over TCP/IP
    - all communications are encrypted
    - primarily used by IT administrators to manage devices such as servers and network devices
  - **Internet Protocol Security (IPSec)**: an IETF standard suite of protocols that is used to connect nodes (e.g. computers or office locations) together
    - IPsec protocol standard provides a common framework for encrypting network traffic and is built into a number of common OSs
    - IPsec establishes a secure channel in either transport or tunnel mode
    - IPsec performs reauthentication of the client system throughout the connected session in order to detect session hijacking
    - IPsec uses two protocols: Authentication Header (AH) and Encapsulating Security Payload (ESP) -- see below
    - widely used in virtual private networks (VPNs)
    - IPSec provides encryption, authentication and data integrity
    - **transport mode**: only packet payload is encrypted for peer-to-peer communication
    - **tunnel mode**: the entire packet (including header) is encrypted for gateway-to-gateway communication
    - **security association (SA)**: represents a simplex communication connection/session, recording any config and status info
    - **authentication header (AH)**: provides authentication, integrity, and nonrepudiation; provides assurance of message integrity, authentication and access control, preventing replay attacks; does not provide encryption; like an official authentication stamp, but it's not encrypted so anyone can read it
    - **encapsulating security payload (ESP)**: provides encryption of the payload which provides confidentiality and integrity of packet content; works with tunnel or transport mode; provides limited authentication and preventing replay attacks (not to the degree of AH)
    - **Internet Security Association and Key Management Protocol (ISAKMP)**: an element of IKE used to organize and manage encryption keys generated/exchanged by OAKLEY and SKEME; a security association is the agreed-upon method of auth and encryption used by two entities; ISAKMP's use of security associations enables IPsec to support multiple simultaneous VPNs from each host; the Oakley protocol specifies a sequence of key exchanges and describes their services (such as identity protection and authentication); and SKEME specifies the actual method of key exchange
  - **Internet Key Exchange (IKE)**: a standard protocol used to set up a secure and authenticated communication channel between two parties via a virtual private network (VPN); the protocol ensures security for VPN negotiation, remote host and network access

- 4.1.4 Implications of multilayer protocols
  - TCP/IP is a multilayer protocol, and derives several associated benefits
    - this means that protocols can be encapsulated within others (e.g. HTTP is encapsulated within TCP, which is in turn encapsulated in IP, which is in Ethernet), and additional security protocols can also be encapsulated in this chain (e.g. TLS between HTTP and TCP, which is HTTPS)
    - note that VPNs use encapsulation to enclose (or tunnel) one protocol inside another
  - Multilayer benefits:
    - many different protocols can be used at higher layers
    - encryption can be incorporated (at various layers)
    - it provides flexibility and resiliency in complex networks
  - Multilayer disadvantages:
    - nothing stops an added layer from being covert
    - encapsulating can be used to bypass filters
    - logical network segments can be traversed

- 4.1.5 Converged protocols (e.g., Internet Small Computer Systems Interface (iSCSI), Voice over Internet Protocol (VoIP), InfiniBand over Ethernet, Compute Express Link)
  - **Converged protocols**: merged specialty or proprietary with standard protocols, such as those from the TCP/IP suite
    - converged protocols provide the ability to use existing TCP/IP supporting network infrastructure to host special or proprietary services without the need to deploy different hardware
  - Examples of converged protocols:
    - **Compute Express Link**: connects CPUs to other devices or memory across the network, as quickly as possible
    - **Fibre Channel over Ethernet (FCoE)**: operating at layer 2, Fibre Channel is a network data-storage solution (SAN or network-attached storage (NAS)) that allows for high-speed file transfers of (up to) 128 Gbps
      - FCoE can be used over existing network infrastructure
      - FCoE used to encapsulate Fibre Channel over Ethernet networks
      - with this technology, Fibre Channel operates as a Network layer (OSI layer 3) protocol, replacing IP as the payload of a standard Ethernet network
    - **InfiniBand over Ethernet**: provides Remote Direct Memory Access (RDMA), or access to memory remotely wherever it may be stored on the network as quickly as possible; useful in high-performance computing
    - **Internet Small Computer Systems Interface (iSCSI)**: operating at layer 3, iSCSI is a converged protocol, network storage standard based on IP, used to enable location-independent file storage, transmission, and retrieval over LAN, WAN, or public internet connections
    - **Multiprotocol Label Switching (MPLS)**: a WAN protocol that operates at both layer 2 and 3 and does label switching; MPLS is a high-throughput/high-performance network technology that directs data across a network based on short path labels rather than longer network addresses
    - **Storage Area Network (SAN)**: a secondary network (distinct from the primary network) used to consolidate/manage various storage devices into single network-accessible storage
    - **Voice over Internet Protocol (VoIP)**: a tunneling mechanism that encapsulates audio, video, and other data into IP packets to support voice calls and multimedia collab
      - VoIP is considered a converged protocol because it combines audio and video encapsulation technology (operating as application layer protocols) with the protocol stack of TCP/IP
      - SIPS and SRTP are used to secure VoIP
      - **Secure Real-Time Transport Protocol (SRTP)**: an extension profile of RTP (Real-Time Transport Protocol) which adds further security features, such as message authentication, confidentiality and replay protection mostly intended for VoIP communications
      - SIPS: see definition above
    Other converged protocols:
      - SDN (see definition above)
      - virtualization [in Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-2024+Objectives.md#34-understand-security-capabilities-of-information-systems-is-eg-memory-protection-trusted-platform-model-tpm-encryptiondecryption-osg-10-chpt-8)
      - SOA (see definition [in Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-2024+Objectives.md#35-assess-and-mitigate-the-vulnerabilities-of-security-architectures-designs-and-solution-elements-osg-10-chpts-6791620))
      - microservices (see definition [Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-2024+Objectives.md#35-assess-and-mitigate-the-vulnerabilities-of-security-architectures-designs-and-solution-elements-osg-10-chpts-6791620))
      - IaC (see definition [in Domain 8](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-8-2024+Objectives.md))
      - serverless architecture (see definition [in Domain 3](https://github.com/jefferywmoore/CISSP-Study-Resources/blob/main/CISSP-Domain-3-2024+Objectives.#35-assess-and-mitigate-the-vulnerabilities-of-security-architectures-designs-and-solution-elements-osg-10-chpts-6791620))

- 4.1.6 Transport architecture (e.g., topology, data/control/management plane, cut-through/store-and-forward)
  - Topology: how devices are interconnected (like bus, star, ring, tree, mesh)
  - Data plane: forwards packets based on the direction of the control plane (packet forwarding & switching); the "do-er", within a switch, the data plane is what are the components in the switch actually moving the data around; transfers packets across the network based on direction from the control plane; can use cut-through, or store-and-forward
  - Control plane: functionss and processes which determine paths (route calculation / determination, OSPF, BGP); the intelligence, determines the optimal path for data packets
  - Management plane: manages and monitors the network's operations; the overall intelligence/configuration of the network
  - Physical topology: the physical connections between devices, and how they are connected to the network; dictates how devices are physically linked and how thye communicate over these physical connections
  - Logical topology: defines how data actually flows within the network, regardless of its physical layout; e.g. in a star-shaped physical network, the logical topology might be a bus if all communications are being broadcast to all nodes
  - Cut-through: switch starts forwarding the packet as soon as it reads the destination address, without waiting for the entire packet to be received; reduces latency but does not allow for error checking of the entire packet
  - Store-and-forward: switch receives the entire packet, checks it for errors, and then forwards it to the destination; introduces more latency, but ensures that the packet is error-free before forwarding

- 4.1.7 Performance metrics (e.g., bandwidth, latency, jitter, throughput, signal-to-noise ratio)
  - **Bandwidth**: theorectical maximum amount of data that can be transmitted over a network or internet connection in a given amount of time
  - **Throughput**: the actual rate of data tranfser successfuly transmitted over a network in a given amount of time
  - **Signal-to-noise ratio (SNR)**: measure of the level of the desired signal to the level of background noise; a higher SNR allows for higher data rates
  - **Latency**: time it takes for a signal to travel from its source to its destination and back (round-trip time, usually measured in miliseconds)
  - **Jitter**: variation in time delay between data packets over a network, measured in miliseconds; inconsistency of latency over time; you want low-latency, low-jitter, high SNR, and high throughput on your network

- 4.1.8 Traffic flows (e.g. north-south, east-west)
  - Traffic patterns (in, through, and out of a datacenter) are crucial considerations when designing network architecture, because they affect the choice of network topologies, routing protocols, and security strategies
  - **North/South (north-south) traffic**: the flows of data in and out of the datacenter, between the datacenter and a customer; traffic between clients on the Internet and servers within the datacenter (northbound), or vice versa (southbound); in SDN terms, data flowing up (northbound) and down (southbound) the stack of data/control/application planes
  - **East/West (east-west) traffic**: the data flows within the datacenter itself, or between interconnected datacenters; network traffic that is within a data, control, or application plane; within a data center or between geo dispersed locations; the data flowing laterally between servers, storage systems, and applications within the datacenter or across datacenters

- 4.1.9 Physical segmentation (e.g. in-band, out-of-band, air-gapped)
  - **In-band management**: managing network devices through the same network that they are used to transmit user or application data; this is ultimately less secure, because there is no physical segmentation
  - **Out-of-band management**: managing network devices using a dedicated network that is separate from the main network; this is more secure
  - **Air-gapped**: extreme form of segmentation where one segment of the network is completely isolated from all others physically and logically; this is most secure, and is typically used for industrial control systems (ICS)
  - **Physical segmentation**: creating a separate physical network

- 4.1.10 Logical segmentation (e.g., virtual local area networks (VLANs), virtual private networks (VPNs), virtual routing and forwarding, virtual domain)s
  - **Virtual Local Area Networks (VLAN)**: allows a single physical network to be partitioned into multiple smaller logical netowrks; a virtual LAN is a hardware-imposed network segmentation created by switches that requires a routing function to support communication between different segments
  - **Virtual Private Network (VPN)**: creates a private network across public network infrastructure; used to connect remote users or separate branches of a business to the main office's network; a traditional remote access technology; VPNs are based on encrypted tunneling; they offer authentication and data protection as a point-to-point solution
    - most common VPN protocols: PPTP, L2TP, SSH, TLS, and IPsec
    - split tunnel: a VPN configuration that allows a VPN-connected client system (e.g. remote node) to access both the org network via the VPN and the internet directly at the same time
    - full tunnel: a VPN configuration in which all the client's traffic is sent to the org network over the VPN link, and any internet-bound traffic is routed out of the org network's proxy or firewall interface
  - **Virtual Routing & Forwarding (VRF)**: allows mutliple instances of a routing table to co-exist within the same router, at the same time; allowing one physical router to emulate multiple virtual routers
  - **Virtual domain**: ability to create multiple separate security domains within a single physical device (e.g. a firewall); allows multiple virtual firewall instances within a single device; provides creating logical segmentation at the virtual machine level

- 4.1.11 Micro-segmentation (e.g., network overlays/encapsulation; distributed firewalls, routers, intrusion detection system (IDS)/intrusion prevention system (IPS), zero trust)
  - **Micro-segmentation**: enhances security by minimizing the lateral movement of attackers within a network, effectively creating a segmented, or compartmentalized architecture where each segment may have its own security policies and controls
  - **Network overlays/encapsulation**: creation of a virtual network that is abstracted or 'overlaid' on top of the physical network; can be done via SDN
  - **Distributed firewalls**: rather than routing traffic through a central firewall, security policies are enforced at the virtual network interface level for each virtual machine (VM) or container; essentially distributing virtual firewall rules and building small virtual firewalls, allowing us to achieve micro-segmation
  - **Distrbuted routers**: similar to distributed firewalls, distributed routers operate at the workload-level to control the flow of traffic between segments
  - IDS/IPS: deployed strategically within the network to monitor and protect individual workloads or network segments rather than just at the perimeter
  - Zero Trust: you can achieve the 'trust nothing, verify everything' nature of ZT by using micro-segmentation; each micro-segment is treated as its own secure zone, and acccess to each zone is given only after the identity and context of the request have been thoroughly verified

- 4.1.12 Edge networks (e.g., ingress/egress, peering)
  - **Edge networks**: broader term where networks that are situated at the edge of a centralized network, closer to the end-users to reduce latecy; designed to deliver content and services with reduced latency and increased performance by being located geographically closer to the user; a CDN, where the goal is to get content as physically close to the user as possible, is an example of a edge network
  - **Ingress**: traffic entering a network; typically created by users accessing services hosted at the edge
  - **Egress**: traffic exiting a network; usually refers to data sent from services at the edge, back to users, or to another network
  - **Peering**: directly interconnecting separate networks for the purpose of exchanging traffic, instead of routing traffic through the Internet; many Internet service providers have peering arangements between providers

- 4.1.13 Wireless networks (e.g. Bluetooth, Wi-Fi, Zigbee, satellite)
  - **Narrowband**: refers to a communication channel or system that operates with a small bandwidth, meaning it uses a limited range of frequencies to transmit data; in contrast to broadband, which can carry large amounts of data over a wide frequency range, narrowband systems focus on efficient transmission of smaller amounts of data, often over long distances, by using lower data rates and narrower frequency bands
  - **Light Fidelity (Li-Fi)**: a form of wireless communication technology that relies on light to transmit data, with theorectical speeds up to 224Gbits/sec
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
      - WEP is weak from RC4 implementation flaws (short, static IV sent in cleartext, IV is part of encryption key, and no integrity protection)
    - **Wi-Fi Protected Access (WPA)**: a security standard for wireless network computing devices; developed by the Wi-Fi Alliance to provide better data encryption and user authentication than WEP, which was the original Wi-Fi security standard
      - **Temporal Key Integrity Protocol (TKIP)**: an encryption protocol that was part of the WPA protocol; TKIP was designed to replace the insecure WEP encryption protocol,TKIP is no longer considered secure and has been deprecated
    - **Wi-Fi Protected Access II (WPA2)**:
      - IEEE 802.11i WPA2 replaced WEP and WPA
      - Uses AES-CCMP (Counter Mode with Cipher Block Chaining Message Authentication Code Protocol)
      - WPA2 operates in two modes, personal and enterprise
        - personal mode or the Pre-Shared Key (PSK) relies on a shared passcode or key known to both the access point and the client device; typically used for home network security
        - enterprise mode uses the more advanced Extensible Authentication Protocol (EAP) and an authentication server and individual credentials for each user or device; enterprise mode is best suited to companies and businesses
    - **Wi-Fi Protected Access 3 (WPA3)**:
      - WPA3-ENT uses 192-bit AES CCMP encryption
      - WPA3-PER remains at 128-bit AES CCMP
      - WPA3 **simultaneous authentication of equals (SAE)**: improves on WPA2's PSK mode by allowing for secure authentication between clients and the wireless network without enterprise user accounts; SAE performs a zero-knowledge proof process known as **Dragonfly Key Exchange** (which is a derivative of Diffie-Hellman); SAE uses a preset password and the MAC addresses of the client and AP to perform authentication and session key exchange
    - 802.1X / EAP
      - IEEE 802.1X defines the use of encapsulated EAP to support a wide range of authentication options for LAN connections; the 802.1x standard is named "Port-Based Network Access Control"
      - 802.1X is a mechanism to proxy authentication from the local device to a different dedicated auth service within the network
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
    - **Site survey**: a formal assessment of wireless signal strength, quality, and interference using an RF signal detector
    - **Wi-Fi Protected Setup (WPS)**: intended to simplify the effort of setting up/adding new clients to a secured wireless network; operates by automatically connecting the first new wireless client to seek the network once WPS is triggered
      - WPS allows users to easily connect devices to a Wi-Fi network by:
        - pressing a physical WPS button on the router
        - entering an 8-digit PIN found on the router
        - using NFC or Push-Button Connect for quick device pairing
        - the 8-digit PIN method is vulnerable to attacks, particularly brute-force, due to the structure of the WPS protocol, since the PIN is validated in two halves; also many routers do not implement rate limiting allowing repeated PIN attempts without lock out
        - Best WPS protection is to turn it off
    - Lightweight Extensible Authentication Protocol (LEAP) is a Cisco proprietary alternative to TKIP for WPA
      - Avoid using LEAP, use EAP-TLS as an alternative; if LEAP must be used a complex password is recommended
    - **Protected Extensible Authentication Protocol (PEAP)**: a security protocol used to better secure WiFi networks; PEAP is protected EAP, and it comes with enhanced security protections by providing encryption for EAP methods, and can also provide authentication; PEAP encapsulates EAP within an encrypted TLS (Transport Layer Security) tunnel, thus encrypting any EAP traffic that is being sent across a network

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
    - Wireless antennas: when setting up a wireless network, the type of antenna used on both the wireless client (device trying to connect) and the base station (such as an access point or router) is important for optimizing signal strength and coverage; different antennas are used depending on the needs of the environment, and these antennas vary in terms of their directionality and range

        | **Antenna Type**          | **Directionality**       | **Range**                    | **Use Case**                                                |
        |---------------------------|--------------------------|------------------------------|-------------------------------------------------------------|
        | **Omnidirectional Pole**   | 360-degree (all around)   | Short to medium               | General-purpose Wi-Fi coverage in homes/offices             |
        | **Yagi Antenna**           | Highly directional        | Long                          | Long-distance links between buildings or to distant devices |
        | **Cantenna**               | Directional               | Medium to long (DIY solutions)| Extending Wi-Fi to a distant access point                   |
        | **Panel Antenna**          | Semi-directional          | Medium                        | Indoor/outdoor targeted coverage in one direction            |
        | **Parabolic Antenna**      | Extremely directional     | Very long                     | Point-to-point communication over miles                     |

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

- 4.1.14 Cellular networks (e.g., 4G, 5G)
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

- 4.1.15 Content Distribution Networks (CDN)
  - **Content Distribution Network (CDN)**: a collection of resource services deployed in numerous data centers across the internet in order to provide low latency, high performance, and high availability of the hosted content
    - CDNs provide multimedia performance quality through the concept of distributed data hosts, geographically distributed, closer to groups of customers
    - Provides geographic and logical load balancing; lower-latency and higher-quality throughput
  - Client-based CDN is often referred to as P2P (peer-to-peer)

- 4.1.16 Software defined networks (SDN), (e.g., application programming interface (API), Software-Defined Wide Area Network, network functions virtualization)
  - Software Defined Netowrks (SDN): provide abstraction from the underlying physical network to enable rapid reconfiguration with centralized control; allows you creation of multiple virtual networks on top of a single physical network; SDN is fundamental to cloud networks
    - an SDN is effectively network virtualization, separating the infrastructure layer (aka the data or forwarding plane) hardware and hardware-based settings, from the control layer - network services of data transmission management
    - in a traditional network, each network device will have it's own control plane and data plane built into it, so each switch is making its own decisions on where to move packets and moving those packets
    - in an SDN the control plane is centralized; you may still have multiple network devices on the network and still responsible for moving packets, but the control plane, the intelligence, is centralized making it much easier to configure/re-configure the network
      - **control plane**: functions and processes which determine paths; receives instructions and sends them to the network; uses protocols to decide where to send traffic
      - **data plane**: functions and processes that forward packets based on the direction of the control plane; includes rules that decide whether traffic will be forwarded
      - **application plane**: where applications run that use APIs to communicate with the SDN about needed resources
    - typically ABAC-based
    - an SDN solution provides the option to handle traffic routing using simpler network devices that accept instructions from the SDN controller
    - Allows org to mix/match hardware
  - **Virtual extensible local area network (VXLAN)**:
    - an encapsulation protocol that enables VLANs to be stretched across subnets and geographic distances
      - VXLANs allow network admins to use switches to create software-based LAN segments that can be defined based on factors other than physical location
    - VLANs are typically restricted to layer 2, but VXLAN tunnels layer 2 connections over a layer 3 network, stretching them across the underlying layer 2 network
    - Allows up to 16 million virtual networks (VLAN limit is 4096)
    - VXLAN can be used as a means to implement microsegmentation without limiting segments to local entities only
    - Defined in [RFC 7348](https://datatracker.ietf.org/doc/html/rfc7348)
    - Encapsulation:
      - the OSI model represents a protocol stack, or a layered collection of multiple protocols, and communication between protocol layers occurs via encapsulation and deencapsulation (defined above)
  - **Software-defined wide area network (SD-WAN/SDWAN)**: an evolution of SDN that can be used to manage the connectivity and control services between distant data centers, remote locations, and cloud services over WAN links; put another way, SDN-WAN is an extension of SDN practices to connect entities spread across the internet, supporing WAN architecture; espcially related to cloud migration
    - SDWANs are commonly used to manage multiple ISP, and other connectivity options for speed, reliability, and bandwidth design goals
  - **Software-defined Visibility (SDV)**: a framework to automate the processes of network monitoring and response; the goal is to enable the analysis of every packet and make deep intelligence-based decisions on forwarding, dropping, or otherwise responding to threats

- 4.1.17 Virtual Private Cloud (VPC)
  - **Virtual Private Cloud (VPC)**: provides a logically isolated and customizable portion of a public cloud provider's infrastructure to a customer; a private cloud environment that's hosted within a public cloud; VPCs allow orgs to create a virtual network that is isolated from other users of the public cloud

- 4.1.18 Monitoring and management (e.g., network observability, traffic flow/shaping, capacity management, fault detection and handling)
  - **Monitoring and management**: tools, practices, and processes aimed at ensuring the availability, performance, and reliability of computer networks, systems, and services; monitoring and management includes performance and security monitoring, configuration management, log management, alerting and notification, reporting and analytics etc.
  - **Network observability**: ability to gain insights into the functionality of the network
  - **Traffic flow/shaping**: means controlling the movement of packets within a network to optimize performance, prioritize critical traffic, and enforce policies; for instance prioriting protocols/traffic like VoIP
  - **Capacity management**: monitoring and planning network resources to ensure they meet current and future demand; this is becoming less important as more organizations move to the cloud (which provides resources on-demand)
  - **Fault-detection and handling**: appropriately handling issues by identifying and diagnosing problems using methods like automatic remediation, manual intervention, IR etc

## [4.2](#42-secure-network-components-osg-10-chpt-11) Secure network components (OSG-10 Chpt 11)

The components of a network make up the backbone of the logical infrastructure for an organization; these components are often critical to day-to-day operations, and an outage or security issue can be very costly

- 4.2.1 Operation of hardware (e.g. redundant power, warranty, support)
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

- 4.2.2 Transmission media (e.g., physical security of media, signal propagation quality)
  - Transmission Media: comes in many forms, not just cables
    - includes wireless, LiFi, Bluetooth, Zigbee, satellites
    - most common cause of network failure (i.e. violations of availability) are cable failures or misconfigurations
    - wired transmission media can typically be described in three categories: coaxial, Ethernet, fiber
    - coaxial is typically used with cable modem installations to provide connectivity to an ISP, and requires a modem to convert the analog signals to digital
    - ethernet can be used to describe many mediums, it is typically associated with Category 5/6 unshielded twisted-pair (UTP) or shielded twisted pair (STP), and can be plenum-rated
    - Key Points for Each Cable Type:
      - **STP (Shielded Twisted Pair)**: features shielding around the pairs of wires to reduce electromagnetic interference (EMI);commonly used in industrial settings or environments with high interference
      - **UTP (Unshielded Twisted Pair)**: the most commonly used cable type for Ethernet (Cat5e, Cat6, etc.); more susceptible to EMI than STP, but cheaper and easier to install
      - **10Base2 Coax (Thinnet)**: used to connect systems to backbond trunks of thicknet cabling (185m, 10Mbps); an older coaxial cable type used for Ethernet networks, now mostly obsolete; requires terminators at each end of the cable to prevent signal loss
      - **10Base5 Coax (Thicknet)**: can span 500 meters and provide up to 10Mbps; early Ethernet cabling standard, thick and heavy, now obsolete; provided long-distance connectivity but was difficult to install and maintain
      - **100BaseT (Fast Ethernet)**: supports speeds up to 100 Mbps, used in early LANs, and still used in some legacy systems
      - **1000BaseT (Gigabit Ethernet)**: uses UTP or STP cables (usually Cat5e or Cat6) for Gigabit Ethernet; widely deployed in modern office and home networks
      - **Fiber Optic**: uses light for data transmission, making it immune to EMI and capable of very high speeds and long distances; most often used in the datacenter for backend components; two main types: Single-mode (for long distances, e.g., up to 40 km) and Multimode (for shorter distances, e.g., up to 2 km); more expensive than copper-based cables but necessary for high-speed, long-distance communication

    | **Cabling Type**       | **Shielding**          | **Max Speed**          | **Max Distance**                  | **Cost**         | **Common Use**                               | **Installation Complexity**                 |
    |------------------------|------------------------|------------------------|-----------------------------------|-----------------|---------------------------------------------|--------------------------------------------|
    | **STP (Shielded Twisted Pair)** | Shielded (protects against interference) | 10 Mbps - 10 Gbps                | Up to 100 meters for higher speeds | Higher than UTP due to shielding | Industrial and high-interference environments | More complex, due to shielding              |
    | **UTP (Unshielded Twisted Pair)** | Unshielded (less interference protection) | 10 Mbps - 10 Gbps                | Up to 100 meters for higher speeds | Lower cost, very common             | Office LANs, home networks                 | Easy, lightweight, flexible to install     |
    | **10Base2 Coax (Thinnet)** | Shielded coaxial cable (RG-58)                | 10 Mbps                         | Up to 185 meters                    | Low cost, outdated                     | Early Ethernet networks, now obsolete      | Requires terminators, prone to signal loss |
    | **10Base5 Coax (Thicknet)** | Thick shielded coaxial cable                  | 10 Mbps                         | Up to 500 meters                    | High (older, now obsolete)             | Early backbone networks, now obsolete      | Difficult, stiff and heavy                 |
    | **100BaseT (Fast Ethernet)** | UTP or STP, depends on the version         | 100 Mbps                        | Up to 100 meters                    | Affordable                             | Office LANs, early Fast Ethernet networks  | Easy with UTP, more complex with STP       |
    | **1000BaseT (Gigabit Ethernet)** | UTP or STP                              | 1 Gbps                          | Up to 100 meters                    | Moderate                               | Modern LANs, gigabit-capable networks      | Same as above, UTP easier than STP         |
    | **Fiber Optic (Single-Mode/Multimode)** | No electrical interference (uses light)  | Up to 100 Gbps or more          | Single-mode: Up to 40 km; Multimode: Up to 2 km | Expensive equipment                    | Data centers, backbone connections         | More complex, fragile, specialized tools   |

    | **Category** | **Frequency Range** | **Max Data Rate**        | **Typical Application**                         | **Max Distance**          | **Description**                                                                 |
    |--------------|---------------------|--------------------------|-------------------------------------------------|---------------------------|---------------------------------------------------------------------------------|
    | **Cat 1**    | None (Analog)        | Analog signals only       | Analog voice communication (e.g., telephone lines) | Varies (typically short distances) | Used for telephone systems, not suitable for data transmission.                  |
    | **Cat 2**    | 1 MHz                | 4 Mbps                   | Early token ring networks, telephone systems    | 100 meters                  | Rarely used today; supports legacy networking protocols.                         |
    | **Cat 3**    | 16 MHz               | 10 Mbps                  | 10Base-T Ethernet, telephone systems            | 100 meters                  | Initially used for 10 Mbps Ethernet, now largely obsolete.                       |
    | **Cat 4**    | 20 MHz               | 16 Mbps                  | Token Ring networks                             | 100 meters                  | Designed for early 16 Mbps token ring networks; now obsolete.                    |
    | **Cat 5**    | 100 MHz              | 100 Mbps                 | Fast Ethernet (100Base-T)                       | 100 meters                  | Widely used for Fast Ethernet networks; no longer recommended for new installs.  |
    | **Cat 5e**   | 100 MHz              | 1 Gbps                   | Gigabit Ethernet                                | 100 meters                  | Enhanced Cat 5 with reduced crosstalk; standard for most Gigabit Ethernet today.  |
    | **Cat 6**    | 250 MHz              | 1 Gbps (up to 10 Gbps for short distances) | Gigabit Ethernet, 10GBase-T (short distances)   | 100 meters for 1 Gbps, 55 meters for 10 Gbps | More robust against interference; supports 10 Gbps at limited distances.         |
    | **Cat 6a**   | 500 MHz              | 10 Gbps                  | 10GBase-T Ethernet                              | 100 meters                  | Enhanced Cat 6; supports 10 Gbps at full 100-meter distances.                    |
    | **Cat 7**    | 600 MHz              | 10 Gbps                  | High-speed networking, data centers             | 100 meters                  | Shielded cables; supports higher frequencies with improved noise resistance.     |
    | **Cat 8**    | 2000 MHz (2 GHz)     | 25 Gbps to 40 Gbps       | Data centers, high-performance computing        | 30 meters                   | Designed for short-distance data center applications; shielded for minimal noise.|

- 4.2.3 Network Access Control (NAC) systems (e.g., physical, and virtual solutions)
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
  - Agentless NAC: no software is installed on the endpoint, instead, the NAC system performs security checks using existing network infrastructure, such as switches, routers, firewalls, and network protocols; it gathers information about the device passively or actively through scans, without requiring direct interaction with the endpoint
  - NAC posture assessment capability determines if a system is sufficiently secure and compliant to connect to the network; this is a form of risk-based access control

    | Feature                          | **Agent-Based NAC**                                           | **Agentless NAC**                                    |
    |-----------------------------------|---------------------------------------------------------------|------------------------------------------------------|
    | **Software Requirement**          | Requires agent installation on devices                        | No software installation required on devices         |
    | **Depth of Security Checks**      | Provides deep insight into device security posture (antivirus, OS, patches) | Provides basic information (device type, MAC, OS)    |
    | **Continuous Monitoring**         | Yes, can perform continuous monitoring after network access    | Typically performs one-time or periodic checks       |
    | **Device Compatibility**          | May not support unmanaged devices or IoT devices               | Works with all devices (IoT, printers, guest devices) |
    | **Deployment Complexity**         | More complex due to agent installation and management          | Easier to deploy, no software installation required  |
    | **Granular Control**              | Offers granular control over security policies                 | Limited control, focuses on basic compliance         |
    | **Remediation Capabilities**      | Can help remediate non-compliant devices (e.g., installing patches) | Limited or no remediation capabilities               |

  - Just as you need to control physical access to equipment and wiring, you need to use logical controls to protect a network; there are a variety of devices that provide this type of protection, including:
    - stateful and stateless firewalls can perform inspection of the network packets and use rules, signatures and patterns to determine whether the packet should be delivered
      - reasons for dropping a packet could include addresses that don’t exist on the network, ports or addresses that are blocked, or the content of the packet (e.g. malicious packets blocked by admin policy)
    - IDP devices, which monitor the network for unusual network traffic and MAC or IP address spoofing, and then either alert on or actively stop this type of traffic
    - proxy server information:
      - **proxy server**: used to mediate between clients and servers, most often in the context of providing clients on a private network with internet access, while protecting the identify of the client
      - **forward proxy**: usually used by clients to anonymize their traffic, improve privacy, and cache data; a forward proxy is configured on client-side devices to manage access to external resources
      - **reverse proxy**: usually positioned in front of servers to distribute incoming traffic, improve performance through load balancing, and enhance security by hiding the details of backend servers; reverse proxies are often deployed to a perimeter network; they proxy communication from the internet to an internal host, such as a web server
      - **transparent proxy**: operates without client configuration and intercepts traffic transparently, often for monitoring or content filtering purposes without altering the client’s perception of the connection
      - **nontransparent proxy**: requires explicit configuration on the client side and may modify traffic to enforce policies, such as restricting access or logging user activities

        | **Attribute**                | **Forward Proxy**                                  | **Reverse Proxy**                                   | **Transparent Proxy**                               | **Nontransparent Proxy**                             |
        |------------------------------|---------------------------------------------------|----------------------------------------------------|----------------------------------------------------|-----------------------------------------------------|
        | **Primary Function**          | Acts as an intermediary between client and internet | Acts as an intermediary between client and backend servers | Intercepts client requests without modifying them  | Requires explicit client configuration               |
        | **Client Awareness**          | Client is aware of proxy usage                    | Client is unaware of proxy usage                    | Client is unaware of proxy usage                    | Client is aware of proxy usage                       |
        | **Use Case**                  | Content filtering, privacy, and caching for users | Load balancing, security, and hiding server identity| Caching, content filtering without client configuration | Content filtering, security, and logging             |
        | **Configuration**             | Configured on client devices or network settings  | Configured on the server side                      | No configuration needed on the client side          | Requires configuration on the client side            |
        | **Visibility**                | Proxy IP address is visible to the target website | Proxy hides server IP address from the client       | Proxy operation is invisible to both client and server | Proxy server IP address is visible to the client     |
        | **Modification of Requests**  | Can modify or filter client requests              | Can modify server responses or requests from clients| Does not modify requests or responses               | Can modify or filter client requests                 |
        | **Security Benefits**         | Provides privacy by hiding client IP addresses    | Provides security by hiding server details, load balancing | Limited security, primarily used for convenience   | High security potential, especially for monitoring   |

- 4.2.4 Endpoint security (e.g., host-based)
  - **Endpoint security**: concept that encourages admins to install firewalls, malware scanners, and IDS on every host
    - each individual device must maintain local security whether or not its network or telecom channels also provide security
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

## [4.3](#43-implement-secure-communication-channels-according-to-design-osg-10-chpt-12) Implement secure communication channels according to design (OSG-10 Chpt 12)

- Protocols that provide security services for application-specific communication channels are called secure communication protocols
  - examples of secure communication protocols include: IPsec, Kerberos, SSH, Signal protocol, S-RPC, and TLS

- 4.3.1 Voice, video, and collaboration (e.g., conferencing, Zoom rooms)
  - **Voice over Internet Protocol (VoIP)**: set of technologies that enables voice to be sent over a packet network
  - As more orgs switch to VoIP, protocols like SIP become more common, and introducing additional management, either via dedicated voice VLANs, or by establishing quality of service (QoS) levels to ensure voice traffic priority
  - Web-based voice apps can be more difficult to manage, causing additional unplanned bandwidth consumption

- 4.3.2 Remote access (e.g., network administrative functions)
  - 4 main types of remote access:
    - **service specific**: gives users the ability to remotely connect to and manipulate or interact with a single service (e.g. email)
    - **remote-control**: grants a remote user the ability to fully control another system that is physically distant
    - **remote node operation**: AKA remote client connecting directly to a LAN
    - **screen scraping**: refers to 1) remote control, remote access, or remote desktop services or 2) technology that allows an automated tool to interact with a human interface
  - Remote access security management requires that security system designers address the hardware and software components of an implementation along with issues related to policy, tasks, and encryption
  - General telecommuting security concerns include:
    - Data Leakage: remote workers may use personal devices or unsecured networks, increasing the risk of data leakage or loss of sensitive information
    - Inadequate Data Encryption: if data isn't encrypted in transit (over the internet) and at rest (on devices), it can be intercepted or accessed by unauthorized parties
    - Unauthorized Data Sharing: sharing files through unapproved channels, such as personal email or cloud storage, which may not meet organizational security standards
    - User home network environment: insecure Wi-Fi networks, VPN misconfigurations, and inconsistent application of security policies and monitoring, increasing the risk of unauthorized access
    - Endpoint security risks: examples include unsecured personal devices, lack of patching and updates, and susceptibility to malware and ransomware
  - General telecomutting security mitigations:
    - Implement strong authentication
    - Use VPNs and secure connections
    - Enforce endpoint protection
    - Implement security awareness training
    - Strengthen remote monitoring and incident response
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

- 4.3.3 Data communications (e.g., backhaul networks, satellite)
  - Whether workers are physically in an office or working remotely, communication between devices should be encrypted to prevent any unauthorized device or person from openly reading the contents of packets as they are sent across a network
  - Corporate networks can be segmented into multiple VLANs to separate different types of resources
  - Communications should be encrypted using TLS or IPSec
  - **Backhaul network**: the segment linking smaller/local networks to a central hub or broader Internet; MPLS can be used with these scenarios as it supports QoS features; Metro Ethernet are also commonly used providing high bandwidth, scalability, and application flexibility
  - Very-small-aperture terminal (VSAT) enables remote terminals to to communicate with geostationary satellites, providing connectivity where traditional terrestrial communication is not available
  - Low Earth Orbit (LEO) satellites (e.g. Starlink) provide reduced latency and higher-speed connectivity compared to traditional geostationary satellites

- 4.3.4 Third-party connectivity (e.g., telecom providers, hardware support)
  - Any time an org’s network is connected directly to another entity’s network, their local threats and risks affect each other; most orgs don't need to interact directly, but for those that do, it's important to consider the risks and ramfications, including partnerships, cloud services, and remote workers
    - **memorandum of understanding (MOU)** or **memorandum of agreement (MOA)**: (Note: MOU = letter of intent) an expression of agreement or aligned intent, will, or purpose between two entities
    - **interconnection security agreement (ISA)**: an ISA is a formal declaration of the security stance, risk, and technical requirements of a link between two organizations’ IT infrastructures
  - Remote workers are another form of third-party connectivity
  - Vendors (like IT auditing firms) may need to connect to your network, and attackers are routinely looking for creative ways to gain organizational access -- third-party connectivity is one option
  - As organizations evaluate third-party connectivity, they need to look carefully at the principle of least privilege and at methods of monitoring use and misuse
