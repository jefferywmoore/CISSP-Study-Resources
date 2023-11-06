[Domain 5](#domain5-top) **Identity and Access Management (IAM)**

The identity and Access Management (IAM) domain focuses on issues related to granting and revoking privileges to access data or perform actions on systems
- Assets include information, systems, devices, facilities, and applications
- Organizations use both physical and logical access controls to protect them
- Identification is the process of a subject claiming, or professing, an identity
- Authentication verifies the subject’s identity by comparing one or more authentication factors against a database holding authentication info for users
- The three primary authentication factors are something you know, something you have, and something you are
- Single sign-on (SSO) technologies allow users to authenticate once and access any resources in a network or the cloud, without authenticating again
- Federated identity management (FIM) systems link user identities in one system with other systems to implement SSO

[5.1](#5.1) Control physical and logical access to assets (OSG-9 Chpts 13)
- controlling access to assets (tangible: things you can touch, or nontangible: info and data) is a central theme of security
- In addition to personnel, assets can be information, systems, devices, facilities, or applications:
    - 5.1.1 Information: an org’s information includes all of its data, stored in simple files (on servers, computers, and small devices, or in databases)
    - 5.1.2 Systems: an org’s systems include anything that provide one or more services; a web server with a database is a system; permissions assigned to user and system accounts control system access
    - 5.1.3 Devices: refers to any computing system (routers & switches to smartphones, laptops, and printers); BYOD has been increasingly adopted, and the data stored on the devices is still an asset to the org
    - 5.1.4 Facilities: any physical location, building, rooms, complexes etc; physical security controls are important to help protect facilities
    - 5.1.5 Applications: apps provide access to data; permissions are an easy way to restrict logical access to apps
- Understand what assets you have, and how to protect them
    - **physical security controls**: such as perimeter security and environmental controls
        - control access and the environment
    - **local access controls**: technical controls used to protect access to information, systems, devices, and applications
        - includes authentication, authorization, and permissions
        - permissions help ensure only authorized entities can access data
        - logical controls restrict access to config settings on systems/networks to only authed individuals
        - applies to on-prem and cloud

[5.2](#5.2) Manage identification and authentication of people, devices, and services (OSG-9 Chpts 13)
- 5.2.1 Identiy management (IdM) implementation

- 5.2.2 Single/Multi-Factor Authentication (MFA)
- 5.2.3 Accountability
- 5.2.4 Session management
- 5.2.5 Registration, proofing, and establishment of identity
- 5.2.6 Federated Identity Management (FIM)
- 5.2.7 Credential management systems
- 5.2.8 Singe Sign On (SSO)
- 5.2.9 Just-In_time (JIT)

[5.3](#5.3) Federated Identity with a third-party service (OSG-9 Chpts 13)

[5.4](#5.4) Implement and manage authorization mechanisms (OSG-9 Chpts 14)

[5.5](#5.5) Manage the identity and access provisioning lifecycle (OSG-9 Chpts 13,14)

[5.6](#5.6) Implement authentication systems (OSG-9 Chpts 14)
