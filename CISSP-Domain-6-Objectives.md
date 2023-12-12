[Domain 6](#domain6-top) **Security Assessment and Testing**

- Security assessment and testing program are an important mechanism for validating the on-going effectiveness of security controls
    - they include a variety of tools, such as vulnerability assessments, penetration tests, software testing, audits, and other control validation
- Every org should have a security assessment and testing program defined and operational
- **Security assessments**: comprehensive reviews of the security of a system, application, or other tested environment
    - during a security assessment, a trained information security professional performs a risk assessment that identifies vulnerabilities in the tested environment that may allow a compromise and makes recommendations for remediation, as needed
    - a security assessment includes the use of security testing tools, but go beyond scanning and manual penetration tests
    - the main work product of a security assessment is normally an assessment report addressed to management that contains the results of the assessment in nontechnical language and concludes with specific recommendations for improving the security of the tested environment
- An organization’s audit strategy will depend on its size, industry, financial status and other factors
    - a small non-profit, a small private company and a small public company will have different requirements and goals for their audit strategies
    - the audit strategy should be assessed and tested regularly to ensure that the organization is not doing a disservice to itself with the current strategy
    - there are three types of audit strategies: internal, external, and third-party

[6.1](#6.1) Design and validate assessment, test, and audit strategies (OSG-9 Chpt 15)
- 6.1.1 Internal
    - An organization’s security staff can perform security tests and assessments, and the results are meant for internal use only, designed to evaluate controls with an eye toward finding potential improvements
    - An internal audit strategy should be aligned to the organization’s business and day-to-day operations
        - e.g. a publicly traded company will have a more rigorous internal auditing strategy than a privately held company
    - Designing the audit strategy should include laying out applicable regulatory requirements and compliance goals
    - Internal audits are performed by an organization’s internal audit staff and are typically intended for internal audiences
    
- 6.1.2 External
    - An external audit strategy should complement the internal strategy, providing regular checks to ensure that procedures are being followed and the organization is meeting its compliance goals
    - External audits are performed by an outside auditing firm
        - these audits have a high degree of external validity because the auditors performing the assessment theoretically have no conflict of interest with the org itself
        - audits by these firms are generally considered acceptable by most investors and governing bodies
    
- 6.1.3 Third-party
    - Third-party audits are conducted by, or on behalf of, another org
    - In the case of a third-party audit, the org initiating the audit generally selects the auditors and designs the scope of the audit
    - The statement on Standards for Attestation Engagements document 18 (SSAE 18), titled Reporting on Controls, provides a common standard to be used by auditors performing assessments of service orgs with the intent of allowing the org to conduct external assessments, instead of multiple third-party assessments, and then sharing the resulting report with customers and potential customers
        - outside of the US, similar engagements are conducted under the International Standard for Attestation Engagements (ISAE) 3402, Assurance Reports on Controls at a Service Organization
    - SSAE 18 and ISAE 3402 engagements are commonly referred to as a service organization controls (SOC) audits
    - Three forms of SOC audits:
        - **SOC 1 Engagements**: assess the organization’s controls that might impact the accuracy of financial reporting
        - **SOC 2 Engagements**: assess the organization’s controls that affect the security (confidentiality, integrity, and availability) and privacy of information stored in a system
            - SOC 2 audit results are confidential and are usually only shared outside an org under an NDA
        - **SOC 3 Engagements**: assess the organization’s controls that affect the security (confidentiality, integrity, and availability) and privacy information stored in a system
            - however, SOC3 audit results are intended for public disclosure
    - Two types of SOC reports:
        - **Type I Reports**: provide the auditor’s opinion on the description provided by management and the suitability of the design of the controls
            - type I reports also cover only a specific point in time, rather than an extended period
            - think of Type I report as more of a documentation review
        - **Type II Reports**: go further and also provide the auditor’s opinion on the operating effectiveness of the controls
            - the auditor actually confirms the controls are functioning properly
            - Type II reports also cover an extended period of time, at least 6 months
            - think of Type II report as similar to a traditional audit; the auditor is checking the paperwork, and verifying the controls are functioning properly
        - Type II reports are considered much more reliable than Type I reports (Type I reports simply take the service orgs word that the controls are implemented as described)

[6.2](#6.2) Conduct security control testing (OSG-9 Chpt 15)
- Security control testing can include testing of the physical facility, logical systems and applications. Here are the common testing methods:
- 6.2.1 Vulnerability assessment
    - **Vulnerabilities**: weaknesses in systems and security controls that might be exploited by a threat
    - Vulnerability assessments: examining systems for these weaknesses
    - The goal of a vulnerability assessment is to identify elements in an environment that are not adequately protected -- and not necessarily from a technical perspective; you can also assess the vulnerability of physical security or the external reliance on power, for instance
        - can include personnel testing, physical testing, system and network testing, and other facilities tests
    - Vulnerability assessments are some of the most important testing tools in the information security professional’s toolkit
    - **Security Content Automation Protocol (SCAP)**: provides a common framework for discussion and facilitation of automation of interactions between different security systems (sponsored by NIST)
        - SCAP components related to vulnerability assessments:
            - **Common Vulnerabilities and Exposures (CVE)**: provides a naming system for describing security vulnerabilities
            - **Common Vulnerability Scoring Systems (CVSS)**: provides a standardized scoring system for describing the severity of security vulnerabilities
            - **Common Configuration Enumeration (CCE)**: provides a naming system for system config issues
            - **Common Platform Enumeration (CPE)**: provides a naming system for operating systems, applications, and devices
            - **Extensible Configuration Checklist Description Format (XCCDF)**: provides a language for specifying security checklists
            - **Open Vulnerability and Assessment Language (OVAL)**: provides a language for describing security testing procedures
    - Vulnerability scans automatically probe systems, applications, and networks looking for weaknesses that could be exploited by an attacker
    - Four main categories of vulnerability scans:
        - network discovery scans
        - network vulnerability scans
        - web application vulnerability scans
        - database vulnerability scans
- 6.2.2 Penetration testing
- 6.2.3 Log reviews
- 6.2.4 Synthetic transactions
- 6.2.5 Code review and testing
- 6.2.6 Misuse case testing
- 6.2.7 Test coverage analysis
- 6.2.8 Interface testing
- 6.2.9 Breach attack simulations
- 6.2.10 Compliance checks

[6.3](#6.3) Collect security process data (e.g. technical and administrative) (OSG-9 Chpts 15,18)
- 6.3.1 Account management
- 6.3.2 Management review and approval
- 6.3.3 Key performance and risk indicators
- 6.3.4 Backup verification data
- 6.3.5 Training and awareness
- 6.3.6 Disaster Recover (DR) and Business Continuity (BC)

[6.4](#6.4) Analyze test output and generate report (OSG-9 Chpt 15)
- 6.4.1 Remediation
- 6.4.2 Exception handling
- 6.4.3 Ethical disclosure

[6.5](#6.5) Conduct or facilitate security audits (OSG-9 Chpt 15)
- 6.5.1 Internal
- 6.5.2 External
- 6.5.3 Third-party