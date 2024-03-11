[Domain 8](#domain8-top) **Software Development Security**

[8.1](#8.1) Understand and integrate security in the Software Develoment Life Cycle (SDLC) (OSG-9 Chpt 20)
- Domain 8 is focused on helping security pros understand, and apply software or application security
    - Applications can present significant risks, and security pros must understand and balance these risks with business requirements and implement appropriate risk mitigation; if a company develops custom software, the custom solution can present additional, unique risks and vulns 
        - orgs with custom solutions should be on the lookout for logic weaknesses (e.g. buffer overflow vulns), and guard against malicious changes (e.g. backdoors) that can leave the system vulnerable to attacks
    - As software development environments have become increasingly complex, it's important to review this area -- one of the biggest threats to an organization's security

- In this domain you'll learn the basic principles behind securely designing, building, testing, operating and even decomissioning enterprise apps
- Security should be part of the design, and incorporated into the architecture, with the level of protection based on requirements and operating environment

- 8.1.1 Development methodologies (e.g. Agile, Waterfall, DevOps, DevSecOps)
    - **Agile methodology**: a project management approach to development that involves breaking the project into phases and emphasizes continuous collaboration and improvement;  teams follow a cycle of planning, executing, and evaluating
        - Agile development emphasizes:
            - the delivery of working software in short iterations, helping to get the software to market faster 
            - reduced risk by frequently testing and providing feedback, helping to identify and resolve issues earlier in the development process
        - Seventeen pioneers of the Agile development approach got together in 2001, producing the Manifesto for Agile Software Development (agilemanifesto.org) that states the core philosophy of the Agile approach:
            - **Individuals and interactions** over processes and tools
            - **Working software** over comprehensive documentation
            - **Customer collaboration** over contract negotiation
            - **Responding to change** over following a plan
        - Agile Manifesto also defines 12 principles:
            - the highest priority is to satisfy the customer through early and continuous delivery of valuable software
            - welcome changing requirements, even late in development; Agile processes harness change for the customer’s competitive advantage
            - deliver working software frequently, from a couple of weeks to a couple of months, with a preference for the shorter timescale
            - business people and developers must work together daily throughout the project
            - build projects around motivated individuals; give them the environment, support, and tools and trust them to build
            - the most efficient and effective method of conveying information to and within a development team is face-to-face conversation
            - working software is the primary measure of progress
            - agile processes promote sustainable development; the them should be able to maintain a constant pace indefinitely
            - continuous attention to technical excellence and good design enhances agility
            - simplicity, or the art of maximizing the amount of work not done,  is essential
            - the best architectures, requirements, and designs emerge from self-organizing teams
            - at regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behavior accordingly
        - Several methodologies have emerged that take these Agile principles and define specific processes around them:
            - **Scrum**: a management framework that teams use to self-organize and work towards a common goal; it describes a set of meetings, tools, and roles for efficient project delivery, allowing teams to self-manage, learn from experience, and adapt to change; named from the daily team meetings, called scrums
            - **Kanban**: a visual system used to manage and keep track of work as it moves through a process; the word kanban is Japanese and roughly translated means "card you can see"; Kanban teams focus on reducing the time a project (or user story) takes from start to finish, using a kanban board and continuously improving their flow of work
            - **Rapid Application Development (RAD)**: an agile software development approach that focuses more on ongoing software projects and user feedback and less on following a strict plan, emphasizing rapid prototyping over planning
            - **Rational Unified Process (RUP)**: an agile software development methodology that splits the project life cycle into four phases:    
                    - inception: which defines the scope of the project and develop business case
                    - elaboration: Plan project, specify features, and baseline the architecture 
                    - construction: Building the product
                    - transition: providing the product to its users 
                - During each of the phases, all six core development disciplines take place: business modeling, requirements, analysis and design, implementation, testing, and deployment
            - **Agile Unified Process (AUP)**: a simplified version of the rational unified process, it describes a simple, easy to understand approach to developing business application software using agile techniques and concepts yet still remaining true to the RUP
            - **Dynamic Systems Development Model (DSDM)**: an agile project delivery framework, initially used as a software development method; key principles:
                - focus on the business need: DSDM teams establish a valid business case and ensure organizational support throughout the project
                - deliver on time: Work should be time-boxed and predictable, to build confidence in the development team
            - **Extreme Programming (XP)**:an Agile project management methodology that targets speed and simplicity with short development cycles, using five guiding values, five rules, and twelve practices for programming; the goal of the rigid structure, focused sprints and continuous integrations is higher quality product
    - **Waterfall**: 
        - Developed by Winston Royce in 1970, the waterfall model seeks to view the systems development lifecycle as a series of sequential activities
        - Traditional model has 7 stages, as each stage is completed, the project moves into the next phase; the iterative waterfall model does allow development to return to the previous phase to correct defects 
            - System requirements
            - Software requirements
            - Preliminary design
            - Detailed design
            - Code and debug
            - Testing
            - Operations and maintenance
        - A major criticism of this model is that it allows the developers to step back only one phase in the process
    - **DevOps (Development and Operations)**: an approach to software development, quality assurance, and technology operations that seeks to unite siloed staff, and bring the three functions together in a single operational model
        - closely aligned with the Agile development approach, DevOps aims to dramatically decrease the time required to develop, test, and deploy software changes
        - using the DevOps model, and continuous integration/continuous delivery (CI/CD), orgs strive to reach the goal of rolling out code dozens or even hundreds of times per day
        - this requires a high degree of automation, including integrating code repositories, the software configuration management process, and the movement of code between development, testing and production environments
        - the tight integration of development and operations also calls for the simultaneous integration of security controls
        - security must be tightly integrated and move with the same agility
    - **DevSecOps**: refers to the integration of development, security, and operations
        - DevSecOps supports the concept of software-defined security, where security controls are actively managed into the CI/CD pipeline

- 8.1.2 Maturity models (e.g., Capability Maturity Model (CMM), Software Assurance Maturity Model (SAMM))
    - the Software Engineering Institute (SEI) (Carnegie Mellon University) created the Capability Maturity Model for Software (AKA Software Capability Maturity Model, abbreviated SW-CMM, CMM, or SCMM)
        - all software development moves through a variety of maturity phases in sequential fashion, and CMM describes the principles and practices underlying software process maturity, intended to help improve the maturity and quality of software processes
        - note that CMM doesn't explicitly address security
        - stages of the SW-CMM:
            - Level 1: Initial: process is disorganized; usually little or no defined software development process
            - Level 2: Repeatable: in this phase, basic lifecycle management processes are introduced
            - Level 3: Defined: in this phase, software developers operate according to a set of formal, documented software development processes
            - Level 4: Managed: in this phase, there is better management of the software process
            - Level 5: Optimizing: in this phase continuous improvement occurs
    - Software Assurance Maturity Model (SAMM): an open source project maintained by the Open Web Application Security Project (OWASP)
        - provides a framework for integrating security into the software development and maintenance process and to offer orgs the ability to assess their maturity
        - SAMM associates software dev with 5 business functions:
            - Governance: the activities needed to manage software development processes
                - this function includes practices for:
                    - strategy
                    - metrics
                    - policy
                    - compliance
                    - education
                    - guidance
            - Design: process used to define software requirements and develop software
                - this function includes practices for:
                    - threat modeling
                    - threat assessment
                    - security requirements
                    - security architecture
            - Implementation: process of building and deploying software components and managing flaws
                - this function includes:
                    - secure build
                    - secure deployment
                    - defect management practices
            - Verification: activities undertaken to confirm code meets business and security requirements
                - this function includes:
                    - architecture assessment
                    - requirements-driven testing
                    - security testing
            - Operations: actions taken to maintain security throughout the software lifecycle after code is released
                - function includes:
                    - incident management
                    - environment management
                    - operational management
- 8.1.3 Operations and maintenance
- 8.1.4 Change management
- 8.1.5 Integrated Product Team (IPT)

[8.2](#8.2) Identify and apply security controls in software development ecosystems (OSG-9 Chpts 15,17,20,21)
- 8.2.1 Programming languages
- 8.2.2 Libraries
- 8.2.3 Tool sets
- 8.2.4 Integrated Development Environment (IDE)
- 8.2.5 Runtime
- 8.2.6 Continuous Integration and Continuous Delivery (CD/CD)
- 8.2.7 Security Orchestration, Automation, and Response (SOAR)
- 8.2.8 Software Configuration Management (SCM)
- 8.2.9 Code repositories
- 8.2.10 Application security testing (e.g., Static Application Security Testing (SAST), Dynamic Application Security Testing (DAST))


[8.3](#8.3) Assess the effectiveness of software security (OSG-9 Chpt 20)
- 8.3.1 Auditing and logging of changes
- 8.3.2 Risk analysis and mitigation

[8.4](#8.4) Assess security impact of acquired software (OSG-9 Chpts 16,20)
- 8.4.1 Commercial-off-the-shelf (COTS)
- 8.4.2 Open source
- 8.4.3 Third-party
- 8.4.4 Managed services (e.g. Software as a Service (SaaS), Infrastructure as a Service (IaaS), Platform as a Service (PaaS))

[8.5](#8.5) Define and apply secure coding guidelines and standards (OSG-9 Chpts 20,21)
- 8.5.1 Security weaknesses and vulnerabilities at the source-code level
- 8.5.2 Security of Application Programming Interfaces (APIs)
- 8.5.3 Security coding practices
- 8.5.4 Software-defined security
