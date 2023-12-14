[Domain 5](#domain5-top) **Identity and Access Management (IAM)**

[5.1](#5.1) Control physical and logical access to assets

### Access Control Concepts
- **What is access control?**  
  Access control is the process of determining who or what has access to a system, network, data, or application. It can be implemented in a variety of ways, but the goal is always to protect sensitive resources from unauthorized access.  Access control is important because it can help to protect organizations from a variety of security threats, including:
    - Data breaches: Data breaches can occur when unauthorized individuals gain access to sensitive data, such as customer records, financial information, or intellectual property. Access control can help to prevent data breaches by restricting access to sensitive data to authorized individuals.
    - Malware infections: Malware infections can occur when users download or open malicious attachments or visit malicious websites. Access control can help to prevent malware infections by restricting users' ability to download and open files from untrusted sources.
- **Types of access control**
  - Physical access control: Controls who can enter or exit a physical location.
  - Logical access control: Controls who can access electronic systems, networks, data, and applications.
- **Access control models**
  - Discretionary access control (DAC): Allows users to control access to their own resources.
  - Mandatory access control (MAC): Enforces a security policy that restricts access to resources based on the sensitivity of the data.
  - Role-based access control (RBAC): Grants users access to resources based on their roles and responsibilities.
- **Access control best practices**
  - Principle of least privilege: Grant users the least amount of access necessary to perform their job duties.
  - Separation of duties: Assign different users different tasks so that no one user has too much control over critical systems or data.
  - Need to know: Only grant users access to resources that they need to know about in order to perform their job duties.

### Physical Access Control
- **Physical access control methods**
  - Locks: Physical devices that prevent unauthorized access to a physical location.
  - Access control systems: Electronic systems that control who can enter or exit a physical location.
  - Security guards: Personnel who are responsible for monitoring and controlling access to a physical location.
  - Biometric scanners: Electronic devices that identify individuals based on their unique physical characteristics, such as fingerprints or facial features.
- **Physical access control best practices**
  - Conduct regular security assessments: Identify and mitigate physical security vulnerabilities.
  - Implement strong perimeter security: Make it difficult for unauthorized individuals to access your premises.
  - Use layered security controls: Implement multiple physical security controls to provide defense in depth.
  - Educate employees on security procedures: Train employees on how to identify and report suspicious activity.

### Logical Access Control
- **Logical access control methods**
  - Usernames and passwords: The most common method of logical access control, which requires users to enter a unique username and password to gain access to a system or application.
  - Multi-factor authentication (MFA): A security measure that requires users to provide two or more factors of authentication to verify their identity.
  - Single sign-on (SSO): A system that allows users to log in to multiple systems and applications with a single set of credentials.
  - Access control lists (ACLs): Lists that define who has access to what resources.
- **Logical access control best practices**
  - Use strong passwords: Passwords should be at least 12 characters long and include a mix of upper and lowercase letters, numbers, and symbols.
  - Implement MFA: MFA is the most effective way to prevent unauthorized access to systems and applications.
  - Use role-based access control: RBAC helps to reduce the risk of human error and misuse of access privileges.
  - Monitor user activity: Monitor user activity to detect and respond to suspicious activity promptly.

### Identity and Access Management (IAM)
- **IAM concepts**
  - Identity: The unique attributes of an individual or object that distinguish it from others.
  - Access: The ability to use a resource.
  - Authentication: The process of verifying the identity of a user or device.
  - Authorization: The process of determining whether a user or device has permission to access a resource.
- **IAM technologies**
  - Identity directories: Databases that store user identity information, such as usernames, passwords, and contact information.
  - Access management systems: Systems that control who has access to what resources.
  - Identity as a service (IDaaS): Cloud-based IAM solutions.
- **IAM best practices**
  - Use a centralized identity management system: This makes it easier to manage user identities and access privileges.
  - Automate user provisioning and deprovisioning: This helps to ensure that users only have access to the resources they need for their current job duties. Additionally, automation can help to reduce the risk of human error, such as forgetting to remove a user account after an employee leaves the company.
  - Implement strong authentication and authorization controls: Strong authentication and authorization controls are essential for preventing unauthorized access to systems and applications. Authentication controls verify the identity of a user, while authorization controls determine whether a user has permission to access a resource. Some common authentication and authorization controls include passwords, multi-factor authentication, and role-based access control.
  - Monitor user activity: Monitoring user activity can help to detect and respond to suspicious activity promptly. This can help to prevent unauthorized access to systems and applications, as well as data breaches and malware infections. Some common user activity monitoring tools include security information and event management (SIEM) systems and intrusion detection systems (IDS).

### Access Control Attacks
- **Common access control attacks**
  - Brute force attacks: Attacks that attempt to crack passwords by trying all possible combinations of characters.
  - Password spraying attacks: Attacks that attempt to crack passwords by trying common passwords against a large number of user accounts.
  - Phishing attacks: Attacks that attempt to trick users into revealing their passwords or other sensitive information.
  - Man-in-the-middle attacks: Attacks that intercept communications between two parties in order to steal data or impersonate one of the parties. Common techniques include:
     - Wi-Fi sniffing: Wi-Fi sniffing is the process of capturing data that is being transmitted over a wireless network. Attackers can use Wi-Fi sniffing to steal sensitive data, such as passwords and credit card numbers if they are not using TLS or some other upper layer encryption.
     - ARP poisoning: ARP poisoning is a type of attack where the attacker sends fake ARP messages to a network device. This can trick the network device into sending traffic to the attacker's machine instead of the intended destination.
     - SSL stripping: SSL stripping is a type of attack where the attacker forces a website to use an unencrypted connection. This can allow the attacker to intercept and steal sensitive data, such as passwords and credit card numbers.
- **Defending against access control attacks**
  - Use strong passwords and MFA: Strong passwords and MFA are the most effective way to defend against access control attacks.
  - Educate employees on security awareness: Train employees on how to identify and report suspicious activity, such as phishing emails and unknown attachments.
  - Protect data in transit: Always use encrypted protocols such as HTTPS/SSH, even with internal network communication.

[5.2](#5.2) Manage identification and authentication of people, devices, and services
### Introduction

- **What is identity and access management (IAM)?** IAM is the process of managing the digital identities of people, devices, and services, and their access to systems and resources. IAM helps organizations to protect their assets from unauthorized access.
- **Why is IAM important?** IAM is important because it helps organizations to reduce the risk of data breaches, malware infections, and other security incidents.
- **The IAM lifecycle:** The IAM lifecycle consists of four phases: 
    - Provisioning: involves creating and configuring user accounts and assigning them the necessary permissions.
    - Authentication: involves verifying the identity of users, devices, and services.
    - Authorization: involves determining which users, devices, and services are allowed to access specific systems and resources.
    - Deprovisioning: involves removing user accounts and permissions when they are no longer needed.
- **Different types of IAM systems and solutions:** 
    - On-premises: hosted and managed by the organization.
    - Cloud-based: hosted and managed by a third-party provider.
    - Hybrid solutions: combine elements of on-premises and cloud-based IAM systems.

### Identification

- **What is identification?** Identification is the process of claiming an identity through the use of some identifier relevant to the system.
- **Different types of identifiers** Identifiers can be:
    - Unique (e.g., social security number, passport number). Unique identifiers are more reliable for identification purposes, but they may be more difficult to use and manage.
    - Non-unique (e.g., username, email address). Non-unique identifiers are easier to use and manage, but they can be more easily spoofed.
- **Common identification methods and factors** Common identification methods and factors include:
    - Username or User ID: Users provide a unique username or user ID associated with their account to identify themselves.
    - Email Address: Users can use their email addresses as a form of identification. Email addresses are unique to each user and are commonly used in online services.
    - One-time passwords (OTPs): a unique password that is only valid for a single use. Often generated by or sent to another account verified to be owned by the subject.
    - Biometric authentication: a method of authentication that uses unique physical characteristics of a user, such as fingerprints, facial features, or iris patterns.
    - Certificates: digital documents that bind a public key to an identity, aka PKI.
    - Security Questions: Users answer security questions that are unique to them and known only to the user. Correct answers identify the user.
- **Identity proofing and assurance** Identity proofing and assurance is the process of verifying the identity of a person with a high degree of certainty. This is often done using a combination of different identification methods and factors. For example, a bank may require customers to provide a government-issued ID and a selfie in order to open an account.

### Authentication

- **What is authentication?** Authentication is the process of verifying that a person, device, or service is who or what it claims to be.
- **Different types of authentication factors** Authentication factors can be categorized into three types: 
    - Knowledge factors (e.g., passwords, PINs)
    - Possession factors (e.g., tokens, smart cards)
    - Inherence factors (e.g., biometrics).
- **Authentication mechanisms and protocols:** the methods used to verify the identity of a person, device, or service. Some common authentication mechanisms and protocols include passwords, OTPs, biometric authentication, and certificates.
- **Multi-factor authentication (MFA):** a security measure that requires the use of two or more authentication factors to verify the identity of a user. MFA helps to protect against unauthorized access, even if an attacker has compromised one authentication factor.
- **Risk-based authentication:** a security measure that adapts the authentication process to the level of risk associated with the login attempt. For example, a user may be required to provide additional authentication factors if they are logging in from a new device or from an unusual location.

### Authentication for Devices and Services

- **Device identification and authentication:** the process of verifying the identity of a device. This can be done using a variety of methods, such as MAC addresses, device certificates, and device fingerprinting.
- **Service authentication:** the process of verifying the identity of a service. This can be done using a variety of methods, such as client certificates and service tokens.
- **Machine-to-machine (M2M) authentication:** the process of authenticating devices and services that communicate with each other without human intervention. This is often done using certificates and tokens.

### Identity and Access Management Best Practices

- **Least privilege:** The principle of least privilege states that users should only be granted the access they need to perform their job duties.
- **Separation of duties:** Separation of duties is a security principle that states that no single user should have the ability to perform all of the steps necessary to complete a sensitive task. This helps to prevent fraud and abuse.
- **Password management:** Password management is the process of creating and managing strong passwords for all of your online accounts. Strong passwords are at least 12 characters long and include a mix of upper and lowercase letters, numbers, and symbols. It is important to never reuse passwords across different accounts.
- **Account monitoring and auditing:** Account monitoring and auditing is the process of tracking and reviewing user activity to detect suspicious activity. This can be done using a variety of methods, such as logging, intrusion detection systems, and security information and event management (SIEM) systems.
- **Security awareness and training:** Security awareness and training is the process of educating employees about security best practices and how to identify and report suspicious activity. This helps to reduce the risk of human error and social engineering attacks.

### Emerging Trends in IAM

- **Cloud-based IAM:** a type of IAM solution that is hosted in the cloud. This type of solution is often more scalable and cost-effective than on-premises IAM solutions.
- **Identity as a service (IDaaS):** a type of cloud-based IAM solution that provides organizations with a single place to manage the identities and access of their users, devices, and services. IDaaS solutions can help to simplify IAM administration and reduce costs.
- **Zero trust security:** a security model that assumes that no user or device can be trusted by default. In a zero trust environment, all users and devices must be authenticated and authorized before they can access any systems or resources. Zero trust security can help to protect organizations from a variety of cyber threats, including data breaches, malware infections, and ransomware attacks.

[5.3](#5.3) Federated Identity with a third-party service
### Introduction

- **Federated identity:** a framework that allows users to access multiple applications and services using a single set of credentials. Federated identity is based on the concept of trust between the user's identity provider (IdP) and the service provider (SP). The IdP authenticates the user and provides the SP with the necessary attributes to authorize access to the service. Federated Identity streamlines authentication processes, promotes seamless user access across systems, and ensures secure data exchange between entities.
- **Benefits:**
  - Improved user experience: Users do not have to remember and manage multiple sets of credentials.
  - Reduced security risks: Federated identity can help to reduce the risk of password breaches and other security vulnerabilities.
  - Increased compliance: Federated identity can help organizations to comply with various regulations that require strong authentication and authorization.
- **Challenges:**
  - Complexity: Federated identity can be complex to implement and manage, especially for large organizations with multiple applications.
  - Security risks: If there is a breach of the identity provider (IdP), it could give attackers access to all of the applications that the IdP federates with.
  - Cost: Implementing and managing federated identity can be expensive, especially if you need to use a third-party IdP.

### Types of federated identity

- **SAML:** SAML (Security Assertion Markup Language) is a standard for federated identity that is widely used by enterprises. SAML uses XML tokens to exchange authentication and authorization information between the IdP and the service provider (SP).
- **OpenID Connect:** OpenID Connect is a newer standard for federated identity that is built on top of OAuth 2.0. OpenID Connect is designed to be more user-friendly and easier to implement than SAML.
- **OAuth 2.0:** OAuth 2.0 is a standard for authorization that is often used in conjunction with federated identity. OAuth 2.0 allows users to authorize applications to access their data on other websites and services.

### Implementing federated identity with a third-party service

- **Choosing a third-party identity provider (IdP):** When choosing a third-party IdP, you should consider the following factors:
    - Features: Does the IdP support the features that you need, such as SAML, OpenID Connect, and OAuth 2.0?
    - Security: Does the IdP have a good security track record?
    - Scalability: Can the IdP handle the number of users and applications that you need to support?
    - Cost: How much does the IdP charge?
- **Configuring the IdP:** Once you have chosen an IdP, you need to configure it to work with your applications. This typically involves creating an account with the IdP and then configuring your applications to trust the IdP. Most IdPs support SAML, OpenID Connect, and OAuth 2.0.
- **Configuring the service provider (SP):** You need to configure your SP to trust the IdP. This typically involves adding the IdP's metadata to the SP. The IdP's metadata is a file that contains information about the IdP, such as its name, URL, and certificates.
- **Testing the federated identity implementation:** Once you have configured the IdP and the SP, you need to test the federated identity implementation to make sure that it is working correctly. This can be done by trying to log in to your SP using your IdP credentials.

### Security considerations for federated identity

- **Single point of failure:** If the IdP is compromised, it could give attackers access to all of the applications that the IdP federates with. This is known as a single point of failure.
- **Identity theft:** If an attacker can steal a user's federated identity credentials, they could use those credentials to log in to any of the applications that the user has federated access to.
- **Data breaches:** If there is a data breach at the IdP, attackers could gain access to the personal information of all of the IdP's users.

### Best practices for federated identity

- **Use strong authentication and authorization:** You should use strong authentication and authorization controls to protect your federated identity implementation. This could include using multi-factor authentication (MFA) and access control lists (ACLs).
- **Monitor the federated identity implementation:** You should monitor your federated identity implementation for suspicious activity. This could involve monitoring the IdP logs and the application logs.
- **Educate users about federated identity:** You should educate your users about federated identity and how to use it safely. This could involve providing training on how to create strong passwords and how to identify phishing attacks.



[5.4](#5.4) Implement and manage authorization mechanisms
### Key Concepts

- **Authorization mechanisms:** The processes and technologies used to determine what resources a user or process is allowed to access. Authorization mechanisms are essential for protecting organizations from unauthorized access to their resources and can be implemented with a variety of technologies, including Identity and access management (IAM) systems, Web application firewalls (WAFs), and API gateways.
- **Access control models:** A conceptual framework for defining and implementing authorization policies. Access control models specify how to determine who has access to what resources and under what conditions. There are a variety of access control models available, each with its own strengths and weaknesses.
- **Role-based access control (RBAC):** An access control model in which users are assigned to roles, and roles are granted permissions to access resources. RBAC is a popular access control model that is relatively easy to implement and manage. RBAC is based on the principle of least privilege, which means that users are only granted the permissions they need to perform their job duties.
- **Rule-based access control (RBAC):** An access control model in which users are granted permissions to access resources based on predefined rules. R(ule)BAC is another popular access control model that is more flexible than R(ole)BAC. RBAC allows for more granular permissions to be granted, and it can be used to implement complex access control policies.
- **Discretionary access control (DAC):** An access control model in which the owner of a resource has the discretion to grant or deny access to other users. DAC is a simple access control model that is often used for personal file systems. However, DAC can be difficult to manage in enterprise environments.
- **Mandatory access control (MAC):** An access control model in which the system enforces access control policies based on security labels assigned to users and resources. MAC is a more secure access control model than DAC. MAC is often used in government and military environments where high levels of security are required.
- **Attribute-based access control (ABAC):** An access control model in which access decisions are made based on user attributes, such as role, department, and location. ABAC is a more flexible access control model than RBAC or MAC. ABAC allows for access decisions to be made based on a variety of user attributes, which can be useful for implementing complex access control policies.
- **Context-aware access control (C-AAC):** An emerging access control model that takes into account contextual factors, such as the time of day, the user's location, and the device being used, when making access decisions. C-AAC can be used to improve the security of organizations by reducing the risk of unauthorized access to resources.
- **Zero trust:** A security model that assumes that no user or device can be trusted by default. Instead, users and devices must be authenticated and authorized before being granted access to resources. Zero trust is a relatively new security model, but it is gaining popularity as organizations become more aware of the risks of cyberattacks.
    - Continuous verification: Users and devices must be continuously verified before being granted access to resources.
    - Least privilege: Users and devices should only be granted the permissions they need to perform their job duties.
    - Microsegmentation: The network should be segmented into small microsegments, and access to each microsegment should be restricted.
    - Assume breach: Organizations should assume that they have already been breached and design their security architecture accordingly.

### Authorization Mechanisms

- **Authentication vs. authorization:** Authentication is the process of verifying the identity of a user or process. Authorization is the process of determining what resources a user or process is allowed to access. Authentication is the first step in any access control system. Once a user or process has been authenticated, the authorization system can determine what resources they are allowed to access.
- **Authorization methods:** There are a variety of authorization methods available, including role-based access control, attribute-based access control, and context-aware access control. The different authorization methods available offer different levels of flexibility and security. For example, role-based access control is a relatively simple authorization method to implement and manage, but it is not as flexible as attribute-based access control.
- **Authorization policies:** Authorization policies define the rules that govern who has access to what resources and are essential for defining and implementing authorization controls. Authorization policies should be based on the organization's risk tolerance and security requirements. For example, an authorization policy might state that all employees must be authenticated using a multi-factor authentication (MFA) solution before they can access the company's network.
- **Authorization rules:** Authorization rules are specific statements that are used to implement authorization policies. Authorization rules typically specify the following:
    - The resource(s) that the rule applies to
    - The users or groups of users that the rule applies to
    - The permissions that are granted or denied by the rule
- **Authorization decision-making:** The process of determining whether to grant or deny access to a resource based on an authorization policy. Authorization decision-making is typically performed by an authorization decision engine (ADE). ADEs evaluate authorization policies and rules to determine whether a user or process has the necessary permissions to access a resource.
- **Authorization enforcement:** The process of implementing authorization decisions. Authorization enforcement is typically performed by an authorization enforcement point (AEP). AEPs prevent users and processes from accessing resources that they are not authorized to access. For example, an AEP might prevent a user from logging into the company's network if they do not have a valid MFA token.

### Access Control Models

- **RBAC:** Role-based access control (RBAC) is an access control model in which users are assigned to roles, and roles are granted permissions to access resources. RBAC is a relatively easy-to-implement and manage access control model, and it is based on the principle of least privilege, which means that users are only granted the permissions they need to perform their job duties.
    - Example: A company might have a role called "Sales Representative" and a role called "Manager." The Sales Representative role might be granted permission to access the company's CRM system, while the Manager role might be granted permission to access the company's financial system.
- **ABAC:** Attribute-based access control (ABAC) is an access control model in which access decisions are made based on user attributes, such as role, department, and location. ABAC is a more flexible access control model than RBAC, but it can be more difficult to implement and manage.
    - Example: A company might use ABAC to allow employees to access files based on their job title and department. For example, an employee in the Sales department might be granted permission to access all files related to sales, while an employee in the Marketing department might be granted permission to access all files related to marketing.
- **C-AAC:** Context-aware access control (C-AAC) is an emerging access control model that takes into account contextual factors, such as the time of day, the user's location, and the device being used, when making access decisions. C-AAC can be used to improve the security of organizations by reducing the risk of unauthorized access to resources.
    - Example: A company might use C-AAC to prevent employees from accessing sensitive files when they are outside of the office.
- **Zero trust:** Zero trust is a security model that assumes that no user or device can be trusted by default. Instead, users and devices must be authenticated and authorized before being granted access to resources. Zero trust is a relatively new security model, but it is gaining popularity as organizations become more aware of the risks of cyberattacks.
    - Example: A company might use zero trust to require employees to authenticate themselves using a multi-factor authentication (MFA) solution before they can access a resource on the company's network.

### Implementing Authorization Mechanisms

1. **Define and document authorization requireme**nts. This includes identifying the resources that need to be protected, the users and groups of users who need access to those resources, and the permissions that need to be granted.
1. **Select an appropriate access control model.** The best access control model for an organization will depend on its specific needs and requirements.
1. **Design authorization policies and rules.** Authorization policies define the high-level rules that govern who has access to what resources. Authorization rules are specific statements that implement authorization policies.
1. **Implement authorization mechanisms in IAM systems or applications.** Most IAM systems and applications have built-in authorization mechanisms. To implement authorization mechanisms, you will need to create roles and assign users to roles. You will also need to define permissions and grant permissions to roles.
1. **Test and validate authorization mechanisms.** Once you have implemented authorization mechanisms, it is important to test and validate them to ensure that they are working as expected.
1. **Monitor and audit authorization mechanisms.** It is also important to monitor and audit authorization mechanisms to identify any unauthorized access or suspicious activity.

### Managing Authorization Mechanisms

- **Monitoring authorization mechanisms:** It is important to monitor authorization mechanisms to ensure that they are working properly and that they are not being abused. You can monitor authorization mechanisms by tracking user access logs and auditing authorization events.
- **Auditing authorization mechanisms:** Auditing authorization mechanisms is the process of reviewing authorization logs and reports to identify suspicious activity. Auditing can help you to identify unauthorized access to resources and to detect security breaches.
- **Tuning authorization mechanisms:** It is important to tune authorization mechanisms regularly to ensure that they are meeting the organization's security requirements. You can tune authorization mechanisms by adjusting permissions and roles.
 
### Best Practices for Authorization

- **Principle of least privilege:** The principle of least privilege states that users should only be granted the permissions they need to perform their job duties.
- **Separation of duties:** Separation of duties is a security principle that states that no single user should have the ability to perform all of the steps necessary to complete a sensitive task.
- **Need-to-know:** Need-to-know is a security principle that states that users should only be granted access to the information they need to perform their job duties.
- **Accountability:** Accountability is a security principle that states that users should be held accountable for their actions.


[5.5](#5.5) Manage the identity and access provisioning lifecycle  
The identity and access provisioning lifecycle is the process of creating, managing, and terminating user accounts and their access to systems and resources. It is a critical component of IAM, as it ensures that only authorized users have access to the information and systems they need to perform their jobs.

### Introduction

- **What is the identity and access provisioning lifecycle?** The identity and access provisioning lifecycle is the process of creating, managing, and terminating user accounts and their access to systems and resources. It includes the following steps:
    1. Identity provisioning: Creating new user accounts and assigning them to roles and groups.
    1. Identity management: Maintaining user accounts and their access to systems and resources.
    1. Identity revocation: Terminating user accounts and revoking their access to systems and resources.
- **Why is it important?** The identity and access provisioning lifecycle is important because it helps to ensure that only authorized users have access to the information and systems they need to perform their jobs. It also helps to protect organizations from unauthorized access, fraud, and abuse.

### Identity Provisioning

- **Creating new user accounts**: When creating new user accounts, it is important to collect the necessary account attributes, such as the user's name, email address, and job title. It is also important to set strong password requirements and to activate the account before granting the user access to systems and resources.
- **Assigning users to roles and groups:** Roles and groups are used to manage user access to systems and resources. Roles define the permissions that a user has, while groups are collections of users who share the same permissions. By assigning users to roles and groups, organizations can easily manage user access without having to grant permissions individually.
- **Granting users access to systems and resources**: Once a user has been assigned to a role or group, they can be granted access to the systems and resources they need to perform their jobs. This can be done through access control lists (ACLs), file permissions, or network permissions.

### Identity Management

- **Maintaining user accounts:** It is important to regularly maintain user accounts to ensure that they are accurate and up-to-date. This includes updating account status changes, such as when a user leaves the organization, and resetting passwords when necessary.
- **Updating user roles and groups:** When a user's job duties change or the organizational structure changes, it is important to update the user's roles and groups accordingly. This will ensure that the user has the necessary access to perform their job and that they do not have access to systems and resources that they no longer need.
- **Managing user access to systems and resources:** As users move around the organization and their job duties change, it is important to manage their access to systems and resources accordingly. This includes adding and removing access to systems and resources, as well as monitoring user access to identify any suspicious activity.

### Identity Revocation

- **Terminating user accounts:** When a user leaves the organization, it is important to terminate their account. This will disable the account and prevent the user from accessing systems and resources.
- **Removing users from roles and groups:** When a user's job duties change or they leave the organization, it is important to remove them from the roles and groups to which they are assigned. This will ensure that they no longer have access to systems and resources that they do not need.
- **Revoking user access to systems and resources:** It is important to revoke a user's access to systems and resources when they leave the organization or when their job duties change. This can be done by disabling accounts, changing passwords, or removing access permissions.

### Best Practices

- **Use a centralized identity management system:** A centralized identity management system allows organizations to manage all of their user accounts and access permissions from a single location. This makes it easier to manage user access and to ensure that all user accounts are properly provisioned and deprovisioned.
- **Automate the identity provisioning process:** Automating the identity provisioning process can help to reduce the risk of human error and to streamline the process of creating, maintaining, and terminating user accounts.
- **Implement role-based access control (RBAC):** RBAC is a method of access control that assigns users to roles and then grants permissions to those roles. This makes it easy to manage user access and to ensure that users only have the access they need to perform their jobs.
- **Conduct regular access reviews:** Regular access reviews help to ensure that users only have the access they need and that they are not hoarding access to systems and resources.
- **Use strong authentication and authorization mechanisms:** Strong authentication and authorization mechanisms help to protect user accounts from unauthorized access. Examples of strong authentication and authorization mechanisms include multi-factor authentication (MFA) and single sign-on (SSO).


[5.6](#5.6) Implement authentication systems

### Introduction

- **What is authentication?** Authentication is the process of verifying the identity of a user or device. It is the first step in the access control process, and it is essential for protecting systems and data from unauthorized access.
- **Types of authentication factors:** Authentication factors can be divided into three categories:
    - Knowledge factors: These factors are based on something that the user knows, such as a password or PIN.
    - Possession factors: These factors are based on something that the user has, such as a security token or smart card.
    - Inherence factors: These factors are based on something that the user is, such as a fingerprint or facial scan.
- **Authentication methods:** Authentication methods are the specific techniques that are used to verify authentication factors. Some common authentication methods include:
    - Password-based authentication: Password-based authentication is the most common authentication method. It involves the user entering a password into a system in order to gain access.
    - Knowledge-based authentication: Knowledge-based authentication involves the user answering a series of questions that only they should know the answers to.
    - Biometric authentication: Biometric authentication involves using a unique physical characteristic of the user, such as their fingerprint or facial scan, to verify their identity.
    - Token-based authentication: Token-based authentication involves the user using a physical token, such as a security token or smart card, to verify their identity.
- **Authentication protocols:** Authentication protocols are the set of rules and procedures that are used to implement authentication methods. Some common authentication protocols include:
    - RADIUS (Remote Authentication Dial-In User Service): RADIUS is a widely used authentication protocol that is used to authenticate users connecting to remote networks.
    - TACACS+ (Terminal Access Controller Access-Control System Plus): TACACS+ is a similar authentication protocol to RADIUS, but it is more secure and offers additional features.
    - LDAP (Lightweight Directory Access Protocol): LDAP is a directory access protocol that can be used for authentication purposes.
    - SAML (Security Assertion Markup Language): SAML is a standard XML-based markup language that can be used to exchange authentication and authorization information between different systems.

### Authentication Factors

- **Single-factor authentication (SFA):** SFA is the simplest type of authentication, and it involves using only one authentication factor to verify the identity of a user. SFA is the least secure type of authentication, and it should only be used for low-risk applications.
- **Two-factor authentication (2FA):** 2FA is more secure than SFA because it requires the user to provide two authentication factors in order to gain access. 2FA is a good choice for most applications, and it is especially important for applications that contain sensitive data.
- **Multi-factor authentication (MFA):** MFA is the most secure type of authentication, and it requires the user to provide three or more authentication factors in order to gain access. MFA is the best choice for applications that contain highly sensitive data or that are at high risk of attack.

### Authentication Methods

- **Password-based authentication:** Password-based authentication is the most common authentication method, but it is also the least secure. Passwords can be easily guessed or stolen, so it is important to use strong passwords and to change them regularly.
- **Knowledge-based authentication:** Knowledge-based authentication is more secure than password-based authentication, but it can be inconvenient for users to remember a large number of questions and answers.
- **Biometric authentication:** Biometric authentication is the most convenient type of authentication, but it can be expensive to implement and it can be vulnerable to certain types of attacks.
- **Token-based authentication:** Token-based authentication is a good balance between security and convenience. Tokens are relatively inexpensive to implement, and they are difficult to steal or forge.

### Authentication Protocols

- **RADIUS (Remote Authentication Dial-In User Service):** a widely used authentication protocol that is used to authenticate users connecting to remote networks, such as VPNs and wireless networks. RADIUS is a client-server protocol, where the client is the device that the user is using to connect to the network and the server is the RADIUS server. The RADIUS server is responsible for verifying the identity of the user and granting them access to the network. RADIUS is a relatively simple protocol, but it is effective and secure. RADIUS uses a variety of security features, such as encryption and authentication, to protect user credentials and prevent unauthorized access.
- **TACACS+ (Terminal Access Controller Access-Control System Plus):** a similar authentication protocol to RADIUS, but it is more secure and offers additional features, such as support for multiple authentication methods and fine-grained authorization. TACACS+ is often used in high-security environments, such as financial institutions and government agencies.
- **LDAP (Lightweight Directory Access Protocol):** a directory access protocol that can be used for authentication purposes. LDAP is a powerful and flexible protocol, but it can be more complex to configure and manage than RADIUS or TACACS+. LDAP is often used in large organizations with complex directory structures.
- **SAML (Security Assertion Markup Language):** an XML-based markup language that can be used to exchange authentication and authorization information between different systems. SAML is a powerful and flexible protocol, but it can be more complex to configure and manage than RADIUS or TACACS+. SAML is often used in single sign-on (SSO) solutions.
- **Choosing an authentication protocol:** The best authentication protocol for your organization will depend on a number of factors, such as the type of network you are using, the security requirements of your organization, and your budget.


| Protocol | Features | Benefits | Drawbacks |
|----------|----------|----------|-----------|
|RADIUS	| Simple | Widely used | May not be secure enough for high-security environments |
|TACACS+|Secure|Supports multiple authentication methods and fine-grained authorization|More complex to configure and manage than RADIUS|
|LDAP|Powerful and flexible|Can be used to authenticate users from different systems|More complex to configure and manage than RADIUS or TACACS+|
|SAML|Powerful and flexible|Can be used to implement SSO|More complex to configure and manage than RADIUS or TACACS+|

### Single Sign-On (SSO)

- **What is SSO?** SSO is a technology that allows users to log in once and gain access to multiple applications without having to enter their credentials again. SSO is a convenient and secure way to manage access to applications, and it can help to reduce the number of passwords that users have to manage.
- **Benefits of SSO:** SSO offers a number of benefits, including:
    - Reduced user workload: SSO eliminates the need for users to enter their credentials multiple times, which can save them time and frustration.
    - Improved security: SSO can help to improve security by reducing the number of passwords that are in circulation and by making it easier to manage and audit user access.
    - Increased compliance: SSO can help organizations to comply with regulations that require strong authentication and access control.
- **Types of SSO solutions:** There are two main types of SSO solutions:
    - Web-based SSO: Web-based SSO solutions use a central server to authenticate users and then redirect them to the applications that they want to access.
    - Kerberos-based SSO: Kerberos-based SSO solutions use Kerberos tickets to authenticate users and grant them access to applications.
- **Implementing SSO:** There are a number of factors to consider when implementing SSO, such as the type of SSO solution to choose, the applications that need to be integrated, and the budget. It is important to carefully plan and implement SSO to ensure a successful deployment.

### Multi-Factor Authentication (MFA)

- **What is MFA?** MFA is a security measure that requires users to provide two or more authentication factors in order to gain access to an application or system. MFA is more secure than single-factor authentication because it is more difficult for attackers to compromise multiple authentication factors.
- **Benefits of MFA:** MFA offers a number of benefits, including:
    - Increased security: MFA makes it more difficult for attackers to gain access to applications and systems.
    - Reduced risk of fraud: MFA can help to reduce the risk of fraud by making it more difficult for attackers to impersonate legitimate users.
    - Improved compliance: MFA can help organizations to comply with regulations that require strong authentication and access control.
- **Types of MFA factors:** There are a number of different types of MFA factors, including:
    - Knowledge factors: Knowledge factors are based on something that the user knows, such as a password, PIN, or security question. Knowledge factors are the most common type of MFA factor, but they are also the least secure. Passwords can be easily guessed or stolen, and security questions can be answered by someone who knows the user well enough.
    - Possession factors: Possession factors are based on something that the user has, such as a security token, smart card, or smartphone. Possession factors are more secure than knowledge factors because they are more difficult to steal. However, possession factors can be lost or damaged, and they may not be practical for all applications.
    - Inherence factors: Inherence factors are based on something that the user is, such as a fingerprint, facial scan, or voice print. Inherence factors are the most secure type of MFA factor because they are very difficult to forge. However, inherence factors can be more expensive to implement and are used less than other types of MFA factors.
- **Implementing MFA:** There are a number of ways to implement MFA, and the best approach will vary depending on the specific needs of the organization. Some common ways to implement MFA include:
    - Using a cloud-based MFA service: There are a number of cloud-based MFA services available that can be easily implemented and used. For instance: Google Authenticator OTPs, and Microsoft Azure Active Directory Multi-Factor Authentication.
    - Using an on-premises MFA solution: There are also a number of on-premises MFA solutions available that can be deployed and managed by the organization. Examples: YubiKey (hardware tokens) & RSA SecurID (software tokens).
    - Using MFA-enabled applications: Some applications have built-in MFA support, which can be used to implement MFA without having to deploy a separate MFA solution. Examples: Google Workspace & Microsoft 365.

### Authentication for Remote Access

- **VPN authentication:** can be implemented using a variety of methods, including RADIUS, TACACS+, and SAML.
- **Web application authentication:** can be implemented using a variety of methods, including HTTP Basic authentication, HTTP Digest authentication, and SAML.
- **Mobile device authentication:** can be implemented using a variety of methods, including PINs, passwords, and biometrics.

### Authentication for Cloud Computing

- **IaaS authentication:** can be implemented using a variety of methods, including IAM roles, access keys, and SAML.
- **PaaS authentication:** can be implemented using a variety of methods, including IAM roles, OAuth, and SAML.
- **SaaS authentication:** is typically implemented using SAML or OAuth.

### Security Considerations for Authentication Systems

- **Password management:** Passwords are the most common authentication factor, so it is important to implement strong password policies and procedures. Password policies should require users to create strong passwords, change their passwords regularly, and not reuse passwords across multiple accounts.
- **Account lockout policies:** Account lockout policies can help to protect against brute-force attacks by locking accounts that are unsuccessfully logged into too many times.
- **Session management:** Session management is the process of creating, tracking, and terminating user sessions. It is important to implement secure session management practices to prevent session hijacking and other attacks.
- **Authentication auditing:** Authentication auditing is the process of logging and reviewing authentication events. Authentication auditing can help to detect and investigate unauthorized access attempts.


## Key Terms
- **Access Control System:** Means to ensure that access to assets is authorized and restricted based on business and security requirements related to logical and physical systems.
- **Access Control Tokens:** The system decides if access is to be granted of denied based upon the validity of the token for the point where it is read based on time, date, day, holiday or other condition used for controlling validation.
- **Accounting:** Access control process which records information about all attempts by all identities to access and resources of the system. See also authentication, authorization.
- **Attribute-based Access Control (ABAC):** This is an access control paradigm whereby access rights are granted to users with policies that combine attributes together.
- **Authentication:** Access control process that validates the identity being claimed by a user or entity is known to the system, by comparing one or more factors of identification. Factors typically include something the user is (e.g. fingerprint), something they have (e.g. hardware token), and something they know (e.g. password). Single-factor (SFA) authenticates with only one of these; multi-factor (MFA) uses two or more.
- **Authorization:** The process of defining the specific resources a user needs and determining the type of access to those resources the user may have.
- **Crossover Error Rate (CER):** This is the point at which the false acceptance (Type 2) error rate equals the false rejection (Type 1) error rate, for a given sensor used in a given system and context. This is only the optimal point of operation if the potential impacts of both types of errors are equivalent.
- **Data Custodian, Custodian:** The individual who manages permissions and access on a day-to-day basis based on instructions from the data owner. Responsible for protecting an asset that has value, while in the custodian's possession.
- **Data Owner / Data Controller:** The individual or entity who is responsible to classify, categorize and permit access to the data. The data owner is the one who is best familiar with the importance of the data to the business.
- **Data Processor:** Any entity, working on behalf or at the direction of the data controller, that processes personally identifiable information (PII).
- **Discretionary Access Control (DAC):** Access control in which the system owner decides who gets access.
- **Ethical Wall:** The separation of information, assets or job functions to establish and enforce need to know boundaries or prevent conflict of interest situations from arising. The use of administrative, physical and/or logical controls to establish, maintain and monitor such separations. Also known as a compartment.
- **False Acceptance Rate (FAR or Type 2):** Incorrectly authenticating a claimed identity as legitimate and recognized, and granting access on that basis.
- **False Rejection Rate (FRR or Type 1):** Incorrectly denying authentication to a legitimate identity and thus denying it access.
- **Granularity of Controls:** Level of abstraction or detail at which a security function can be configured or tuned for performance and sensitivity purposes.
- **Identity-as-a-Service (IDaaS):** Cloud-based services that broker IAM functions to target systems on customers' premises and/or in the cloud.
- **Identity Proofing:** The process of collecting and verifying information about a person for the purpose of proving that a person who has requested an account, a credential or other special privilege is indeed who the claim to be and establishing a reliable relationship that can be trusted electronically between the individual and said credential for purposes of electronic authentication.
- **Logical Access Control System:** Automated systems that authorize or deny access to and use of and information system and its assets to an individual user, based on verification that the identity presented matches that which was previously approved.
- **Mandatory Access Controls (MAC):** Access control that requires the system itself to manage access controls in accordance with the organization's security policies.
- **Multi-factor Authentication (MFA):** Ensures that a user is who they claim to be. The more factors used to determine a person's identity, the greater the trust of authenticity.
- **Open Authorization (OAuth):** The OAuth 2.0 authorization framework enables a third-party application to obtain limited access to an HTTP service, either on behalf of a resource owner by orchestrating an approval interaction between the resource owner and the HTTP service, or by allowing the third-party application to obtain access on its own behalf.
- **Privilege Creep:** The unnecessary accumulation of access privileges by a user, typically due to failing to remove privileges when they are no longer needed.
- **Self-Service Identity Management:** Elements of the identity management life-cycle and provisioning process, which the end user (the identity in question) can initiate or perform with little or no interaction or assistance from administrators. Examples include password resets, postal address updates or changes to challenge questions and answers.
- **Single-Factor Authentication (SFA):** Involves the use of simply one of the three available factors solely to carry out the authentication process being requested.
- **Whaling Attack:** Phishing attacks that attempt to trick highly placed officials or private individuals with sizable assets into authorizing large fund wire transfers to previously unknown entities.
