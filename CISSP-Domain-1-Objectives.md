[Domain 1](#domain1-top) **Security and Risk Management**

[1.1](#1.1) Understand, adhere to, and promote professional ethics
As a CISSP, you must understand and follow the (ISC)² code of ethics, as well as your organization’s own code.

- (ISC)² Code of Professional Ethics. Take the time to read the code of ethics available at www.isc2.org/Ethics. At a
minimum, know and understand the ethics canons:

  - Protect society, the common good, necessary public trust and confidence, and the infrastructure.
This is “do the right thing.” Put the common good ahead of yourself. Ensure that the public can have faith
in your infrastructure and security.

  - Act honorably, honestly, justly, responsibly, and legally. Always follow the laws. But what if you find
yourself working on a project where conflicting laws from different countries or jurisdictions apply? In such
a case, you should prioritize the local jurisdiction from which you are performing the services.

  - Provide diligent and competent service to principles. Avoid passing yourself as an expert or as qualified
in areas that you aren’t. Maintain and expand your skills to provide competent services.

  - Advance and protect the profession. Don’t bring negative publicity to the profession. Provide competent
services, get training and act honorably. Think of it like this: If you follow the first three canons in the code
of ethics, you automatically comply with this one.

- Organizational code of ethics. You must also support ethics at your organization. This can be interpreted to mean
evangelizing ethics throughout the organization, providing documentation and training around ethics, or looking
for ways to enhance the existing organizational ethics. Some organizations might have slightly different ethics than
others, so be sure to familiarize yourself with your organization’s ethics and guidelines.

[1.2](#1.2) Understand and apply security concepts
- **Confidentiality**:
  - Concept of measures used to ensure the protection of the secrecy of data, objects, and resources
  - Confidentiality protections prevent disclosure while protecting authorized access
  - Preserving authorized restrictions on information access and disclosure, including the means for protecting personal privacy and prioprietary information
  - Sensitive data, including personally identifiable information (PII) must be kept confidential. Confidentiality is different from secrecy
  - Preserving confidentiality means protecting an asset or data, even if it's not a secret
  
- **Integrity**:
  - Concept of protecting the reliability and correctness of data. Integrity protection prevents unauthorized alterations of data
  - Preventing unauthorized subjects from making modifications
  - Preventing authorized subjects from making unauthorized modifications, such as mistakes
  - Maintaining the internal and external consistency of objects

- **Availability**:
  - Authorized subjects are granted timely and uninterrupted access to objects
  - To ensure high availability of services and data, use techniques like failover clustering, site resiliency,
automatic failover, load balancing, redundancy of hardware and software components, and fault tolerance

- **Authenticity**: ensuring a transmission, message or sender is legitimate. See the NIST glossary for examples: https://csrc.nist.gov/glossary/term/authenticity

- **Nonrepudiation**: 
  - ensures that the subject of activity or who caused an event cannot deny that the event occurred
  - Nonrepudiation is made possible through identification, authentication, authorization, accountability, and auditing

- **AAA Services**:
  - Identification: claiming to be an identity when attempting to access a secured area or system
  - Authentication: proving that you are that claimed identity
  - Authorization: defining the permissions (i.e. allow/grant and/or deny) of a resource and object access for a specific identity or subject
  - Auditing: recording a log of the events and activities related to the system and subjects
  - Accounting: (aka accountability) is reviewing log files to check for compliance and violations in order to hold subjects accountable for their actions, especially violations of organizational security policy
 
 [1.3](#1.3) **Evaluate and apply security governance principles**
 
- **Security governance**: the collection of practices related to supporting, evaluating, defining, and directing the security efforts of an organization. 
  - security governance is the implementation of a security solution and a management method that are tightly interconnected
  - There are numerous security frameworks and governance guidelines, including the National Institute of Standards and Technology (NIST) SP 800-53 and NIST SP 800-100
- **The security function**: the aspect of operating a business that focuses on the task of evaluating and improving security over time. To manage security, an org must implement proper and sufficient security governance
  - the act of performing a risk assessment to drive the security policy is the clearest and most direct example of management of the security function
- **Alignment of Security Function to Business Strategy, Goals, Mission, and Objectives**
  - **Strategic Plan**: a strategic plan is a long-term plan (useful for 5 years). It defines the organization's security purpose. A strategic plan should include risk assessment.
  - **Tactical Plan**: mid-term plan (1 year or less) developed to provide more details on accomplishing the goals set forth in the strategic plan
  - **Operational Plan**: a short-term, highly detailed plan based on strategic or tactical plans
  - All of these — strategy, goals, missions, and objectives — flow down, with each one supporting the others.
Objectives are the closest to the ground and represent small efforts to help you achieve a mission. Missions
represent a collection of objectives, and one or more missions leads to goals. When you reach your goals, you are
achieving the strategy
  - A security framework must closely tie to mission and objectives,enabling the business to complete its objectives and advance the mission while securing the environment based on risk tolerance
- **Organizational Processes**
  -  Security governance should address every aspect of an organization, including organizational processes of acquisitions, divestitures, and governance
  -  Be aware of the risks in acquisitions (since the state of the IT environment to be integrated is unknown, due diligence is key) and divestitures (how to split the IT infrastructure and what to do with identities and credentials)
  -  Understand the value of governance committees (vendor governance, project governance, architecture governance, etc.)
  -  Executives,managers and appointed individuals meet to review architecture, projects and incidents (security or otherwise),and provide approvals for new strategies or directions. The goal is a fresh set of eyes, often eyes that are not purely focused on information security
  - When evaluating a third-party for your security integration, consider the following:
    - on-site assement
    - document exchange and review
    - process/policy review
    - third-party audit

- **Organizational Roles and Responsibilities**
  -  Senior Manager: has a responsibility to keep the business running and to maximize profits and shareholder value
  - Security Professional: has the functional responsibility for security, including writing the security policy and implementing it
  - Asset Owner: responsible for classifying information for placement or protection within the security solution
  - Custodian: responsible for the task of implementing the proscribed protection defined by the security policy and senior management
  - Auditor: responsible for reviewing and verifying that the security policy is properly implemented

- **Security control frameworks**
  - A control framework helps ensure that your organization is covering all the bases around securing the environment. There are many frameworks to choose from, such as:
    -  Control Objectives for Information Technology (COBIT)
    -  ISO 27000 series (27000, 27001, 27002, etc.). 
    -  NIST CyberSecurity Framework (CSF)
      - designed for commerical orgs and critical infrastructure, consisting of five functions:
        - identify
        - protect
        - detect
        - respond
        - recovery    
  - These frameworks fall into four categories:
    - Preventative: security issues and violations through strategies such as policies and security awareness training
    - Deterrent: Discouraging malicious activities using access controls or technologies such as firewalls,intrusion detection systems and motion-activated cameras
    - Detective: Uncovering unauthorized activity in your environment
    - Corrective: Getting your environment back to where it was prior to a security incident 
