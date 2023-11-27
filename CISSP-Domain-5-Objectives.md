[Domain 5](#domain5-top) **Identity and Access Management (IAM)**

The identity and Access Management (IAM) domain focuses on issues related to granting and revoking privileges to access data or perform actions on systems
- Assets include information, systems, devices, facilities, and applications
- Organizations use both physical and logical access controls to protect them
- Identification is the process of a subject claiming, or professing, an identity
- Authentication verifies the subject’s identity by comparing one or more authentication factors against a database holding authentication info for users
- The three primary authentication factors are something you know, something you have, and something you are
- Single sign-on (SSO) technologies allow users to authenticate once and access any resources in a network or the cloud, without authenticating again
- Federated Identity Management (FIM) systems link user identities in one system with other systems to implement SSO

[5.1](#5.1) Control physical and logical access to assets (OSG-9 Chpt 13)
- Controlling access to assets (tangible: things you can touch, or nontangible: info and data) is a central theme of security
- In addition to personnel, assets can be information, systems, devices, facilities, or applications:
    - 5.1.1 Information: an org’s information includes all of its data, stored in simple files (on servers, computers, and small devices), or in databases
    - 5.1.2 Systems: an org’s systems include anything that provide one or more services; a web server with a database is a system; permissions assigned to user and system accounts control system access
    - 5.1.3 Devices: refers to any computing system (e.g. routers & switches, smartphones, laptops, and printers); BYOD has been increasingly adopted, and the data stored on the devices is still an asset to the org
    - 5.1.4 Facilities: any physical location, building, rooms, complexes etc; physical security controls are important to help protect facilities
    - 5.1.5 Applications: apps provide access to data; permissions are an easy way to restrict logical access to apps
- Understand what assets you have, and how to protect them
    - **physical security controls**: such as perimeter security and environmental controls
        - control access and the environment
    - **logical access controls**: technical controls used to protect access to information, systems, devices, and applications
        - includes authentication, authorization, and permissions
        - permissions help ensure only authorized entities can access data
        - logical controls restrict access to config settings on systems/networks to only authed individuals
        - applies to on-prem and cloud

[5.2](#5.2) Manage identification and authentication of people, devices, and services (OSG-9 Chpt 13)
- **Identification**: the process of a subject claiming, or professing an identity
- **Authentication**: verifies the subject’s identity by comparing one or more factors against a database of valid identities, such as user accounts
    - a core principle with authentication is that all subjects must have unique identities
    - identification and authentication occur together as a single two-step process
    - users identify themselves with usernames and authenticate (or prove their identity) with passwords
- 5.2.1 Identiy management (IdM) implementation
    - Identity and access management is a collection of processes and techologies that are used to control access to critical assets; it's purpose is the management of access to information, systems, devices, and facilities
    - Identity Management (IdM) implementation techniques generally fall into two categories:
        - **centralized access control**: implies a single entity within a system performs all authorization verification
            - potentially creates a single point of failure
            - small team can manage initially, and can scale to more users
        - **decentralized access control**: (AKA distributed access control) implies several entities located throughout a system perform auth verification
            - requires more individuals or teams to manage, and admin may be spred across numerous locations
            - difficult to maintain consistency
            - changes made to any individual access control point needs to be repeated at others
    - With ubiquitious mobile computing and anywhere, anytime access (to apps & data), identity is the "new perimeter"

- 5.2.2 Single/Multi-Factor Authentication (MFA)
- 5.2.3 Accountability
- 5.2.4 Session management
- 5.2.5 Registration, proofing, and establishment of identity
- 5.2.6 Federated Identity Management (FIM)
    - Federated Identity Management (FIM) systems (a form of SSO) are often used by cloud-based apps
    - A federated identity links a user’s identity in one system with multiple identity management systems
    - FIM allows multiple orgs to join a federation or group, agreeing to share identity information
        - users in each org can log in once in their own org, and their credentials are matched with a federated identity
        - users can then use this federated identity to access resources in any other org within the group
        - where each organization decides what resources to share
    - Methods used to implement federated identity management systems include:
        - Security Assertion Markup Language (SAML)
        - OAuth
        - OpenID Connect (OIDC)
    - Cloud-based federation typically uses a third-party service to share federated identities
    - Federated identity management systems can be hosted on-premises, in the cloud, or in a combination of the two as a hybrid system
- 5.2.7 Credential management systems
- 5.2.8 Singe Sign On (SSO)
    - **Single Sign-On (SSO)**: a centralized access control technique allowing a subject to be authenticated once on a system and access multiple resources without authenticating again
    - Advantages of using SSO include:
        - reduces the number of passwords that users need to remember, and they are less likely to write them down
        - eases administration by reducing the number of accounts
    - Disadvantages:
        - once an account is compromised, an attacker gains unrestricted access to all of the authorized resources
    - Within an organization, a central access control system, such as a directory service, is often used for SSO
        - **directory service**: a centralized database that includes information about subjects and objects, including authentication data
        - many directory services are based on the Lightweight Directory Access Protocol (LDAP)
        
- 5.2.9 Just-In_time (JIT)

[5.3](#5.3) Federated Identity with a third-party service (OSG-9 Chpt 13)

[5.4](#5.4) Implement and manage authorization mechanisms (OSG-9 Chpt 14)

[5.5](#5.5) Manage the identity and access provisioning lifecycle (OSG-9 Chpts 13,14)

[5.6](#5.6) Implement authentication systems (OSG-9 Chpt 14)
