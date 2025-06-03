# [Domain-6](#domain-6-security-assessment-and-testing) **Security Assessment and Testing**

Security assessment and testing programs are an important mechanism for validating the on-going effectiveness of security controls; this domain accounts for ~12% of the exam

- Security assessment and testing include a variety of tools, such as vulnerability assessments, penetration tests, software testing, audits, and other control validation; every org should have a security assessment and testing program defined and operational
- **Security assessments**: comprehensive reviews of the security of a system, application, or other tested environment
  - during a security assessment, a trained information security professional performs a risk assessment that identifies vulnerabilities in the tested environment that may allow a compromise and makes recommendations for remediation, as needed
  - a security assessment includes the use of security testing tools, but goes beyond scanning and manual penetration tests
  - the main work product of a security assessment is normally an assessment report addressed to management that contains the results of the assessment in nontechnical language and concludes with specific recommendations for improving the security of the tested environment
- An organization’s audit strategy will depend on its size, industry, financial status and other factors
  - a small non-profit, a small private company and a small public company will have different requirements and goals for their audit strategies
  - the audit strategy should be assessed and tested regularly to ensure that the organization is not doing a disservice to itself with the current strategy
  - there are three types of audit strategies: internal, external, and third-party
- Software testing verifies that code functions as designed and doesn't contain security flaws
- Security management needs to perform a variety of activities to properly oversee the information security program
  - Log reviews, especially for admin activities, ensure that systems are not misused
  - Account management reviews ensure that only authorized users have access to information and systems
  - Backup verification ensures that the org's data protection process is working properly
  - Key performance and risk indicators provide a high-level view of security program effectiveness

- **Artifact**: piece of evidence such as text, or a reference to a resource which is submitted in response to a question
- **Assessment**: testing or evaluation of controls to understand which are implemented correctly, operating as intended and producing the desired outcome in meeting the security or privacy requirements of a system or org
- **Audit**: process of reviewing a system for compliance against a standard or baseline (e.g. audit of security controls, baselines, financial records) can be formal and independent, or informal/internal
- **Chaos Engineering**: discipline of experiments on a software system in production to build confidence in the system's capabilities to withstand turbulent/unexpected conditions
- **Code testing suite**: usually used to validate function, statement, branch and condition coverage
- **Compliance Calendar**: tracks an org's audits, assessments, required filings, due dates and related
- **Compliance Tests**: an evaluation that determines if an org's controls are being applied according to management policies and procedures
- **Examination**: process of reviewing/inspecting/observing/studying/analyzing specs/mechanisms/activities to understand, clarify, or obtain evidence
- **FedRAMP: (see Domain 1) a government-wide program that standardizes the security assessment, authorization, and monitoring of cloud services and products; the program was established in 2011 to help the federal government use cloud technologies while protecting federal information
- **Findings**: results created by the application of an assessment procedure
- **Functional order of controls**: deter, deny, detect, delay, determine, and decide
- **Fuzzing**: uses modified inputs to test software performance under unexpected circumstances
  - Mutation (dumb) fuzzing modifies known inputs to generate synthetic inputs that may trigger unexpected behavior
  - Generational (intelligent) fuzzing develops inputs based on models of expected inputs to perform the same task
- **IAM system**: identity and access management system combines lifecycle management and monitoring tools to ensure that identity and authorization are properly handled throughout an org
- **ITSM**: IT Service Management tools include change management and associated approval tracking
- **Judgement Sampling**: AKA purposive or authoritative sampling, a non-probability sampling technique where members are chosen only on the basis of the researcher's knowledge and judgement
- **Misuse Case Testing**: testing strategy from a hostile actor's point of view, attempting to lead to integrity failures, malfunctions, or other security or safety compromises
- **Mutation testing**: mutation testing modifies a program in small ways and then tests that mutant to determine if it behaves as it should or if it fails; technique is used to design and test software through mutation
- **Penetration Testing/Ethical Penetration Testing**: security testing and assessment where testers actively attempt to circumvent/default a system's security features; typically constrained by contracts to stay within specified Rules of Engagement (RoE)
- **Plan of Action and Milestones (POA&M)**: a document identifying tasks to be accomplished, including details, resources, milestones, and completion target dates
- **RUM**: real user monitoring is a passive monitoring technique that records user iteration with an app or system to ensure performance and proper app behavior; often used as a pre-deployment process using the actual user interface
- **RoE**: Rules of Engagement, set of rules/constraints/boundaries that establish limits of participant activity; in ethical pen testing, an RoE defines the scope of testing, and to establish liability limits for both testers and the sponsoring org or system owners
- **SCF**: Script Check Engine is designed to make scripts interoperable with security policy definitions
- **Statistical Sampling**: process of selecting subsets of examples from a population with the objective of estimating properties of the total population
- **Substantive Test**: testing technique used by an auditor to obtain the audit evidence in order to support the auditor's opinion
- **Testing**: process of exercising one or more assessment objects (activities or mechanisms) under specified conditions to compare actual to expected behavior
- **Trust Services Criteria (TSC)**: used by an auditor when evaluating the suitability of the design and operating effectiveness of controls relevant to the security, availability, or processing integrity of information and systems or the confidentiality or privacy of the info processed by the entity

## [6.1](#61-design-and-validate-assessment-test-and-audit-strategies-osg-10-chpt-15) Design and validate assessment, test, and audit strategies (OSG-10 Chpt 15)

- Security audits occur when a third-party performs an assessment of the security controls protecting an org's information assets

- 6.1.1 Internal (e.g., within organization control)
  - An organization’s security staff can perform security tests and assessments, and the results are meant for internal use only, designed to evaluate controls with an eye toward finding potential improvements
  - An internal audit strategy should be aligned to the organization’s business and day-to-day operations
    - e.g. a publicly traded company will have a more rigorous internal auditing strategy than a privately held company
  - Designing the audit strategy should include laying out applicable regulatory requirements and compliance goals
  - Internal audits are performed by an organization’s internal audit staff and are typically intended for internal audiences, and management use

- 6.1.2 External (e.g., outside organization control)
  - An external audit strategy should complement the internal strategy, providing regular checks to ensure that procedures are being followed and the organization is meeting its compliance goals
  - External audits are performed by an outside auditing firm
    - these audits have a high degree of external validity because the auditors performing the assessment theoretically have no conflict of interest with the org itself
    - audits by these firms are generally considered acceptable by most investors and governing bodies
    - third-party audit reporting is generally intended for the org's governing body

- 6.1.3 Third-party (e.g., outside of enterprise control)
  - Third-party audits are conducted by, or on behalf of, another org
  - In the case of a third-party audit, the org initiating the audit generally selects the auditors and designs the scope of the audit
  - The statement on **Standards for Attestation Engagements document 18 (SSAE 18)**, titled Reporting on Controls, provides a common standard to be used by auditors performing assessments of service orgs with the intent of allowing the org to conduct external assessments, instead of multiple third-party assessments, and then sharing the resulting report with customers and potential customers
    - outside of the US, similar engagements are conducted under the International Standard for Attestation Engagements (ISAE) 3402, Assurance Reports on Controls at a Service Organization
  - SSAE 18 and ISAE 3402 engagements are commonly referred to as a service organization controls (SOC) audits
  - Three forms of SOC audits:
    - **SOC 1 Engagements**: assess the organization’s controls that might impact the accuracy of financial reporting
    - **SOC 2 Engagements**: assess the organization’s controls that affect the security and privacy of information stored in a system
      - SOC 2 focus on 5 trust principles: Security, Availability, Confidentiality, Processing Integrity, and Privacy
      - SOC 2 audit results are confidential and are usually only shared outside an org under an NDA
    - **SOC 3 Engagements**: assess the organization’s controls that affect the security (confidentiality, integrity, and availability) and privacy information stored in a system
      - however, SOC3 audit results are intended for public disclosure; they are regarded primarily as marketing tools
  - Two types of SOC reports:
    - **Type I Reports**: provide the auditor’s opinion on the description provided by management and the suitability of the design of the controls
      - type I reports cover only a specific point in time, rather than an extended period
      - think of Type I report as more of a documentation review
    - **Type II Reports**: go further and also provide the auditor’s opinion on the operating effectiveness of the controls
      - the auditor actually confirms the controls are functioning properly
      - Type II reports also cover an extended period of time, at least 6 months, typically a year
      - think of Type II report as similar to a traditional audit; the auditor is checking the paperwork, and verifying the controls are functioning properly
    - Type II reports are considered much more reliable than Type I reports (Type I reports simply take the service orgs word that the controls are implemented as described); security pros want SOC2, Type II reports

- 6.1.4 Location (e.g., on-premise, cloud, hybrid)
  - On-premise assessment: focuses on evaluating the security measures and infrastructure of in-house systems, or within an organization's physical data centers and facilities
  - Cloud assessment: focus is on assessing the security of data and applications hosted in cloud service providers environment
  - Hybrid assessment: assess connectivity and security measures used between on-premise and cloud resources; this assessment looks at data flow or interconnection and integration security controls

## [6.2](#62-conduct-security-controls-testing-osg-10-chpt-15) Conduct security controls testing (OSG-10 Chpt 15)

- Security control testing can include testing of the physical facility, logical systems and applications; common testing methods include the following

- 6.2.1 Vulnerability assessment
  - **Vulnerabilities**: weaknesses in systems and security controls that might be exploited by a threat
  - **Vulnerability assessments**: examining systems for these weaknesses; steps in the assessment:
    - Reconnaissance: passively gather publicly available info
    - Enumeration: actively enumerate through target IP addresses and ports
    - Vulnerability Analysis: Identify potential vulns to be exploited
    - Execution: applies only if you are doing a penetration test
    - Document Findings: reporting on findings and severity
  - The goal of a vulnerability assessment is to identify elements in an environment that are not adequately protected -- and not necessarily from a technical perspective; you can also assess the vulnerability of physical security or the external reliance on power, for instance
    - can include personnel testing, physical testing, system and network testing, and other facilities tests
  - Vulnerability assessments are some of the most important testing tools in the information security professional’s toolkit
  - **Security Content Automation Protocol (SCAP)**: provides a common framework and suite of specifications that standardize how software flaws and security configuration is communicated both to machines and humans; provides discussion and facilitation of automation of interactions between different security systems (see [NIST 800-126](https://csrc.nist.gov/pubs/sp/800/126/r3/final))
    - SCAP components related to vulnerability assessments:
      - **Common Vulnerabilities and Exposures (CVE)**: provides a naming system for describing security vulnerabilities
      - **Common Vulnerability Scoring Systems (CVSS)**: provides a standardized scoring system for describing the severity of security vulnerabilities; it includes metrics and calc tools for exploitability, impact, how mature exploit code is, and how vulnerabilities can be remediated, and a means to score vulns against users' unique requirements
      - **Common Configuration Enumeration (CCE)**: provides a naming system for system config issues
      - **Common Platform Enumeration (CPE)**: provides a naming system for operating systems, applications, and devices
      - **eXtensible Configuration Checklist Description Format (XCCDF)**: provides a language for specifying security checklists
      - **Open Vulnerability and Assessment Language (OVAL)**: provides a language for describing security testing procedures; used to describe the security condition of a system
  - Vulnerability scans automatically probe systems, applications, and networks looking for weaknesses that could be exploited by an attacker
    - flaws may include missing patches, misconfigurations, or faulty code
  - Four main categories of vulnerability scans:
    - network discovery scans
    - network vulnerability scans
    - web application vulnerability scans
    - database vulnerability scans
  - **Authenticated scans**: (AKA credentialed security scan) involves conducting vulnerability assessments and security checks on a network, system, or application using valid credentials; this approach enables the scanner to simulate the actions of an authenticated user, allowing it to access deeper layers of the target system, gather more information, and provide a more accurate assessment of vulnerabilities; often uses a read-only account to access configuration files

- 6.2.2 Penetration testing (e.g., red, blue, and/or purple team exercises)
  - Penetration tests go beyond vulnerability testing techniques because they attempt to exploit systems
  - **Vulnerability management**: the cyclical process of identifying, classifying, prioritizing, and mitigating vulnerabilities; programs take the results of the tests as inputs and then implement a risk management process for identified vulnerabilities, with the following steps:
    - Asset inventory
    - Identifying the value of each asset
    - Identifying the vulnerabilities for each asset
    - Ongoing review and assessment
  - Testing stages from the OSG include:
    - Reconnaissance: passively gather publicly available info
    - Enumeration: active network discovery (i.e. find target IP address and ports)
    - Vulnerability analysis: identify potential vulns
    - Execution: attempt to exploit vulns
    - Document findings: report on findings
  - NIST defines the penetration testing process as consisting of four phases:
    - **planning**: includes agreement on the scope of the test and the rules of engagement
      - ensures that both the testing team and management are in agreement about the nature of the test and that it is explicitly authorized
    - **information gathering and discovery**: uses manual and automated tools to collect information about the target environment
      - basic reconnaissance (website mapping)
      - network discovery
      - testers probe for system weaknesses using network, web and db vuln scans
    - **attack**: seeks to use manual and automated exploit tools to attempt to defeat system security
      - step where pen testing goes beyond vuln scanning as vuln scans don’t attempt to actually exploit detected vulns
    - **reporting**: summarizes the results of the pen testing and makes recommendations for improvements to system security
  - tests are normally categorized into three groups:
    - **white-box penetration test**:
      - AKA "**known environment tests**"
      - white box provides the attackers with **detailed information** about the systems they target
      - this bypasses many of the reconnaissance steps that normally precede attacks, shortening the time of the attack and increasing the likelihood that it will find security flaws
      - in white-box testing, the tester has access to the source code and performs testing from a developer's perspective
    - **gray-box penetration test**:
      - AKA **partial knowledge tests**, these are sometimes chosen to balance the advantages and disadvantages of white- and black-box penetration tests
      - this is particularly common when black-box results are desired but costs or time constraints mean that some knowledge is needed to complete the testing
      - these tests are sometimes called "**partially known environment**" tests
      - in gray-box testing, the tester evaluates software from a user perspective but has access to the source code
    - **black-box penetration test**:
      - AKA "**unknown environment tests**"
      - does not provide attackers with any information prior to the attack
      - this simulates an external attacker trying to gain access to information about the business and technical environment before engaging in an attack
  - Differences between vulnerability assessments and pen tests: vuln assessments are usually more automated, can be performed quickly, and no attempt to made to exploit vulns
  - Red, blue andd purple teams have been around for a long time, and is becoming more popular
    - Red team: this is the in-house offensive security team, they are the simulated hackers or the threat providing:
      - offensive security
      - ethical hacking
      - penetration testing
      - social engineering
      - threat intelligence
    Blue team: the blue team is the in-house defensive team, working to stop the threat:
      - defensive security
      - security monitoring
      - incident response
      - digital forensics
      - security operations
    Purple: not a separate team, but purple represents the collaboration between the red and blue teams:
      - red and blue teams working together
      - providing information sharing and healthy competition

- 6.2.3 Log reviews
  - **Security Information and Event Management (SIEM)**: packages that collect information using the syslog functionality present in many devices, operating systems, and applications
  - SIEM capabilities: aggregation, normalization, correlation, secure storage, analysis, reporting
  - Log data is recorded in databases; common logs include:
    - security, application, firewall, proxy, and change management logs
  - Log files should be protected by centrally storing them and using permissions to restrict access, and archived logs should be set to read-only to prevent modification
  - Admins may choose to deploy logging policies through Windows Group Policy Objects (GPOs)
  - Logging systems should also make use of the Network Time Protocol (NTP) to ensure that clocks are synchronized on systems sending log entries to the SIEM as well as the SIEM itself, ensuring info from multiple sources have a consistent timeline
  - Information security managers should also periodically conduct log reviews, particularly for sensitive functions, to ensure that privileged users are not abusing their privileges
  - Network flow (NetFlow) logs are particularly useful when investigating security incidents

- 6.2.4 Synthetic transactions/benchmarks
  - **Synthetic transactions**: scripted transactions with known expected results
  - **Synthetic monitoring**: uses emulated or recorded transactions to monitor for performance changes in response time, functionality, or other performance monitors
  - Dynamic testing may include the use of synthetic transactions to verify system performance; synthetic transactions are run against code and compare out to expected state

- 6.2.5 Code review and testing
  - Code review and testing is "one of the most critical components of a software testing program"
  - These procedures provide third-party reviews of the work performed by developers before moving code into a production environment, possibly discovering security, performance, or reliability flaws in apps before they go live and negatively impact business operations
  - In code review, AKA peer review, developers other than the one who wrote the code review it for defects; code review can be a formal or informal validation process
  - **Fagan inspections**: the most formal code review process follows six steps:
    1) planning
    2) overview
    3) preparation
    4) inspection
    5) rework
    6) follow-up
    - Entry criteria are the criteria or requirements which must be met to enter a specific process
    - Exit criteria are the criteria or requirements which must be met to complete a specific process
  - **Static application security testing (SAST)**: evaluates the security of software without running it by analyzing either the source code or the compiled application; code reviews are an example of static app security testing
  - **Dynamic application security testing (DAST)**: evaluates the security of software in a runtime environment and is often the only option for organizations deploying applications written by someone else

- 6.2.6 Misuse case testing
  - **Misuse case testing**: AKA abuse case testing - used by software testers to evaluate the vulnerability of their software to known risks; focuses on behaviors that are not what the org desires or that are counter to the proper function of a system/app
  - In misuse case testing, testers first enumerate the known misuse cases, then attempt to exploit those use cases with manual or automated attack techniques

- 6.2.7 Coverage analysis
  - A test coverage analysis is used to estimate the degree of testing conducted against new software; to provide insight into how well testing covered the use cases that an app is being tested for
  - **Test coverage**: number of use cases tested / total number of use cases
    - requires enumerating possible use cases (which is a difficult task), and anyone using test coverage calcs to understand the process used to develop the input values
  - Five common criteria used for test coverage analysis:
    - **branch coverage**: has every IF statement been executed under all IF and ELSE conditions?
    - **condition coverage**: has every logical test in the code been executed under all sets of inputs?
    - **functional coverage**: has every function in the code been called and returned results?
    - **loop coverage**: has every loop in the code been executed under conditions that cause code execution multiple times, only once, and not at all?
    - **statement coverage**: has every line of code been executed during the test?
  - **Test coverage report**: measures how many of the test cases have been completed; is used to provide test metrics when using test cases

- 6.2.8 Interface testing (e.g., user interface, network interface, application programming interface (API))
  - Interface testing assesses the performance of modules against the interface specs to ensure that they will work together properly when all the development efforts are complete
  - Interface testing essentially assesses the interaction between components and users with API testing, user interface testing, and physical interface testing
    - Three types of interfaces should be tested:
      - application programming interfaces (APIs): offer a standardized way for code modules to interact and may be exposed to the outside world through web services
        - should test APIs to ensure they enforce all security requirements
      - user interfaces (UIs): examples include graphical user interfaces (GUIs) and command-line interfaces
        - UIs provide end users with the ability to interact with the software, and tests should include reviews of all UIs
      - physical interfaces: exist in some apps that manipulate machinery, logic controllers, or other objects
        - software testers should pay careful attention to physical interfaces because of the potential consequences if they fail
    - Also see [OWASP API security top 10](https://owasp.org/API-Security/editions/2023/en/0x11-t10/)

- 6.2.9 Breach attack simulations
  - **Breach and attack simulation (BAS)**: platforms that seek to automate some aspects of penetration testing
  - The BAS platform is not actually waging attacks, but conducting automated testing of security controls to identify deficiencies
  - A BAS system combines red team (attack) and blue team (defense) techniques together with automation to simulate advanced persistent threats (and other advanced threat actors) running against the environment
  - Designed to inject threat indicators onto systems and networks in an effort to trigger other security controls (e.g. place a suspicious file on a server)
    - detection and prevention controls should immediately detect and/or block this traffic as potentially malicious
  - See:
    - OWASP Web Security Testing Guide
    - OSSTMM (Open Source Security Testing Methodology Manual)
    - NIST 800-115
    - FedRAMP Penetration Test Guidance
    - PCI DSS Information Supplemental on Penetration Testing

- 6.2.10 Compliance checks
  - Orgs should create and maintain compliance plans documenting each of their regulatory obligations and map those to the specific security controls designed to satisfy each objective
  - Compliance checks are an important part of security testing and assessment programs for regulated firms: these checks verify that all of the controls listed in a compliance plan are functioning properly and are effectively meeting regulatory requirements

## [6.3](#63-collect-security-process-data-eg-technical-and-administrative-osg-10-chpts-1518) Collect security process data (e.g. technical and administrative) (OSG-10 Chpts 15,18)

- Many components of the information security program generate data that is crucial to security assessment processes; these components include:
  - Account management process
  - Management review and approval
  - Key performance and risk indicators
  - Backup verification data
  - Data generated by disaster recovery and business continuity programs

- 6.3.1 Account management
  - Preferred attacker techniques for obtaining privilege user access include:
    - compromising an existing privileged account: mitigated through use of strong authentication (strong passwords and multifactor), and by admins use of privileged accounts only for specific tasks
    - privilege escalation of a regular account or creation of a new account: these approaches can be mitigated by paying attention to the creation, modification, and use of user accounts

- 6.3.2 Management review and approval
  - Account management reviews ensure that users only retain authorized permissions and that unauthorized modifications do not occur
  - Full review of accounts: time-consuming to review all, and often done only for highly privileged accounts
  - Organizations that don’t have time to conduct a full review process may use sampling, but only if sampling is truly random
  - Adding accounts: should be a well-defined process, and users should sign an AUP
  - Adding, removing, and modifying accounts and permissions should be carefully controlled and documented
  - Accounts that are no longer needed should be suspended
  - ISO 9000 standards use a Plan-Do-Check-Act loop
    - plan: foundation of everything in the ISMS, determines goals and drives policies
    - do: security operations
    - check: security assessment and testing (this objective)
    - act: formally do the management review

- 6.3.3 Key performance and risk indicators
  - **Key Performance Indicators (KPIs)**: measures that provide significance of showing the performance of an ISMS compared to stated goals; KPIs are backward looking
    - Choose the factors that can show the state of security
    - Define baselines for some (or better yet all) of the factors
    - Develop a plan for periodically capturing factor values (use automation!)
    - Analyze and interpret the data and report the results
    - Key metrics or KPIs that should be monitored by security managers may vary from org to org, but could include:
      - number of open vulns
      - time to resolve vulns
      - vulnerability/defect recurrence
      - number of compromised accounts
      - number of software flaws detected in pre-production scanning
      - repeat audit findings
      - user attempts to visit known malicious sites
    - Develop a dashboard of metrics and track them
  - **Key Risk Indicators (KRIs)**: indicate the level of exposure to operational risk; they help monitor potential future shifts in risk conditions or emerging risks; KRIs are forward-looking

- 6.3.4 Backup verification data
  - Managers should periodically inspect the results of backups to verify that the process functions effectively and meets the organization’s data protection needs
    - this might include reviewing logs, inspecting hash values, or requesting an actual restore of a system or file

- 6.3.5 Training and awareness
  - Training and awareness programs play a crucial role in preparing an organization’s workforce to support information security programs
  - They educate employees about current threats and advise them on best practices for protecting information and systems under their care from attacks
  - Program should begin with initial training designed to provide foundation knowledge to employees who are joining the org or moving to a new role; the initial training should be tailored to an individual’s role
  - Training and awareness should continue to take place throughout the year, reminding employees of their responsibilities and updating them on changes to the organization’s operating environment and threat landscape
  - Use phishing simulations to evaluate the effectiveness of their security awareness programs

- 6.3.6 Disaster Recover (DR) and Business Continuity (BC)
  - **Business Continuity (BC)**: the processes used by an organization to ensure, holistically, that its vital business processes remain unaffected or can be quickly restored following a serious incident
  - **Disaster Recovery (DR)**: is a subset of BC, that focuses on restoring information systems after a disaster
    - these programs should take a comprehensive approach to planning and include considerations related to the initial response effort, personnel involved, communication among the team members and with internal and external entities, assessment of response efforts, and restoration of services
    - DR programs should also include training and awareness efforts to ensure personnel understand their responsibilities and lessons learned sessions to continuously improve the program
  - These processes need to be periodically accessed, and regular testing of disaster recovery and business continuity controls provide organizations with the assurance they are effectively protected against disruptions to business ops
  - Protection of life is of the utmost importance and should be dealt with first before attempting to save material things

## [6.4](#64-analyze-test-output-and-generate-report-osg-10-chpt-15) Analyze test output and generate report (OSG-10 Chpt 15)

- Step 1: review and understand the data
  - The goal of the analysis process is to proceed logically from facts to actionable info
  - A list of vulns and policy exceptions is of little value to business leaders unless it's used in context, so once all results have been analyzed, you're ready to start writing the official report
- Step 2: determine the business impact of those facts
  - Ask "so what?"
- Step 3: determine what is actionable
  - The analysis process leads to valuable results only if they are actionable

- 6.4.1 Remediation
  - Rather than software defects, most vulnerabilities in average orgs come from misconfigured systems, inadequate policies, unsound business processes, or unaware staff
  - Vuln remediation should include all stakeholders, not just IT

- 6.4.2 Exception handling
  - **Exception handling**: the process of handling unexpected activity, since software should never depend on users behaving properly
    - "expect the unexpected", gracefully handle invalid input and improperly sequenced activity etc
  - Sometimes vulns can't be patched in a timely manner (e.g. medical devices needing re-accreditation) and the solution is to implement compensatory controls, document the exception and decision, and revisit
    - **compensatory controls**: measures taken to address any weaknesses of existing controls or to compensate for the inability to meet specific security requirements due to various different constraints
    - e.g. micro-segmentation of device, access restrictions, monitoring etc
  - Exception handling may be required due to system crash as the result of patching (requiring roll-back)

- 6.4.3 Ethical disclosure
  - While conducting security testing, cybersecurity pros may discover previously undiscovered vulns (perhaps implementing compensating controls to correct) that they may be unable to correct
  - **Ethical disclosure**: the idea that security pros who detect a vuln have a responsibility to report it to the vendor, providing them with enough time to patch or remediate
    - the disclosure should be made privately to the vendor providing reasonable amount of time to correct
    - if the vuln is not corrected, then public disclosure of the vuln is warranted, such that other professionals can make informed decisions about future use of the product(s)

## [6.5](#65-conduct-or-facilitate-security-audits-osg-10-chpt-15) Conduct or facilitate security audits (OSG-10 Chpt 15)

- 6.5.1 Internal
  - Having an internal team conduct security audits has several advantages:
    - understanding the internal environment reduces time
    - an internal team can delve into all parts of systems, because they have insider knowledge
    - internal auditors can be more agile in adapting to changing needs, rescheduling failed assessment components quickly
  - Disadvantages of using an internal team to conduct security audits:
    - the team may have limited exposure to new/other methodologies (e.g. the team may have depth but not breadth of experience and knowledge)
    - potential conflicts of interest (e.g. reluctance to throw other teams under the bus and accurately report their findings)
    - audit team members may start with an agenda (say to secure funding) and overstate faults, or have interpersonal motives

- 6.5.2 External
  - An external audit (sometimes called a second-party audit) is one conducted by (or on behalf of) a business partner
  - External audits are tied to contracts; by definition, an external audit should be scoped to include only the contractual obligations of an organization

- 6.5.3 Third-party
  - Third-party audits are often needed to demonstrate compliance with some government regulation or industry standard
  - Advantages of having a third-party audit an organization:
    - they likely have breadth of experience auditing many types of systems, across many types of organizations
    - they are not affected by internal dynamics or org politics
  - Disadvantage of using a third-party auditor:
    - cost: third-party auditors are going to be much more costly than internal teams; this means that the organization is not likely to conduct audits as frequently
    - internal resources are still required to assist or accompany auditors, to answer questions and guide

- 6.5.4 Location (e.g., on-premise, cloud, hybrid)
  - As in 6.1.4 above:
  - On-premise assessment: focuses on evaluating the security measures and infrastructure of in-house systems, or within an organization's physical data centers and facilities
  - Cloud assessment: focus is on assessing the security of data and applications hosted in cloud service providers environment
  - Hybrid assessment: assess connectivity and security measures used between on-premise and cloud resources; this assessment looks at data flow or interconnection and integration security controls
