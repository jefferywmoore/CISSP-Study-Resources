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
    - **Static code scanning techniques**: the scanner scans code in files, similar to white box testing
    - **Dynamic techniques**: the scanner runs executable files in a sandbox to observe their behavior.

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
    - Principles such as least privilege and separation of duties help prevent security policy violations, and monitoring helps to deter and detect any violations that occur despite the use of preventive controls

- 7.4.3 Privilege account management
    - **Privileged Account Management (PAM)**: solutions that restrict access to privileged accounts or detect when accounts use any elevated privileges (e.g. admin accounts)
        - Microsoft domains, this includes local admin accounts, Domain and Enterprise Admins groups
        - Linux includes root or sudo accounts
    - PAM solutions should monitor actions taken by privileged accounts, new user accounts, new routes to a router table, altering config of a firewall, accessing system log and audit files
    
- 7.4.4 Job rotation
    - **Job rotation**: (AKA rotation of duties) means that employees rotate through jobs or rotate job responsibilities with other employees
        - using job rotation as a security control provides peer review, reduces fraud, and enables cross-training
        - job rotation policy can act as both a deterrent and a detection mechanism
- 7.4.5 Service Level Agreements (SLA)
    - **Service Level Agreement (SLA)**: an agreement between an organization and an outside entity, such as a vendor, where the SLA stipulates performance expectations and often includes penalties if the vendor doesn’t meet these expectations
    - **Memoradum of Understanding (MOU)**: documents the intention of two entities to work together toward a common goal

[7.5](#7.5) Apply resource protection (OSG-9 Chpt 16)
- Media management should consider all types of media as well as short- and long-term needs and evaluate:
    - Confidentiality
    - Access speeds
    - Portability
    - Durability
    - Media format
    - Data format
- For the test, data storage media should include any of the following:
    - Paper
    - Microforms (microfilm and microfiche)
    - Magnetic (HD, disks, and tapes)
    - Flash memory (SSD and memory cards)
    - Optical (CD and DVD)
 - Mean Time Between Failure (MTBF) is an important criterion when evaluating storage media, especially where valuable or sensitive information is concerned
 - Media management includes the protection of the media itself, which typically involves policies and procedures, access control mechanisms, labeling and marking, storage, transport, sanitization, use, and end-of-life
- 7.5.1 Media management
    - **Media management**: refers to the steps taken to protect media (i.e. anything that can hold data) and the data stored on that media; includes mostt portable devices (e.g. smart phones, memory/flash cards etc)
    - As above, OSG-9 also refers to tape media, as well as “hard-copy data”
- 7.5.2 Media protection techniques
    - If media includes sensitive info, it should be stored in a secure location with strict access controls to prevent loss due to unauthorized access
        - any location used to store media should have temperature and humidity controls to prevent losses due to corruption
    - Media management can also include technical controls to restrict device access from computer systems
    - When media is marked, handled, and stored properly, it helps prevent unauthorized disclosure (loss of confidentiality), unauthorized modification (loss of integrity), and unauthorized destruction (loss of availability)

[7.6](#7.6) Conduct incident management (OSG-9 Chpt 17)
- Incident response is the process to detect and respond to incidents and to reduce the impact when incidents occur; it attempts to keep a business operating or restore operations as quickly as possible in the wake of an incident
- Incident management is usually conducted by an Incident Response Team (IRT), which comprises individuals with the required expertise and experience to manage security incidents; the IRT is accountable for implementing the incident response plan, which is a written record that defines the processes to be followed during each stage of the incident response cycle

- The main goals of incident response:
    - Provide an effective and efficient response to reduce impact to the organization
    - Maintain or restore business continuity
    - Defend against future attacks

- An important distinction needs to be made to know when an incident response process should be initiated: events take place continually, and the vast majority are insignificant; however, events that lead to some type of adversity can be deemed incidents, and those incidents should trigger an org's incident response process steps:
    - **Preparation**: includes developing the IR process, assigning IR team members, and everything related to what happens when an incident is identified; preparation is critical, and will anticipate the steps to follow
    - **Analysis:** Gathering and analyzing information about the incident to determine its scope, impact, and root cause (e.g., by interviewing witnesses, collecting and analyzing evidence, and reviewing system logs).
    - **Containment:** Limiting the impact of the incident and preventing further damage (e.g., by isolating affected systems, changing passwords, and implementing security controls).
    - **Eradication:** Removing the cause of the incident (e.g., by removing malware, patching vulnerabilities, and disabling compromised accounts).
    - **Recovery:** Restoring systems and data to their normal state (e.g., by restoring from backups, rebuilding systems, and re-enabling compromised accounts).
    - **Lessons Learned:** Documenting the incident and learning from it to improve future responses (e.g., by identifying areas where the incident response process can be improved and by sharing lessons learned with other organizations)

- The following steps (Detection, Response, Migtation, Reporting, Recovery, Remediation, and Lessons Learned) are on the exam
- 7.6.1 Detection
    - **Detection:** the identification of potential security incidents via monitoring and analyzing security logs, threat intelligence, or incident reports; as above, understanding the distinction between an event and an incident, the goal of detection is to identify an adverse event (an incident) and begin dealing with it
    - Common methods to detect incidents:
        - intrusion detection and prevention systems
        - antimalware
        - automated tools that scan audit logs looking for predefined events
        - end users sometimes detect irregular activity and contact support
    - Note: receiving an alert or complaint doesn’t always mean an incident has occurred
- 7.6.2 Response
    - After detecting and verifying an incident, the next step is activate an Incident Response (IR) or CSIRT team 
    - An IR team is AKA computer incident response team (CIRT) or computer security incident response team (CSIRT)
    - Among the first steps taken by the IR Team will be an impact assessment to determine the scale of the incident, how long the impact might be experienced, who else might need to be involved etc.
    - The IR team typicall investigate the incident, assess the damage, collect evidence, report the incident, perform recovery procedures, and participate in the remediation and lessons learned stages, helping with root cause analysis
    - its important to protect all data as evidence during an investigation, and computers should not be turned off

- 7.6.3 Mitigation
    - **Migitation**: attempt to contain an incident; in addition to conducting an impact assessment, the IR Team will attempt to minimize or contain the damage or impact from the incident
    - The IR Team's job at this point is not to fix the problem; it's simply to try and prevent further damage
    - Note this may involve disconnecting a computer from the network; sometimes responders take steps to mitigate the incident, but without letting the attacker know that the attack has been detected

- 7.6.4 Reporting
    - Reporting occurs throughout the incident response process 
    - Once an incident is mitigated, formal reporting occurs because numerous stakeholders often need to understand what has happened
    - Jurisdictions may have specific laws governing the protection of personally identifiable information (PII), and must report if it's been exposed
    - Additionally, some third-party standards, such as the Payment Card Industry Data Security Standard (PCI DSS), require orgs to report certain security incidents to law enforcement

- 7.6.5 Recovery
    - At this point, the goal is to start returning to normal
    - Recovery is the next step, returning a system to a fully functioning state
    - The most secure method of restoring a system after an incident is completely rebuilding the system from scratch, including restoring all data from the most recent backup
        - effective configuration and change management will provide the necessary documentation to ensure the rebuilt systems are configured properly
    - According to the OGS, you should check these areas as part of recovery:
        - access control lists (ACLs), including firewall or router rules
        - services and protocols, ensuring the unneeded services and protocols are disabled or removed
        - patches
        - user accounts, ensuring they have changed from default configs
        - known compromises have been reversed

- 7.6.6 Remediation
    - Remediation stage: personnel look at the incident, identify what allowed it to occur, and then implement methods to prevent it from happening again
    - Remediation includes performing a root cause analysis (which examines the incident to determine what allowed it to happen), and if  the root cause analysis identifies a vulnerability that can be mitigated, this stage will recommend a change

- 7.6.7 Lessons Learned
    - Lessons learned stage: an all-encompassing view of the situation related to an incident, where personnel, including the IR team and other key stakeholders, examine the incident and the response to see if there are any lessons to be learned
        - the output of this stage can be fed back to the detection stage of incident management
    - It's common for the IR team to create a report when they complete a lessons learned review
        - based on the findings, the team may recommend changes to procedures, the addition of security controls, or even changes to policies
        - management will decide what recommendations to implement and is responsible for the remaining risk for any recommendations they reject

- NOTE: Incident management DOES NOT include a counterattack against the attacker

- Incident Response Summary:

    | Step | Stage | Action/Goal |  
    |--------|---------------| -----------|
    | Preparation|||
    | Detection  | Triage||
    | Response | Triage| activate IR team |
    | Mitigation  | Investigate| containment|
    | Reporting  | Investigate||
    | Recovery | Recovery | return to normal|
    | Remediation  | Recovery| prevention|
    | Lessons Learned | Recovery| improve process|


[7.7](#7.7) Operate and maintain detective and preventative measures (OSG-9 Chpts 11,17)

- As noted in Domain 1, a preventive or preventative control is deployed to thwart or stop unwanted or unauthorized activity from occurring
    - Examples:
        - fences
        - locks
        - biometrics
        - separation of duties policies
        - job rotation policies
        - data classification
        - access control methods
        - encryption
        - smart cards
        - callback procedures
        - security policies
        - security awareness training
        - antivirus software
        - firewalls
        - intrusion prevention systems
- A detective control is deployed to discover or detect unwanted or unauthorized activity; detective controls operate after the fact
    - Examples:
        - security guards
        - motion detectors
        - recording and reviewing of events captured by security cameras
        - job rotation policies
        - mandatory vacation policies
        - audit trails
        - honeypots or honeynets
        - intrusion detection systems
        - violation reports
        - supervision and reviews of users
        - incident investigations
- Some preventative measures:
    - Keep systems and applications up to date
    - Remove or disable unneeded services and protocols
    - Use intrusion detection and prevention systems
    - Use up-to-date antimalware software
    - Use firewalls
    - Implement configuration and system management processes
    
- 7.7.1 Firewalls (e.g. next generation, web application, network)
    - Firewalls are preventive and technical controls
    - Types of firewalls:
        - application gateway firewall: filters traffic based on specific application requirements
        - circuit-level gateway firewall: designed to provide connection security to internal and external computers in a network's session layer, they filter traffic based on the communications circuit; they do not engage in packet filtering based on packet contents
        - third-generation firewalls: (AKA stateful inspection firewalls and dynamic packet filtering firewalls) filter traffic based on its state within a stream of traffic
        - app firewalls: control traffic going to or from a specific app or service
            - e.g. a web application firewall (WAF) inspects traffic going to a web server and can block malicious traffic such as SQL injection attacks and cross-site scripting (XSS) attacks
        - next-generation firewall (NGFW): functions as a unified threat management (UTM) device and combines several capabilities, including traditional functions such as packet filtering and stateful inspection, and can also perform packet inspection allowing identification and blocking of malicious traffic

- 7.7.2 Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS)
    - Intrusion Detection Systems (IDSs) and Intrusion Prevention Systems (IPSs) are two methods organizations typically implement to detect and prevent attacks
    - **Intrusion detection**: a specific form of monitoring events, usually in real time, to detect abnormal activity indicating a potential incident or intrusion
        - Intrusion Detection System (IDS) automates the inspection of logs and real-time system events to detect intrusion attempts and system failures
        - IDSs are an effective method of detecting many DoS and DDoS attacks
        - an IDS actively watches for suspicious activity by monitoring network traffic and inspecting logs
        - an IDS is intended as part of a defense-in-depth security plan
        - **knowledge-based detection**: AKA signature-based or pattern-matching detection, the most common method used by an IDS
        - **behavior-based detection**: AKA statistical intrusion, anomaly, and heuristics-based detection; behavior-based IDSs use baseline, activity stats, and heuristic eval techniques to compare current activity against previous activity to detect potentially malicious events
    - An IPS includes detection capabilities, you’ll see them referred to as intrusion detection and prevention systems (IDPSs)
        - an IPS includes all the capabilities of an IDS but can also take additional steps to stop or prevent intrusions
    - IDS/IPS should be deployed at strategic network locations to monitor traffic, such as at the perimeters, or between network segments, and should be configured to alert for specific types of scans and traffic patterns
    - See NIST SP 800-94

- 7.7.3 Whitelisting/blacklisting
    - Method used to control which applications run and which applications can’t is allow list and deny list (AKA whitelists and blacklists)
    - **Allow list**:: identifies a list of apps authorized to run on a system and blocks all other apps
    - **Deny list**: identifies a list of apps that are not authorized to run on a system
    - Allow and deny lists use for applications help to prevent malware infections
    - Important to note: a system would only use one list, either allow or deny
    - Apple iOS running on iPhones/iPads is an example of an extreme version of an allow list; users are only able to install apps from the App Store
- 7.7.4 Third-party provided security services
    - Some orgs outsource security services such as auditing and penetration testing to third party security services
    - Some outside compliance entities (e.g. PCI DSS) require orgs to ensure that service providers comply
    - OSG also mentions that some SaaS vendors provide security services via the cloud (e.g. next-gen firewalls, UTM devices, and email gateways for spam and malware filtering)
- 7.7.5 Sandboxing
    - **Sandboxing**: refers to a security technique where a separate, secure environment is created to run and analyze untested or untrusted programs or code without risking harm to the host device or network; this isolated environment, known as a sandbox, effectively contains the execution of the code, allowing it to run and behave as if it were in a normal computing environment, but without the ability to affect the host system or access critical resources and data 
    - Sandboxing provides a security boundary for applications and prevents the app from interacting with other apps
- 7.7.6 Honeypots/honeynets
    - **Honeypots**: individual computers created as a trap or a decoy for intruders or insider threats
    - **Honeynet**: two or more networked honeypots used together to simulate a network
    - They look and act like legit systems, but they do not host data of any real value for an attacker; admins often configure honeypots with vulnerabilities to tempt intruders into attacking them
    - In addition to keeping the attacker away from a production environment, the honeypot allows administrators to observe an attacker’s activity without compromising the live environment
- 7.7.7 Anti-malware
    - Malware is malicious software that negatively impacts a system
    - The most important protection against malicious code is the use of antimalware software with up-to-date signature files and heuristic capabilities
        - multi-pronged approach with antimalware software on each system in addition to filtering internet content helps protect systems from infections
        - following the principle of least privilege, ensuring users do not have admin permissions on systems won’t be able to install apps that may be malicious
    
    - These are the characteristics of each malware type:
        - virus: the defining characteristic is that it's a piece of malware that has to be triggered in some way by the user
        - worm: malware that can self-propagate and spread through a network or a series of systems on its own by exploiting a vulnerability in those systems
        - companion: helper software -- it's not malicious on its own; it could be something like a wrapper that accompanies the actual malware
        - macro: associated with Microsoft Office products, and is created using a straightforward programming language to automate tasks; macros can be programmed to be malicious and harmful
        - multipartite: means the malware spreads in different ways; (e.g. Stuxnet)
        - polymorphic: malware that can change aspects of itself as it replicates to evade detection (e.g. file name, file size, code structure etc)
        - trojan: A Trojan horse is malware that looks harmless or desirable but contains malicious code; trojans are often found in easily downloadable software
        - botnet: many infected systems that have been harnessed together and act in unison
        - boot sector infectors: pieces of malware that can install themselves in the boot sector of a drive
        - hoaxes/pranks: not actually software, they're usually part of social engineering—via email or other means—that intends harm (hoaxes) or a joke (pranks)
        - logic bomb: code that will execute based on some triggering event
        - stealth: malware that uses various active techniques to avoid detection
        - ransomware: type of malware that typically encrypts a system or a network of systems, effectively locking users out, and then demands a ransom payment (usually in the form of a digital currency) to gain access to the decryption key
        - rootkit: Similar to stealth malware, a rootkit attempts to mask its presence on a system; typically includes a collection of malware tools that an attacker can utilize according to specific goals
        - zero-day: is any type of malware that's never been seen in the wild before, and the vendor of the impacted product is unaware (or hasn't issued a patch), as are security companies that create anti-malware software intended to protect systems

- 7.7.8 Machine learning and Artificial Intelligence (AI) based tools
    - **AI**: gives machines the ability to do things that a human can do better or allows a machine to perform tasks that we previously thought required human intelligence
    - **Machine Learning**: a subset of AI and refers to a system that can improve automatically through experience
        - a ML system starts with a set of rules or guidelines
        - an AI system starts with nothing and progressively learns the rules, creating its own algorithms as it learns the rules and applies ML techniques based on these rules
    - Behavior-based detection is one way ML and AI can apply to cybersecurity
        - an admin relates a baseline of normal activities and traffic on a network; the baseline in this case is similar to a set of rules given to a ML system
        - during normal operations, it detects anomalies and reports them; if the detection is a false positive, the ML system learns
    - An AI system starts without a baseline, monitors traffic and slowly creates its own baseline based on the traffic it observes
        - as it creates the baseline it also looks for anomalies
        - an AI system also relies on feedback from admins to learn if alarms are valid or false positives
[7.8](#7.8) Implement and support patch and vulnerability management (OSG-9 Chpt 16)
    - Patch and vulnerability management processes work together to help protect an org against emerging threats; patch management ensures that appropriate patches are applied, and vuln management helps verify that systems are not vulnerable to known threats
    - **Patch**: (AKA updates, quick or hot fixes) a blanket term for any type of code written to correct bug or vulnerability or to improve existing software performance
        - in the context of security, admins are primarily concerned with security patches, which are patches that affect a system’s vulns
    - An effective patch management program ensures that systems are kept up to date with current patches
    - **Patch Tuesday**: several big-tech orgs (e.g. Microsoft, Adobe, Oracle etc) regularly release patches on the second Tuesday of every month
    - There are three methods for determining patch levels:
        - agent: update software (agent) installed on devices
        - agentless: remotely connect to each device
        - passive: monitor traffic to infer patch levels
    - Deploying patches can be done manually or automatically
    - Common steps within an effective program:
        - evaluate patches: determine if they apply to your systems
        - test patches: test patches on an isolated, non-production system to determine if the patch causes any unwanted side effects
        - approve the patches: after successful testing, patches are approved for deployment; it’s common to use Change Management as part of the approval process
        - deploy the patches: after testing and approval, deploy the patches; many orgs use automated methods to deploy patches, via third-party or the software vendor
        - verify that patches are deployed: regularly test and audit systems to ensure they remain patched
    - **Vulnerability Management**: regularly identifying vulns, evaluating them, and taking steps to mitigate risks associated with them 
        - it isn’t possible to eliminate risks, and it isn’t possible to eliminate all vulnerabilities
        - a vuln managment program helps ensure that an org is regularly evaluating vulns and mitigating those that represent the greatest risk
        - one of the most common vulnerabilities within an org is an unpatched system, and so a vuln management program will often work in conjunction with a patch management program

[7.9](#7.9) Understand and participate in change management processes (OSG-9 Chpt 16)
- **Change management**: ensures that the costs and benefits of changes are analyzed and changes are made in a controlled manner to reduce risks
    - Change management processes allow various IT experts to review proposed changes for unintended consequences before implementing
    - Change management controls provide a process to control, document, track, and audit all system changes
- The change management process includes multiple steps that build upon each other:
    - Change request: a change request can come from any part of an org and pertain to almost any topic; companies typically use some type of change management software
    - Assess impact: after a change request is made, however small the request might be, the impact of the potential change must be assessed
    - Approval/reject: based on the requested change and related impact assessment, common sense plays a big part in the approval process
    - Build and test: after approval, any change should be developed and tested, ideally in a test environment
    - Schedule/notification: prior to implementing any change, key stakeholders should be notified
    - Implement: after testing and notification of stakeholders, the change should be implemented; it's important to have a roll-back plan, allowing personnel to undo the change
    - Validation: once implemented, senior management and stakeholders should again be notified to validate the change
    - Document the change: documentation should take place at each step; it's critical to ensure all documentation is complete and to identify the version and baseline related to a given change
- When a change management process is enforced, it creates documentation for all changes to a system, providing a trail of info if personnel need to reverse the change, or make the same change on other systems
- Change management control is a mandatory element for some security assurance requirements (SARs) in the ISO Common Criteria

[7.10](#7.10) Implement recovery strategies (OSG-9 Chpt 18)
- **Recovery strategy**: a plan for restoring critical business components, systems, and operations following a disruption
- **Disaster recovery (DR)**: set of practices that enables an organization to minimize loss of, and restore, mission-critical technology infrastructure after a catastrophic incident 
- **Business continuity (BC)**: set of practices that enables an organization to continue performing its critical functions through and after any disruptive event
- 7.10.1 Backup storage strategies
- 7.10.2 Recovery site strategies
- 7.10.3 Multiple processing sites
- 7.10.4 System resilience, High Availability (HA), Quality of Service (QoS), and fault tolerance
    - **System resilience**: the ability of a system to maintain an acceptable level of service during an adverse event
     - **High Availability (HA)**: the use of redundant technology components to allow a system to quickly recover from a failure after experiencing a brief disruption
     - **Quality of Service (QoS)**: controls protect the availability of data networks under load
        - many factors contribute to the quality of the end-user experience and QoS attempts to manage all of these factors to create an experience that meets business requirements
        - factors contributing to QoS:
            - bandwidth: the network capacity available to carry communications
            - latency: the time it takes a packet to travel from source to destination
            - packet loss: some packets may be lost between source and destination, requiring re-transmission
            - interference: electrical noise, faulty equipment, and other factors may corrupt the contents of packets
    - **fault tolerance**: the ability of a system to suffer a fault but continue to operate
   
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
