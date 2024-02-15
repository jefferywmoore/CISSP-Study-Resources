[Domain 7](#domain7-top) **Security Operations**

[7.1](#7.1) Understand and comply with investigations (OSG-9 Chpt 19)
- **Investigation**: a formal inquiry and systematic process that involves gathering information to determine the cause of a security incident or violation
- Investigators must be able to conduct reliable investigations that will hold up in court; securing the scene is an essential and critical part of every investigation
    - securing the scene might include any/all of the following:
        - sealing off access to the area or crime scene
        - taking images of the scene
        - documenting evidence
        - ensuring evidence (e.g. computers, mobile devices, portable drives etc) is not contacted, tampered with, or destroyed 
    - general principles:
        - identify and secure the scene
        - protect evidence -- proper collection of evidence preserves its integrity and the chain of custody
        - identification and examination of the evidence
        - further analysis of the most compelling evidence
        - final reporting of findings
    
- **Locard exchange principle**: whenever a crime is commited something is taken, and something is left behind
- The purpose of an investigation is to:
    - identify the root cause of the incident
    - prevent future occurrences
    - mitigate the impact of the incident on the organization
- Types of investigations:
    - **administrative**: an investigation that is focused on policy violations
    - **criminal**: conducted by law enforcement, this type of investigation tries to determine if there is cause to believe (beyond a reasonable doubt) that someone committed a crime
        - the goal is to gather evidence that can be used to convict in court
        - the job of a security professional is to preserve evidence, ensure law enforcement has been contacted, and assist as necessary
    - **civil**: non-criminal investigation for matters such as contract disputes
        - the goal of a civil investigation is to gather evidence that can be used to support a legal claim in court, and is typically triggered from an imminent or on-going lawsuit
        - the level of proof is much lower for a civil compared to a criminal investigation
    - **regulatory**: investigation initiated by a government regulator when there is reason to believe an organization is not in compliance
        -  this type of investigation varies significantly in scope and could look like any of the other three types of investigation depending on the severity of the allegations
        - as with criminal investigations, it is key to preserve evidence, and assist the regulator’s investigators

- 7.1.1 Evidence collection and handling
    - Evidence collection is complex, should be done by professionals, and can be thrown out of court if incorrectly handled
    - It’s important to preserve original evidence
    - International Organization on Computer Evidence (IOCE) six principles for media, network and software analysis:
        - all general forensic and procedural principles must be applied to digital evidence collection 
        - seizing digital evidence shouldn't change the evidence
        - accessing original digital evidence should only be done by trained professionals
        - all activity relating to seizure, access, storage, or transfer of digital evidence must be fully documented, preserved, and available for review
        - a person in possession of digital evidence is responsible for all actions taken with respect to that evidence
        - any agency that is responsible for seizing, accessing, storing, or transferring digital evidence is responsible for compliance with these principles
    - Scientific Working Group on Digital Evidence (SWGDE) developed principles for standardized recovery of computer-based evidence:
        - legal system consistency
        - use of a common language
        - durability
        - ability to cross international and state boundaries
        - instill confidence in evidence integrity
        - forensic evidence applicability at the individual, agency, and country levels
    - **ISO/IEC 27037: Guidelines for Identification, Collection, Acquisition, and Preservation of Digital Evidence**: the international standard on digital evidence handling, with four phases:
        - identification
        - collection 
        - acquisition
        - preservation
    - Types of evidence:
        - **primary evidence**:
            - most reliable and used at trial
            - original documents (e.g. legal contracts), no copies or duplicates
        - **secondary evidence**:
            - less powerful and reliable than primary evidence (e.g. copies of originals, witness oral evidence etc)
            - if primary evidence is available secondary of the same content is not valid
        - **real evidence**: this type of evidence includes physical objects, such as computers, hard drives, and other storage devices, that can be brought into a court of law
        - **direct evidence**: this type of evidence is based on the observations of a witness or expert opinion and can be used to prove a fact at hand (with backup evidence support)
        - **circumstantial evidence**: this type of evidence is based on inference and can be used to support a conclusion, but not prove it
        - **corroborative evidence**: this type of evidence is used to support other evidence and can be used to strengthen a case
        - **hearsay evidence**: type of evidence that is based on statements made by someone outside of court and is generally not admissible
        - **best evidence rule**: states that the original evidence should be presented in court, rather than a copy or other secondary evidence
    - It is important to note that evidence should be collected and handled in a forensically sound manner to ensure that it is admissible in court and to avoid any legal issues
    - The chain of custody: focuses on having control of the evidence -- who collected and handled what evidence, when, and where
        - think about establishing the chain of custody as:
            - tag, 
            - bag, and 
            - carry the evidence
    - Five rules of evidence: five evidence characteristics providing the best chance of surviving legal and other scrutiny:
        - **authentic**: evidence is not fabricated or planted, and can be proven through crime scene photos, or bit-for-bit copies of storage
        - **accurate**: evidence that has integrity (not been modified)
        - **complete**: evidence must be complete, and all parts available and shared, whether they support the case or not
        - **convincing**: evidence must be easy to understand, and convey integrity
        - **admissible**: evidence must be accepted as part of a case

- 7.1.2 Reporting and documentation
    - Each investigation should result in a final report that documents the goals of the investigation, the procedures followed, the evidence collected, and the final results
    - Preparing formal documentation prepares for potential legal action, and even internal investigations can become part of employment disputes
    - Identify in advance a single point of contact who will act as your liasion with law enforcement, providing a go-to person with a single perspective, potentially improving the working relationship
    - Participate in the FBI’s InfraGard program

- 7.1.3 Investigative techniques
    - Whether in response to a crime or incident, an organizational policy breach, troubleshooting a system or network issue etc, digital forensic methodologies can assist in finding answers, solving problems, and in some cases, help in successfully prosecuting crimes
    - The forensic investigation process should include the following:
        - identification and securing of a crime scene
        - proper collection of evidence that preserves its integrity and the chain of custody
        - examination of all evidence
        - further analysis of the most compelling evidence
        - final reporting
    - Sources of information and evidence:
        - oral/written statements: given to police, investigators, or as testimony in court by people who witness a crime or who may have pertient information
        - written documents: checks, printed contracts, handrwitten letters/notes
        - computer systems: components, local/portable storage, memory etc
        - visual/audio: visual and audio evidence pertient to a security investigation could include photographs, video, taped recordings, and surveillance footage from security cameras
    - Several investigative techniques can be used when conducting analysis:
        -  media analysis: examining the bits on a hard drive that are intact dispite not having an index
        - software analysis: focuses on an applications and malware, determining how it works and what it's trying to do, with a goal of attribution

- 7.1.4 Digital forensics tools, tactics, and procedures
    - Digital forensics: the scientific examination and analysis of data from storage media so that the information can be used as part of an investigation to identify the culprit or the root cause of an incident
    - **Live evidence**: data stored in a running system e.g. random access memory (RAM), cache, and buffers
    - Examining a live system can change the state of the evidence 
        - small changes like interacting with the keyboard, mouse, loading/unloading programs, or of course powering off the system, can change or eliminate live evidence
    - Whenever a forensic investigation of a storage drive is conducted, two identical bit-for-bit copies of the original drive should be created first
    - **eDiscovery**: the process of identifying, collecting, and producing electronic evidence in legal proceedings

- 7.1.5 Artifacts (e.g. computer, network, mobile device)
    - Forensic artifacts: remnants of a system or network breach/attempted breach, which and may or may not be relevant to an investigation or response
    - Artifacts can be found in numerous places, including:
        - computer systems
        - web browsers
        - mobile devices
        - hard drives, flash drives

[7.2](#7.2) Conduct logging and monitoring activities (OSG-9 Chpts 17,21)

- 7.2.1 Intrusion detection and prevention
    - **Intrusion**: occurs when an attacker can bypass or thwart security mechanisms and access an organization’s resources
    - **Intrusion detection**: a specific form of monitoring events, usually in real time, to detect abnormal activity indicating a potential incident or intrusion
    - **Intrusion Detection System (IDS)**: automates the inspection of logs and real-time system events to detect intrusion attempts and system failures
        - an IDS is intended as part of a defense-in-depth security plan
    - **Intrusion Prevention Systems (IPS)**: includes detection capabilities, you’ll also see them referred to as intrusion detection and prevention systems (IDPSs)
    - NIST SP 800-94 Guide to Intrusion Detection and Prevention Systems provides comprehensive coverage of both IDS and IPS
- 7.2.2 Security Information and Event Management (SIEM)
    - Security Information and Event Management (SIEM): systems that ingest logs from multiple sources, compile and analyze log entries, and report relevant information
        - SIEM systems are complex and require expertise to install and tune
        - require a properly trained team that understands how to read and interpret info, and escalation procedures to follow when a legitimate alert is raised
        - SIEM systems represent technology, process, and people, and each is important to overall effectiveness
        - a SIEM includes significant intelligence functionality, allowing large amounts of logged events and analysis and correlation of the same to occur very quickly
    - SIEM capabilities include:
        - Aggregation
        - Normalization
        - Correlation
        - Secure storage
        - Analysis
        - Reporting
- 7.2.3 Continuous monitoring
    - After a SIEM is set up, configured, tuned, and running, it must be routinely updated and continuously monitored to function effectively
    - Effective continuous monitoring encompasses technology, processes, and people
    - Continuous monitoring steps are:
        - Define
        - Establish
        - Implement
        - Analyze/report
        - Respond
        - Review/update
    - **monitoring**: the process of reviewing information logs, looking for something specific
        - necessary to detect malicious actions by subjects as well as attempted intrusions and system failures
        - can help reconstruct events, provide evidence for prosecution, and create reports for analysis
        - continuous monitoring ensures that all events are recorded and can be investigated later if necessary
    - **log analysis**: a detailed and systematic form of monitoring where logged info is analyzed for trends and patterns as well as abnormal, unauthorized, illegal, and policy-violating activities
        - log analysis isn’t necessarily in response to an incident, it’s a periodic task
    
- 7.2.4 Egress monitoring
    - It’s important to monitor traffic exiting as well as entering a network, and **Egress monitoring** refers to monitoring outgoing traffic to detect unauthorized data transfer outside the org (AKA data exfiltration)
    - Common methods used to detect or prevent data exfiltration are data loss prevention (DLP) techniques and monitoring for steganography
- 7.2.5 Log management
    - **Log management**: refers to all the methods used to collect, process, and protect log entries (see SIEM definition above)
    - **rollover logging**: allows admins to set a maximum log size, when the log reaches that max, the system begins overwriting the oldest events in the log
- 7.2.6 Threat intelligence (e.g. threat feeds, threat hunting)
    - **Threat intelligence**: an umbrella term encompassing threat research and analysis and emerging threat trends; gathering data on potential threats, including various sources to get timely info on current threats
    - **Kill chain**: military model (used for both offense and defense):
        - find/identify a target through reconnaissance
        - get the target’s location
        - track the target’s movement
        - select a weapon to use on the target
        - engage the target with the selected weapon
        - evaluate the effectiveness of the attack
    - Orgs have adapted this model for cybersecurity: Lockheed Martin created the **Cyber Kill Chain** framework including seven ordered stages of an attack:
        - reconnaissance: attackers gather info on the target
        - weaponize: attackers identify an exploit that the target is vulnerable to, along with methods to send the exploit
        - delivery: attackers send the weapon to the target via phishing attacks, malicious email attachments, compromised websites, or other common social engineering methods
        - exploitation: the weapon exploits a vulnerability on the target system
        - installation: code that exploits the vulnerability then installs malware with a backdoor allowing attacker remote access
        - command and control: attackers maintain a command and control system, which controls the target and other compromised systems
        - actions on objectives: attackers execute their original goals such as theft of money, or data, destruction of assets, or installing additional malicious code (eg. ransomware)
    
- 7.2.7 use and Entity Behavior Analytics (UEBA)
    - **UEBA (aka UBA)**: focuses on the analysis of user and entity behavior; analysis engines are typically included with SIEM solutions or may be added via subscription
    - **Behavior-based detection**: AKA statistical intrusion, anomaly, and heuristics-based detection, starts by creating a baseline of normal activities and events; once enough baseline data has been accumulated to determine normal activity, it can detect abnormal activity (that may indicate a malicious intrusion or event)
    - Behavior-based IDSs use the baseline, activity statistics, and heuristic evaluation techniques to compare current activity against previous activity to detect potentially malicious events

[7.3](#7.3) Perform Configuration Management (CM) (e.g. provisioning, baselining, automation) (OSG-9 Chpt 16)
- **Configuration Management (CM)**: the process of identifying, controlling, and verifying the configuration of systems and components throughout their lifecycle
    - CM is an integral part of secure provisioning and relates to the proper configuration of a device at the time of deployment
    - CM helps ensure that systems are deployed in a secure, consistent state and that they stay in a secure, consistent state throughout their lifecycle
- **Provisioning** refers to installing and configuring the operating system and needed apps on new systems
    - new systems should be configured to reduce vulnerabilities introduced via default configurations; the key is to harden a system based on intended useage
- **Hardening a system**: makes it more secure than the default configuration and includes the following:
    - disable all unused services
    - close all unused logical ports
    - remove all unused apps
    - change default passwords
- **Baseline**: in the context of configuration management, it is the starting point or starting config for a system
    - an easy way to think of a baseline is as a list of services; an OS baseline identifies all the settings to harden specific systems
    - many organizations use images to deploy baselines; baseline images improve the security of systems by ensuring that desired security settings are always configured correctly
    - baseline images improve the security of systems by ensuring that desired security settings are always configured correctly; they also reduce the amount of time required to deploy and maintain systems, reducing overall maintenance costs
- Automation: it's typical to create a baseline, and then use automated methods to add additional apps, features, or settings for specific groups of computers
    - note that admins can use create/modify group policy settings to create domain-level standardization or to make security-related Windows registry changes

[7.4](#7.4) Apply foundational security operations concepts (OSG-9 Chpt 16)
- Security operations encompasses the day-to-day tasks, practices, and processes involved in securing and maintaining the operational integrity of an organization's information systems and assets; it includes security monitoring, incident response, and security awareness and training
- The primary purpose of security operations practices is to safeguard assets such as information, systems, devices, facilities, and apps, and helping organizations to detect, prevent, and respond to security threats
- Implementing common security operations concepts, along with performing periodic security audits and reviews, demonstrates a level of due care and due diligence

- 7.4.1 Need-to-know/least privilege
    - **Need-to-know principle**: imposes the requirement to grant users access only to data or resources they need to perform assigned work tasks
    - **Least privilege principle**: states that subjects are granted only the privileges necessary to perform assigned work tasks and no more
        - privilege in this context includes both permissions to data and rights to perform systems tasks
        - limiting and controlling privileges based on this concept protects confidentiality and data integrity
        - principle relies on the assumption that all users have a well-defined job description that personnel understand
        - least privilege is typically focused on ensuring that user privileges are restricted, but it also applies to apps or processes (e.g. if an app or service is compromised, the attacker can assume the service account’s privileges)
- 7.4.2 Separation of Duties (SoD) and responsibilities
    - **Separation of Duties (SoD)**: ensures that no single person has total control over a critical function or system
        - SoD policies help reduce fraud by requiring collusion between two or more people to perform unauthorized activity
        - example of how SoD can be enforced, is by dividing the security or admin capabilities and functions among multiple trusted individuals
    - **Two-person control**: (AKA two-man rule) requires the approval of two individuals for critical tasks
        - using two-person controls within an org ensures peer review and reduces the likelihood of collusion and fraud
        - ex: privilege access management (PAM) solutions that create special admin accounts for emergency use only; perhaps a password is split in half so that two people need to enter the password to log on
    - **Split knowledge**: combines the concepts of separation of duties and two-person control into a single solution; the info or privilege required to perform an operation is divided among two or more users, ensuring that no single person has sufficient privileges to compromise the security of the environment

- 7.4.3 Privilege account management
    - **Privileged Account Management (PAM)**: solutions that restrict access to privileged accounts or detect when accounts use any elevated privileges (e.g. admin accounts)
        - Microsoft domains, this includes local admin accounts, Domain and Enterprise Admins groups
        - Linux includes root or sudo accounts
    - PAM solutions should monitor actions taken by privileged accounts, new user accounts, new routes to a router table, altering config of a firewall, accessing system log and audit files
    - Principles such as least privilege and separation of duties help prevent security policy violations, and monitoring helps to deter and detect any violations that occur despite the use of preventive controls

- 7.4.4 Job rotation
    - **Job rotation**: (AKA rotation of duties) means that employees rotate through jobs or rotate job responsibilities with other employees
        - using job rotation as a security control provides peer review, reduces fraud, and enables cross-training
        - job rotation policy can act as both a deterrent and a detection mechanism
- 7.4.5 Service Level Agreements (SLA)
    - **Service Level Agreement (SLA)**: an agreement between an organization and an outside entity, such as a vendor, where the SLA stipulates performance expectations and often includes penalties if the vendor doesn’t meet these expectations
    - **Memoradum of Understanding (MOU)**: documents the intention of two entities to work together toward a common goal

[7.5](#7.5) Apply resource protection (OSG-9 Chpt 16)
- 7.5.1 Media management
- 7.5.2 Media protection techniques

[7.6](#7.6) Conduct incident management (OSG-9 Chpt 17)
- 7.6.1 Detection
- 7.6.2 Response
- 7.6.3 Mitigation
- 7.6.4 Reporting
- 7.6.5 Recovery
- 7.6.6 Remediation
- 7.6.7 Lessons Learned

[7.7](#7.7) Operate and maintain detective and preventative measures (OSG-9 Chpts 11,17)
- 7.7.1 Firewalls (e.g. next generation, web application, network)
- 7.7.2 Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS)
- 7.7.3 Whitelisting/blacklisting
- 7.7.4 Third-party provided security services
- 7.7.5 Sandboxing
- 7.7.6 Honeypots/honeynets
- 7.7.7 Anti-malware
- 7.7.8 Machine learning and Artificial Intelligence (AI) based tools

[7.8](#7.8) Implement and support patch and vulnerability management (OSG-9 Chpt 16)

[7.9](#7.9) Understand and participate in change management processes (OSG-9 Chpt 16)

[7.10](#7.10) Implement recovery strategies (OSG-9 Chpt 18)
- 7.10.1 Backup storage strategies
- 7.10.2 Recovery site strategies
- 7.10.3 Multiple processing sites
- 7.10.4 System resilience, High Availability (HA), Quality of Service (QoS), and fault tolerance

[7.11](#7.11) Implement Disaster Recovery (DR) processes (OSG-9 Chpt 18)
- 7.11.1 Response
- 7.11.2 Personnel
- 7.11.3 Communications
- 7.11.4 Assessment
- 7.11.5 Restoration
- 7.11.6 Training and awareness
- 7.11.7 Lessons learned

[7.12](#7.12) Test Disaster Recovery Plans (DRP) (OSG-9 Chpt 18)
- 7.12.1 Read-through/tabletop
- 7.12.2 Walkthrough
- 7.12.3 Simulation
- 7.12.4 Parallel
- 7.12.5 Full interruption

[7.13](#7.13) Particpate in Business Continuity (BC) planning and exercises (OSG-9 Chpt 3)

[7.14](#7.14) Implement and manage physical security (OSG-9 Chpt 10)
- 7.14.1 Perimeter security controls
- 7.14.2 Internal security controls

[7.15](#7.15) Address personnel safety and security concerns (OSG-9 Chpt 16)
- 7.15.1 Travel
- 7.15.2 Security training and awareness
- 7.15.3 Emergency management
- 7.15.4 Duress
