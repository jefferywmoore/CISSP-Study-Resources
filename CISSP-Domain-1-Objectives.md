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
      - COBIT is a documented set of best IT security practices by ISACA
      - Six key principles:
        - Provide stakeholder value
        - Holistic approach
        - Dynamic governance system
        - Governance distinct from management
        - Tailored to enterprise needs
        - End-to-end governance system   
    -  ISO 27000 series (27000, 27001, 27002, etc.). 
    -  NIST CyberSecurity Framework (CSF)
      - designed for commerical orgs and critical infrastructure, consisting of five functions:
        - identify
        - protect
        - detect
        - respond
        - recovery    
  - Due care/due diligence
    - Due diligence is establishing a plan, policy, and process to protect the interests of the organization. Due diligence is about understanding your security governance principles (policies and procedures) and the risks to your organization. Due diligence often involves gathering information through discovery, risk assessments and review of existing documentation; developing a formalized security structure containing a security policy, standards, baselines guidlines, and procedures; documentation to establish written policies; and disseminating the information to the organization
    - Due care is practicing the individual activities that maintain the due diligence effort. Due care is about your legal responsibility within the law or within organizational policies to implement your organization’s controls, follow security policies, do the right thing and make reasonable choices
    - Security documentation is the security policy
    - After establishing a framework for governance, security awareness training should be implemented, including all new hires, who complete the security awareness training as they come on board, and existing employees who should recertify regularly (typically yearly).

[1.4](#1.4) **Determine compliance and other requirements**
- Understand the difference between criminal, civil, and administrative law.
  - Criminal law: protects society against acts that violate the basic principles we believe in. Violations of criminal law are prosectued by federal and state governments
  - Civil law: provides the framework for the transaction of business between people and organizations. Violations of civil law are brought to the court and argued by the two affected parties
  - Administrative law is used by government agencies to effectively carry out their day-to-day business
- Compliance: Organizations may find themselves subject to a wide variety of laws, and regulations imposed by regulatory agencies or contractual obligation
  -  Payment Card Industry Data Security Standard (PCI DSS) - governs the security of credit card information and is enforced through the terms of a merchant agreement between a business that accpets CC payments, and the bank that processes the business' transactions
  -  Sarbanes-Oxley (SOX) - financial systems may be audited to ensure security controls are sufficient to ensure compliance with SOX
  -  Gramm-Leach-Bliley Act (GLBA) - affects banks, insurance companies, and credit providers; included a number of limitations on the types of information that could be exchanged even among subsidiaries of the same corp, and required financial institutions to provide written privacy policies to all their customers
  -  Health Insurance Portability and Accountability Act (HIPAA) - privacy and security regulations requiring strict security measures for hospitals, physicians, insurance companies, and other organizations that process or store private medical information about individuals; also clearly defines the rights of individuals who are the subject of medical records and requires organizations that maintain such records to disclose these rights in writing
  -  Federal Information Security Management Act (FISMA), requires federal agencies to implement an information security program that covers the agency's operations and contractors
  -  Computer Fraud and Abuse Act (CFAA) (as amended) protects computers used by the government or in interstate commerce from a variety of abuses
  -  Electronic Communications Privacy Act (ECPA) makes it a crime to invade the electronic privacy of an individual
  -  Digital Millennium Copyright Act prohibits the circumvention of copyright protection mechanisms placed in digital media and limits the liability of internet service providers for the activities of their users
-  Privacy requirements
  - European Union's General Data Protection Regulation (GDPR) - replaced Data Protection Directive (DPD), purpose is to provide a single, harmonized law that covers data throughout the EU
    - Lawfulness, fairness, and transparency
    - Purpose Limitation
    - Data Minimization
    - Accuracy
    - Storage Limitation
    - Security
    - Accountability
  - California Consumer Privacy Act (CCPA)
  - Be familiar with the EU Data Protection Directive. Be familiar with the requirements around healthcare
data, credit card data and other PII data as it relates to various countries and their laws and regulations

[1.5](#1.5) **Understand legal and regulatory issues that pertain to information security in a holistic context**
  - Cybercrime and data breaches:
    - Understand the notification requirements placed on organizations that experience a data breach
    - California's SB 1386 implemented the first statewide requiremnt to notify individuals of a breach of their personnel information; all other states eventually followed suit with similar laws
    - Currently, federal law only requires notification of individuals when a HIPAA-covered entity breaches their protected health information
    - Before an organization expands to other countries, perform due diligence to understand legal systems and what changes might be required to the way that data is handled and secured
    - In particular, be familiar with:
      - Council of Europe Convention on Cybercrime, a treaty signed by many countries that establishes standards for cybercrime policy 
      - laws about data breaches, including notification requirements. 
      - In the US, the Health Information Technology for Economic and Clinical Health (HITECH) Act requires notification of a data breach in some cases, such as when the personal health information was not protected as required by the Health Insurance Portability and Accountability Act (HIPAA) law 
      - The Gramm-Leach-Bliley Act (GLBA) applies to insurance and financial organizations; it requires notification to federal regulators, law enforcement agencies and customers when a data breach occurs. 
      - Certain states also impose their own requirements concerning data breaches 
      - the EU and other countries have their own requirements, for instance, the GDPR has very strict data breach notification requirements: A data breach must be reported to the competent supervisory authority within 72 hours of its discovery
      - Some countries do not have any reporting requirements
  - Licensing and intellectual property (IP) requirements
    - Trademarks:words, slogans, and logos used to identify a company and its products or services
    - Patents:A temporary monopoly for producing a specific item such as a toy, which must be novel and unique to qualify for a patent
      - Utility: protect the intellectual property rights of inventors
      - Design: cover the appearance of an invention and last for 15 years. They don't protect the idea of an invention only its form, and are generally seen as weaker
      - Software: area of on-going controversy; Google vs Oracle; given to rise of "patent trolls"
    - Copyright: exclusive use of artistic, musical or literary works which prevents unauthorized duplication, distribution or modification
    - Licensing: a contract between the software producer and the consumer which limits the use and/or distribution of the software
    - Trade Secrets: intellectual property that is critical to a business, and significant damage would result if it were disclosed to competitors or the public
  - Import / Export controls:
    -  Every country has laws around the import and export of hardware and software. For example, the US has restrictions around the export of cryptographic technology, and Russia requires a license to import encryption technologies manufactured outside the country
  -  Transborder data flow: 
    - Organizations should adhere to origin country-specific laws and regulations, regardless of where data resides
    - Also be aware of applicable laws where data is stored and systems are used
  - Privacy:
    -  Many laws include privacy protections for personal data. The EU’s General Data Protection Regulation (GDPR) has strong privacy rules that apply to any organization anywhere that stores or processes the personal data of EU residents; these individuals must be told how their data is collected and used, and they must be able to opt out. 
    -  The privacy guidelines of the Organization for Economic Co-operation and Development (OECD) require organizations to avoid unjustified obstacles to trans-border data flow, set limits to personal data collection, protect personal data with reasonable security and more. 
    -  The EU-US Privacy Shield (formerly the EU-US Safe Harbor agreement) controls data flow from the EU to the United States. The EU has more stringent privacy protections and without the Privacy Shield, personal data flow from the EU to the United States would not be allowed

[1.6](#1.6) **Understand requirements for investigation types (i.e. administrative, criminal, civil, regulatory, industry standards)**
An investigation will vary based on the type of incident being investigated. As an example, for a financial services company, a financial system compromise might cause a regulatory investigation. A system breach or website compromise might cause a criminal investigation. Each type of investigation has special considerations:
- **Administrative**: An administrative investigation has a primary purpose of providing the appropriate authorities with incident information. Thereafter, the authorities will determine the proper action, if any. Administrative investigations are often tied to HR scenarios, such as when a manager has been accused of improprieties
- **Criminal**: A criminal investigation occurs when a crime has been committed and you are working with a law enforcement agency to convict the alleged perpetrator. In such a case, it is common to gather evidence for a court of law, and to share the evidence with the defense. Therefore, you need to gather and handle the information using methods that ensure the evidence can be used in court. Remember that in a criminal case, a suspect must be proven guilty beyond a reasonable doubt. This is more difficult than showing a preponderance of evidence, which is often the standard in a civil case.
- **Civil**: In a civil case, one person or entity sues another. For example, one company might sue another for a trademark violation. A civil case is typically about monetary damages, and doesn't involve criminality. In a civil case, a preponderance of evidence is required to secure a victory. This differs from criminal cases, where a suspect is innocent until proven guilty beyond a reasonable doubt
- **Industry Standards**: An industry standards investigation is intended to determine whether an organization is adhering to a specific industry standard or set of standards, such as logging and auditing failed logon attempts. Because industry standards represent well-understood and widely implemented best practices, many organizations try to adhere to them even when they are not required to do so in order to improve security, and reduce operational and other risks
- **Regulatory**: A regulatory investigation is conducted by a regulatory body, such as the Securities and Exchange Commission (SEC) or Financial Industry Regulatory Authority (FINRA), against an organization suspected of an infraction. In such cases, the organization is required to comply with the investigation, for example, by not hiding or destroying evidence.

[1.7](#1.7) **Develop, document, and implement security policy, standards, procedures and guidelines**
The top tier of a formalized hierarchically organization security documentation is the security policy. A security policy is a document that defines the scope of security needed by the organization, and discusses the assets that require protection and the extent to which security solutions should go to provide the necessary protections. It defines the strategic security objectives, vision, and goals and outlines the security framework of the organization.
**Acceptable User Policy**: the AUP is a commonly produced document that exists as part of the overall  security documentation infrastructure. This policy defines a level of acceptable performance and expectation of behavior and activity. Failure to comply with the policy may result in job action warnings, penalties, or termination.

Security Standards, Baselines and Guidelines

Once the main security policies are set, the remaining security docuemntation can be crafted from these policies. 
- **Policies**: these are high-level documents, usually written by the management team. Policies are mandatory. A policy might will provide requirements, but not the steps for implementation
- **Standards**: more descriptive than policies, standards define compulsary requirements for the homogenous use of hardware, software, technology, and security controls, uniformly implemented throughout the organization
- **Baseline**: defines a minimum level of security that every system throughout the organization must meet. Baselines are usually system specific and refer to industry / government standards. As an example, a baseline for  server builds would be a list of configuration areas that should be applied to every server that is built. A Group Policy object (GPO) in a Windows network is sometimes used to comply with standards. Configuration management solutions can also help you establish baselines and spot configurations that are not in alignment
- **Guideline**: offers recommendations on how standards and baselines should be implemented & serves as an operational guide for security professionals and users. Guidelines are flexible, and can be customized for unique systems or conditions. They state which security mechanism should be deployed instead of prescribing a specific product or control. They are not complusory
- **Procedure** (or Standard Operating Procedure or SOP): detailed, step-by-step how-to doc that describes the exact actions necessary to implement a specific security mechanism, control, or solution

[1.8](#1.8) **Identiy, analyze, and prioritize business continuity (BC) requirements**

Business Continuity Planning (BCP) involves assessing the risk to organizational processes and creating policies, plans, and procedures to minimize the impact those risks might have on the organization if they were to occur.

BCP is used to maintain the continuous operation of a business in the event of an emergency, with a goal to implement a combination policies, procedures, and processes
Business continuity requires a lot of planning and preparation. Actual implementation of business continuity processes occurs quite infrequently. The primary facets of business continuity are resilience (within a data center and between sites or data centers), recovery (if a service becomes unavailable, you need to recover it as soon as possible), and contingency (a last resort in case resilience and recovery prove ineffective)

BCP vs DR: 

- BCP activities are typically strategically focused at a high level and center themselves on business processes and operations.
- DR plans tend to be more tactical and describe technical activities such as recovery sites, backups, and fault tolerance.

The overall goal of BCP is to provide a quick, calm, and efficient response in the event of an emergency and to enhance a company's ability to recover from a distruptive event promptly.

The BCP process has four main steps:

- **Project scope and planning**: Developing the project scope and plan starts with gaining support of the management team, making a business case (cost/benefit analysis, regulatory or compliance reasons,etc.) and gaining approval to move forward. Next, you need to form a team with representatives from the business as well as IT. Then you are ready to begin developing the plan. Start with a business continuity policy statement, then conduct a business impact analysis (see next item), and then develop the remaining components: preventive controls, relocation, the actual continuity plan, testing, training and maintenance)
- **Business impact analysis (BIA)**:Identify the systems and services that the business relies on and assess the impacts that a disruption or outage would cause, including the impacts on business processes like accounts receivable and sales. You also need to figure out which systems and services you need to get things running again (think foundational IT services such as the network and directory, which many other systems rely on). Finally, prioritize the order in which critical systems and services are recovered or brought back online. As part of the BIA, establish the **recovery time objectives** (RTOs) (how long it takes to recover), the **recovery point objectives** (RPOs) (the maximum tolerable data loss), and **maximum tolerable downtime** (MTD), along with the costs of downtime and recovery
- **Continuity planning**: The first two phases of the BCP process (project scope and planning and the business impact analysis) focus on determining how the BCP process will work and prioritizing the business assets that you must protect against interruption. The next phase of BCP development, continuity planning, focuses on developing and implementing a continuity strategy to minimize the impact realized risks might have on protected assets.

There are two primary subtasks involved in continuity planning:

  - Strategy development
  - Provisions and processes
  - Approval and implementation

The goal of this process is to create a **continuity of operations plan** (COOP), which focuses on how an organization will carry out critical business functions beginning shortly after a disruption occurs and extending up to one month of sustained operations.

The top priority of BCP and DRP is people. Primarily to get people out of harm's way, and then address IT recovery and restoration issues.

[1.9](#1.9) **Contribute to and enforce personnel security policies and procedures**

People are often considered the weakest element in any security solution. No matter what physical or logical controls are deployed, humans can discover ways of to avoid them, circumvent or subvert them, or disable them. Malicious actors are routinely targeting users with phishing and spear phishing campaigns, social engineering, and other types of attacks. Everybody is a target. And once attackers compromise an account, they can use that entry point to move around the network and elevate their privileges. However, people can also become a key security asset when they are properly trained and are motivated to protect not only themselves but the security of the organization as well.

The following strategies can reduce your risk:
  - **Candidate screening and hiring**: To properly plan for security, you must have standards in place for job descriptions, job classification, work tasks, job responsibilities, prevention of collusion, candidate screening, background checks, security clearances, employment agreements, and nondisclosure agreements. Screening employment candidates thoroughly is a key part of the hiring process. Be sure to conduct a full background check that includes a criminal records check, job history verification, education verification, certification validation and confirmation of other accolades when possible. Additionally, all references
should be contacted.

  - **Employment agreements and policies**: An employment agreement specifies job duties, expectations, rate of pay, benefits and information about termination. Sometimes, such agreements are for a set period (for example, in a contract or short-term job). Employment agreements facilitate termination when needed for an underperforming employee. The more information and detail in an employment agreement, the less risk (risk of a wrongful termination lawsuit, for example) the company has during a termination proceeding. For example, a terminated employee might take a copy of their email with them without thinking of it as stealing, but they are less likely to do so if an employment agreement or another policy document clearly prohibits it.
  - example employee agreements:
    - non-compete 
    - codes of conduct such as an acceptable use policy (AUP), which defines what is and isn’t acceptable acitivty, practice, or use for company equipemnt and resources
    - nondisclosure agreement (NDA), which is a doc used to protect confidential information from being disclosed by a current or former employee
  - **Onboarding, transfers and termination processes**:
    - onboarding: process of bringing a new employee into the organization
    - creating documented processes allowing the new employee to be intgrated quickly and consistently
    - transfer: an employee moves from one job to another, likely requiring adjusted account access to maintain appropriate least privilege
    - termination or offboarding: offboarding is the removal of an employee’s identity from the IAM system, once that person has left the oranization; can also be an element used when an employee transfers into a new role
    - whether cordial or abrupt, the ex-employee should be escorted off the premises and not allowed to return
  - **Vendor, consultant, contractor agreements and controls
    - organizations commonly outsource many IT functions, particularly data center hosting, contact-center support, and application development.
    - Info security policies and procedures must address outsourcing secuity and the use of service providers, vendors and consultants. Access control, document exchange and review, maintenance, on-site assessment, process and policy review, and service level agreements (SLAs) are examples of outsourcing security considerations
  - **Compliance policy requirements**:
    - compliance is the act of confirming or adhering to rules, policies, regulations, standards, or requirements
    - on a personnel level, compliance is related to individual employees following company policies and procedures
    - employees need to be trained on company standards as defined in the security policy and remain in compliance with any contractual obligations (e.g. with PCI DSS)
    - compliacne is a form of administrative or managerial security control
    - compliance enforcement is the application of sanctions or consequences for failing to follow policy, training, best practices, or regulations
  - **Privacy policy requirements**: 
    - Personally identifiable information (PII) about employees, partners, contractors, customers and other people should be stored in a secure way, accessible only to those who require the information to perform their jobs.
    - Organizations should maintain a documented privacy policy which outlines the type of data covered by the policy and who the policy applies to. Employees and contractors should be required to read and agree to the privacy policy upon hire and on a regular basis thereafter (such as annually)

[1.10](#1.10) **Understand and apply risk management concepts**

