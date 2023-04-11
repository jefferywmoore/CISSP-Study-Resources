[Domain 3](#domain3-top) **Security Architecture and Engineering**

You may find this domain to be more technical than others, and if you have experience woring in a security engineering role you likely have an advantage. If not, allocate extra time to this domain to ensure you have a good understanding of the topics

[3.1](#3.1) Research, implement, and manage engineering processes using secure design principles

- **Threat modeling**: a security process where potential threats are identified, categorized, and analyzed. It can be performed as a proactive measure during design and development or as an reactive measure once a product has been deployed
    - Threat modeling identifies the potential harm, the probability of occurrence, the priority of concern, and the means to eradicate or reduce the threat
- **Least privilege**: states that subjects are granted only the privileges necessary to perform assigned work tasks and no more; this concept extends to data and systems
    - Limiting and controlling privileges based on this concept protects confidentiality and data integrity
- **Defense in Depth**: AKA layering, is the use of multiple controls in a series, where a single failed control should not result in exposure of systems or data. Layers should be used in a series (one after the other), NOT in parallel. When you see the terms levels, multilevel, layers, classifications, zones, realms, compartments, protection rings etc think about Defense in Depth
- **Secure defaults**: when you think about defaults, consider how something operates brand new, just turned over to you by the vendor
    - e.g. wireless router default admin password, or firewall configuration requiring changes to meet an organization's needs
- **Fail securely**: if a system, asset, or process fails, it shouldn't reveal sensitive information, or be less secure than during normal operation. Failing securely could involve reverting to defaults
- **Separation of duties (SoD)**: separation of duties (SoD) and responsibilities ensures that no single person has total control over a critical function or system;  SoD is a process to minimize opportunities for misuse of data or environment damage. 
    - e.g. one person sells tickets, another collects tickets and restricts access to ticket holders in a movie theater
- **Keep it simple**: AKA keep it simple, stupid (KISS), this concept is the encouragement to avoid overcomplicating the environment, organization, or product design
- **Zero Trust**: "assume breach"; a security concept and alternative the traditional (castle/moat) approach where nothing is automatically trusted. Instead each request for activity or access is assumed to be from an unknown and untrusted location until otherwise verified; 
    - Goal is to have every access request authenticated, authorized, and encrypted prior to access being granted to an asset or resource
- **Privacy by design (PbD)**: a guideline to integrate privacy protections into products during the earliest design phase rather than tacking it on at the end of development; 
    - Same overall concept as "security by design" or "integrated security" where security is an element of design and architecture of a product starting at initiation and continuing through the software development lifecycle (SDLC).
    - There are 7 recognized principles to achieve privacy by design:
        - Proactive, preventative: think ahead and design for things that you anticipate might happen
        - Default setting: make private by default, e.g. social media app shouldn't share user data with everybody by default
        - Embedded: build privacy in; don’t add it later
        - Full functionality, positive-sum: achieve both security and privacy, not just one or the other
        - Full lifecycle protection: privacy should be achieved before, during and after a transaction. Part of this is securely disposing of data when it is no longer needed
        - Visibility, transparency, open: publish the requirements and goals; audit them and publish the findings
        - Respect, user-centric: involve end users, providing the right amount of information for them to make informed decisions about their data

- **Trust but verify**: based on a Russian proverb, and no longer sufficient; it's the traditional approach of trusting subjects and devices within a company's security perimeter automatically, leaving an org vulnerable to insider attacks and providing intruders the ability to easily perform lateral movement
- **Shared responsibility**: the security design principle that indicates that organizations do not operate in isolation
    - Everyone in an organization has some level of security responsibility; 
    - the job of the CISO and security team is to establish & maintain security
    - The job of regular employees to perform their tasks within the confines of security
    - The job of the auditor is to monitor the environment for violations
    - When working with third parties, especially with cloud providers, each entity needs to understand their portion of the shared responsibility of performing work operations and maintaining security. This is often referenced as the **cloud shared responsibility model**


[3.2](#3.2) Understand the fundamental concepts of security modles (e.g. Biba, Star Model, Bell-LaPadula)

Security models: 
- Intended to provide an explicit set of rules that a computer can follow to implement the fundamental security concepts, processes, and procedures of a security policy 
- Provide a way for a designer to map abstract statements into a security policy prescribing the algorithms and data structures necessary to build  hardware and software
- Enable people to access only the data classified for their clearance level
- **Bell-LaPadula**: Model was established in 1973. The goal is to ensure that information is exposed only to those with the right level of classification
    - Focuse is on confidentiality 
    - Simple property: No read-up 
    - Star (*) property: No write-down (AKA confinement property)
    - Discretionary Security Property: uses an access matrix (need to know in order to access)
    - Doesn't address covert channels
- **Biba**: Released in 1977, this model was created to supplement Bell-LaPadula 
    - Focus is on integrity 
    - “No read down” (for example, users with a Top Secret clearance can’t read data classified as Secret)
    - “No write up” (for example, a user with a Secret clearance can’t write data to files classified as Top Secret)
    - By combining it with Bell-LaPadula, you get both confidentiality and integrity
- **Take-Grant**: 
    - The take-grant model employs a directed graph to dictate how rights can be passed from one subject to another, or from a subject to an object
    - Four rules: 
        - take 
        - grant 
        - create 
        - remove
- **Clark-Wilson**:
    - Designed to protect integrity using the access control triplet
    - A program interface is used to limit what is done by a subject; if the focus of an intermediary program between subject and object is to protect integrity, then it is an implementation of the Clark-Wilson model
- **Brewer and Nash Model**:
    - AKA "ethical wall", and "cone of silence"
    - created to permit access controls to change dynamically based on a user's previous activity 
- **Goguen-Meseguer Model**:
    - An integrity model
    - Foundation of noninterference conceptual theories
- **Sutherland Model**:
    - Focuses on preventing interference in support of integrity
- **Graham-Denning Model**
    - Focused on the secure creation and deletion of both subjects and objects
    - 8 primary protection rules or actions
        - 1-4:securely create/delete a subject/object
        - 5-8:securely provide the read/grant/delete/transfer access right
- **Harrison-Ruzzo-Ullman Model**:
    - Focuses on the assignment of object access rights to subjects as well as the resilience of those assigned rights
    - HRU is an extension of Graham-Denning model
- **Star Model**: 
    - Not an official model, but name refers to using asterisks (stars) to dictate whether a person at a specific level of confidentiality is allowed to write data to a lower level of confidentiality
    - Also determines whether a person can read or write to a higher or lower level of confidentiality

[3.3](#3.3) Select controls based upon systems security requirements

Be familiar with the **Common Criteria (CC)** for Information Technology Security Evaluation
- The CC provides a standard to evaluate systems, defining various levels of testing and confirmation of systems' security capabilities 
- The number of the level indicates what kind of testing and confirmation has been performed
- The important concepts:
    - To perform an evaluation, you need to select the **Target of Evaluation (TOE)** (e.g. firewall or an anti-malware app)
    - The evaluation process will look at the **protection profile (PP)**, which is a document that outlines the security needs (customer "I wants"). A vendor might use a specific protection profile for a particular solution
    - The evaluation process will look at the **Security Target (ST)**, specifying the claims of security from the vendor that are built into a TOE (the ST is usually published to customers and partners and available to internal staff)
    - An organization's PP is compared to various STs from the selected vendor's TOEs, and the closest or best match is what the org purchases
    - The evaluation will attempt to gauge the confidence level of a security feature 
    - **Security assurance requirements (SARs)** are documented and based on the development of the solution
    - Key actions during development and testing should be captured 
    - An **evaluation assurance level (EAL)** is a numerical rating used to assess the rigor of an evaluation. The scale is EAL 1 (cheap and easy) to EAL7 (expensive and complex)
        - EAL1: functionally tested
        - EAL2: structurally tested
        - EAL3: methodically tested and checked
        - EAL4: methodically designed, tested, and reviewed
        - EAL5: semi-formally designed and tested
        - EAL6: semi-formally verified, designed, and tested
        - EAL7: formally verified, designed, and tested
- **Authorization to Operate (ATO)**: official auth to use specific IT systems to perform tasks/accept identified risks

[3.4](#3.4) Understand security capabilities of Information Systems (IS) (e.g. memory protection, Trusted Platform Model (TPM), encryption/decryption)

Security capabilities of information systems include memory protection, virtualization, Trusted Platform Module (TPM), encryption/decryption, interfaces, and fault tolerance

A computing device is likely running multiple applications and services simultaneously, each
occupying a segment of memory. The goal of memory protection is to prevent one application or service from impacting another. There are two primary memory protection methods:
-  Process isolation: OS provides separate memory spaces for each processes instructions and data, and prevents one process from impacting another
- Hardware segmentation: forces separation via physical hardward controls rather than logical processes; in this type of segmentation, the operating system maps processes to dedicated memory locations.

**Virtualization**: technology used to host one or more operating systems within the memory of a single host, or to run applications that are not compatible with the host OS. The goal is to protect the hypervisor and ensure that compromising one VM doesn't affect others on that host

**Trusted Platform Module (TPM)**: a cryptographic chip that is sometimes included
with a client computer or server. A TPM enhances the capabilities of a computer by offering hardware-based cryptographic operations. Many security products and encryption solutions require a TPM
- TPM is both a specification for a cryptoprocessor chip on a motherboard and the general name for implementation of the specification
- A TPM is an example of a **hardware security module (HSM)**
- An HSM is a cryptoprocessor used to manage and store digital encryption keys, accelerate crypto operations, support faster digital signatures, and improve authentication

User interface: a constrained UI can be used in an application to restrict what users can do or see based on their privileges
- e.g. dimming/graying out capabilities for users without the correct privilege

An interface is also the method by which two or more systems communicate. 
Be aware of the common security capabilities of interfaces:
- Encryption/decryption: when communications are encrypted, a client and server can communicate without exposing information to the network; when an interface doesn’t provide such a capability, use IPsec or another encrypted transport mechanism
- Signing: used for non-repudiation; In a high-security environment,both encrypt and sign all communications if possible


[3.5](#3.5) Assess and mitigate the vulnerabilities of security architectures, designs and solution elements

[3.6](#3.6) Select and determine cryptographic solutions

[3.7](#3.7) Understand methods of cryptanalytic attacks

[3.8](#3.8) Apply security principles to site and facility design

[3.9](#3.9) Design site and facility security controls
