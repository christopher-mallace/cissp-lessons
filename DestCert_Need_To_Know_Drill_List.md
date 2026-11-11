# DestCert CISSP — Need-to-Know Drill List

Source: DestCert Review Guides, all 8 domains, pulled from Christopher's DestCert account at new.my.destcert.com on Nov 10–11, 2026. Read-only extraction.

Coverage: 263 topics total — Domain 1: 34, Domain 2: 16, Domain 3: 71, Domain 4: 38, Domain 5: 31, Domain 6: 19, Domain 7: 36, Domain 8: 18.

What this is: every Core Concepts box and every blue side call-out, plus other explicit memorize / know directives, WITH the answer from the guide — steps in order, models, definitions, formulas, values, tables. Drill the prompt, then check yourself against the answer.

Gaps flagged in the file: a few items where the guide extract did not give the full detail, and topics that are video-only (no Guidebook, so no Core Concepts / blue blurbs exist). Nothing was invented to fill those gaps.

---

## DOMAIN 1 — SECURITY AND RISK MANAGEMENT (34 topics)

### 1.1.1 Ethics
- Memorize the wording and order of the Preamble and the Canons. Blue blurb: "How to apply Ethics Canons in a real-world situation."
- Preamble: the safety and welfare of society and the common good, duty to principals, and to each other, requires adherence to the highest ethical standards; strict adherence is a condition of certification.
- The 4 Canons, IN ORDER (apply in order; 1 is most important, then 2, etc.): 1. Protect society, the common good, necessary public confidence, and public safety; 2. Act honorably, honestly, justly, responsibly, and legally; 3. Provide diligent and competent service to principals; 4. Advance and protect the profession.
- Ethics = doing nothing harmful; codified in corporate laws/policies.

### 1.2.1 Focus of Security
- Core Concepts: protect assets; protecting data is primary; the three security goals are Confidentiality, Integrity, Availability (CIA); CIA prioritized by severity; data-center power 2N has no integrity implication.

### 1.2.2 CIA Triad
- Confidentiality, Integrity, Availability, plus Authenticity and Nonrepudiation (Parkerian Hexad + Utility).
- Authenticity vs Nonrepudiation: Authenticity = verify origin; Nonrepudiation = cannot deny after the action.
- Miller taxonomy: assets at risk, access, illegal use, etc.

### 1.3.1 Alignment of security function to business
- Alignment only assured in a top-down structure.
- Strategic (3–5 yr, upper management, set direction), Tactical (mid-level, implement direction), Operational (day-to-day technical, minimizes errors).
- 6 alignment components: knowledge, strategy, work products, respect, incentive, retention. Scoping vs Tailoring.

### 1.3.2 Accountability vs Responsibility
- Accountability cannot be delegated; Responsibility can.
- Ultimate accountability: Board/CEO, then VP Finance, etc. CSP is responsible for operating controls; customer/owner remains accountable.

### 1.3.3 Roles & Responsibilities
- Security as enabler, not hindrance. Owner/Controller, Processor, Custodian, Steward, Subject/Users.
- Custodian vs Owner table; security function provides tools, owners decide.

### 1.3.4 Due Care vs Due Diligence
- Due Care = accountable protection of assets; Due Diligence = ability to prove due care.
- Example: owner requiring regular pen tests = due care; the pen test itself = due diligence.

### 1.4.1 Licensing and IP
- Trade Secret — can protect indefinitely if secret kept (Coca-Cola recipe), information valuable, disclosure not required.
- Patent — 20 years from filing, full disclosure required, new/useful/non-obvious; source-code tradeoff: trade secret when keeping code private vs patent when wanting protection + disclosure.
- Copyright — life of author + 70 years, symbol not required under Berne, penalty up to $150,000 per infringement willful.
- Trademark — 10 years, renewable indefinitely, protection from brand confusion.

### 1.4.2 Import/Export Controls
- No Core Concepts box. Wassenaar Arrangement; ITAR — US State Dept / DDTC, US Munitions List, missiles/rockets/bombs; EAR — US Commerce / BIS, commercial including dual-use computers/lasers/marine.

### 1.4.3 Transborder Data Flow
- 3 challenges: laws, cultural differences, language.
- GDPR breach notification 72 hours; EU-US Privacy Shield, 2023 EU-US Data Privacy Framework, Standard Contractual Clauses, Binding Corporate Rules, adequacy decisions.

### 1.4.4 Privacy
- Privacy = individual right to be left alone / control personal information.
- Personal data = information relating to an identifiable individual, direct or indirect.
- Direct — Name, Phone, Gov ID (SIN/SSN/DL), Account numbers, Certificate/license, Biometric; Indirect — Age, Gender, Ethnicity, City, State, Zip/postal; Online — Email, IP, Cookies. Privacy laws vary local/national/international.

### 1.4.5 Privacy Requirements
- Supervisory authorities are independent authorities in each EU state investigating privacy complaints.
- GDPR 7 principles: Lawfulness/fairness/transparency, Purpose limitation, Data minimization, Accuracy, Storage limitation, Integrity/confidentiality, Accountability; breach 72h.
- OECD 8 principles: Collection Limitation, Data Quality, Purpose Specification, Use Limitation, Security Safeguards, Openness, Individual Participation, Accountability.
- Country laws: US GLBA, HIPAA, SOX, COPPA, CCPA, CPRA 2020; Canada PIPEDA; China PIPL; South Africa POPIA; Argentina PDPL 25,326; South Korea PIPA; Australia Privacy Act + APPs. Roles Owner/Custodian/Processor/Subject.

### 1.4.6 Privacy Assessments
- PIA goals: (1) identify/evaluate risks re privacy breaches, (2) identify controls to mitigate, (3) offer compliance. DPIA GDPR Art. 35, ISO/IEC 29134:2017.
- 8 PIA/DPIA steps IN ORDER: 1. Identify need, 2. Describe data processing, 3. Assess necessity/proportionality, 4. Consult interested parties (DPO, subjects, controllers, processors), 5. Identify and assess risks, 6. Identify measures to mitigate, 7. Sign off and record outcomes, 8. Monitor and Review (risk changes / high-risk new processing, also periodically).
- GDPR Art. 35 minimum DPIA: systematic description + purposes, necessity/proportionality assessment, risk assessment to rights/freedoms, measures including safeguards/security/mechanisms to ensure protection + demonstrate compliance.
- Frequency: annually, new processing, high risk, risk change.

### 1.4.7 Contractual/legal requirements
- Compliance Requirements: Laws, Regulations (ITAR, EAR), Industry Standards (NERC CIP, NIST), Import/Export, Transborder, Assets (see D2 2.1), Personal Data (1.4.5), Corporate Policies (1.6).
- Legal, privacy and audit work together; management + security implement controls; classification / approving access / retention-destruction.

### 1.5.1 Types of investigations
- VIDEO ONLY, no Guidebook; stated "Covered in Domain 7" (see Domain 7, 7.1).

### 1.6.1 Policies, Standards, Procedures, Baselines, Guidelines
- Policies = Corporate Laws, document/communicate management goals, overarching policy from upper management (tone from top); Procedures = step-by-step, mandatory; Standards = specific hardware/software solutions, e.g. McAfee AV, Forescout access control, Cisco ASA firewall, ISO 27001 adopted as standard; Baselines = defined minimal implementation levels, e.g. IDS/access-control configs; Guidelines = recommendations/suggestions.
- Policy model: create/maintain — roles, sign-off flow, review.

### 1.7.1 Business continuity (BCP)
- No Guidebook in Domain 1; stated "Covered in Domain 7" (see Domain 7, 7.11–7.13).

### 1.8.1 Personnel Security Controls
- Job rotation (fraud prevention, cross-training), Mandatory vacations (detect fraud, must take vacation), Separation of duties (prevent fraud, >1 employee for critical functions), Need-to-know / Least privilege (minimum permissions).
- Onboarding: identity proofing, signoff on policies/agreements, access per Least Privilege & Need-to-Know. Termination/Offboarding: timely removal of access, involuntary vs voluntary.
- Enforcement: Contracts/agreements, NDAs, Attestation/audit; NDA definition, noncompete, ethical questionnaires, vendor/consultant/contractor agreements.

### 1.9.1 Risk Management
- Steps: Value → Risk → Treatment.
- Value = identify assets, rank most to least valuable, quant/qual. Risk Analysis = Threat (any potential danger), Vulnerability (weakness exploitable), Impact (extent asset negatively affected), Probability/likelihood. Treatment = Avoid, Transfer, Mitigate, Accept. Every organization has limited resources.

### 1.9.2 Asset Valuation
- Before risks can be identified/managed, valuable assets must first be identified.
- Qual vs Quant: Qual = no monetary value, relative ranking, professional judgement, Low/Med/High, 1–5, simple/efficient; Quant = objective monetary values, fully quantitative when all elements quantified, difficult/time-consuming.

### 1.9.3 Risk Analysis
- Identify threats/vulns related to asset; understand probability/impact.
- Threat/Vuln examples: Natural/Env — Flood / building on floodplain; Human — Hacker / employees not trained, susceptible to social engineering; Operational/Process — highly susceptible to fraud e.g. issuing cheques / no segregation of duties; Technical — Malware / unpatched software; Physical — Power outage / no backup power.
- Terms: Threat Agent, Threat, Attack, Vulnerability, Risk, Asset, Exposure/Impact, Countermeasures & Safeguards, Residual Risk.
- Blue blurbs "Risk analysis steps" and "Calculating residual risk" — titles only in this section; no step list given there.

### 1.9.4 ALE Calculation
- ALE = SLE × ARO; SLE = AV × EF.
- ALE, SLE, AV (asset value), EF (exposure factor, % lost), ARO (annual rate of occurrence). Example CCTV AV $2,000. Control cost should not exceed risk cost.

### 1.9.5 Risk Response / Treatment
- Four approaches; risk can never be entirely eliminated.
- Avoid (stop doing risky thing; diving-board analogy — don't jump, opportunity cost: miss fun), Transfer (share with another party, usually insurance; get someone else to jump), Sharing is a subcomponent of transfer, Mitigate (controls reduce to acceptable level; jump from lower board), Accept (take no action; must always be asset owner/senior management — accountable; just jump from top). Risk ignorance is NOT viable.

### 1.9.6 Types of Controls
- VIDEO ONLY, no Guidebook.

### 1.9.7 Categories of Controls
- Safeguards = proactive (before), Countermeasures = reactive (after); categories Administrative, Physical, Logical/Technical.
- Directive — Policy/Procedure, Configuration Standards, "Authorized Personnel Only" signs / Traffic Lights; Deterrent — Guideline, Warning banner, "Beware of Dog" signs; Preventative — User registration, Login mechanism (security kernel)/OS restrictions, Fence / RFID badges; Detective — Review violation reports, SIEM, CCTV; Corrective — Termination, Unplug/isolate/terminate connection, Fire suppression; Recovery — DR Plan, Backups, Rebuild; Compensating — Supervision/Job Rotation/Logging, CCTV/Keystroke Logging, Layered Defense.

### 1.9.8 Functional & Assurance
- VIDEO ONLY, no Guidebook (video title "Categorizing Controls" 6:20).

### 1.9.9 Selecting Controls
- Controls must support org goals, must be cost effective. Criteria: Alignment, Cost-effectiveness (cost-justified), Complete control (preventive+detective+corrective minimum), Functional and assurance effectiveness.
- Measuring: metrics; senior management most interested in… Continuous Improvement Deming Cycle Plan-Do-Check-Act: Plan — determine controls based on risks; Do — implement; Check — monitoring/assurance, are controls operating effectively?; Act — based on findings, take additional actions.
- Risk analysis frequency: as often as necessary, depends on nature. Blue blurb: "How to determine if a control should be implemented".

### 1.9.10 Supply Chain Risk
- VIDEO ONLY, no Guidebook.

### 1.9.11 Risk Frameworks
- NIST SP 800-37 RMF, ISO 31000, COSO ERM, ISACA Risk IT.
- RMF 7 steps IN ORDER: 1. Prepare to execute RMF, 2. Categorize Information Systems, 3. Select Security Controls, 4. Implement Security Controls, 5. Assess Security Controls, 6. Authorize Information System, 7. Monitor Security Controls.

### 1.10.1 Threat Modeling Methodologies
- Threat modeling = systematic identify/enumerate/prioritize threats.
- STRIDE: Spoofing-Authentication, Tampering-Integrity, Repudiation-Non-repudiation, Information Disclosure-Confidentiality, DoS-Availability, Elevation of Privilege-Authorization.
- PASTA 7 stages: 1. Define Objectives, 2. Define Technical Scope, 3. Application Decomposition, 4. Threat Analysis, 5. Vulnerability & Weakness Analysis, 6. Attack Modeling, 7. Risk & Impact Analysis.
- DREAD 1–10: Damage, Reproducibility, Exploitability (guide spells "Expoiltability"), Affected Users, Discoverability.

### 1.10.2 Anything related to social engineering
- Social engineering = manipulation through intimidation and/or deception; prevalent means of attack; best combat = awareness/education/training.
- Tactics: intimidation (inducing fear), deception (tricking), rapport (gradual relationship).
- Phishing, Spear Phishing, Whaling, Smishing, Vishing, Pretexting, Baiting (USB etc.), Tailgating/Piggybacking.
- Mitigations: awareness/training, requesting proof of identity, requiring callback authorization for voice/text-only requests for network alterations/sensitive info, etc.

### 1.11.1 SLR, SLA and Service Level Reports
- SLR contents: detailed service descriptions, detailed service level targets, mutual responsibilities.
- SLA contents: Service Levels, Governance, Security, Compliance, Liability/Indemnification.
- Service Level Reports: Achievement of metrics defined in SLA, Identification of issues, Reporting channels, Management, Third-party SOC reports.

### 1.11.2 Risks in Acquisition
- No Core Concepts box. Product Tampering, Counterfeits, Implants.
- Mitigations: Third-party assessment and monitoring, Minimum security requirements, Silicon root of trust, Physically unclonable function (PUF), SBOM (comprehensive list components/libraries/modules).

### 1.12.1 Awareness Training Education
- No Core Concepts box. Awareness vs Training vs Education: Awareness — How to identify activity etc., broad communications to 100% audience; Training — How to perform tasks, guidance process, targeted attendees, simulations; Education — Why tasks performed, academic, students, degrees.

---

## DOMAIN 2 — ASSET SECURITY (16 topics)

### 2.1.1 Asset Classification
- Classification policies/procedures/processes help achieve proper protection based on value; common problem: orgs don't know what assets they have; balancing cost; proper classification ensures appropriate level based on value.
- Benefits: identification of critical information, sensitivity to modification, commitment to protect valuable assets, commitment to confidentiality where applicable.

### 2.1.2 Classification Process
- Begins with asset inventory; owners determine classification; ongoing process. Classify on CIA: confidentiality/sensitivity, integrity/accuracy, availability/criticality.
- Owners overprioritize then underclassify when cost; solution: committee/working group + consistent scoring system vetted by board/committee.
- Steps: inventory → owner identified → owner classifies by value → protect/handle by level → periodic review/assessment (value changes, assets added/removed, owners change, laws change). Blue blurb: "Asset classification steps".

### 2.1.3 Classification vs Categorization
- Classification = system of classes ordered according to value; Categorization = act of sorting into defined classifications.
- Examples: Top secret, secret, confidential, sensitive but unclassified, unclassified; Financially sensitive; Company restricted; Proprietary; Trade secret; PII. Different orgs, same terminology, different corresponding protection.

### 2.1.4 Marking & Labeling
- Labeling = classification, system-readable; Marking = handling instructions, human-readable; consistently applied to all assets; labeling cost-effective.
- Labeling — system-readable, association of security attributes with subjects/objects in internal data structures, enables system-based enforcement; Marking — human-readable, association with objects in human-readable form, enables process-based enforcement.
- Labeling approaches: Metadata, Barcodes, QR codes, RFID tags, GPS tags.

### 2.2.1 Media Handling
- Handling based on classification, not media type; Owners determine who may access media, especially sensitive.
- Storage/Retention: PCI DSS audit log retention minimum 1 year, 90 days immediately available; destroy card info as soon as no longer required.

### 2.3.1 Data Owners
- Owners accountable; assignment drives classification. Owner = person who directly interacts most, best understands value; IT is not owner.
- Owner accountabilities: classifying/categorizing, managing access, ensuring appropriate controls based on classification; can delegate responsibility, never accountability.
- Owner types: Data, Process, System, Product, Service, Hardware, Applications, IP, etc.
- Owner/Controller — accountable, legal rights, defines policies; Processor — responsible for processing on behalf of owner/controller (cloud provider); Custodian — technical responsibility (security, availability, capacity, continuity, backup/restore); Steward — business responsibility (metadata, data quality, governance, compliance); Subject — individual to whom personal data pertains.

### 2.3.2 Data Classification Policy
- Policy concerned with management of information to ensure sensitive/valuable protected/handled accordingly; considers laws, regulations, privacy, customer requirements, cost of creation, operational impact, liability, reputation.
- Should: start with asset policy which drives classification policy; be accompanied by retention, destruction, archiving policies; clearly define accountability/responsibility; define varying forms asset media (digital, tape, paper); include all factors that drive value → determine protection; outline asset liability / consequences regulatory oversight; describe industry standards / impact reputation; involve security consulting/expertise, owners drive process.
- Value factors: 1. Laws/regulations, 2. Privacy, 3. Creation cost, 4. Operational impact, 5. Liability, 6. Reputation.

### 2.4.1 Data Roles
- VIDEO ONLY, no Guidebook.

### 2.4.2 Information Life Cycle
- Data must be protected at each phase. Stages: Create (generation of new digital content, or alteration/updating/modifying existing), Store (committing to storage repository, nearly simultaneous with create), Use (viewed/processed/used, not including modification), Share (made accessible to others — users/customers/partners), Archive (leaves active use, long-term storage), Destroy (permanently destroyed physical/digital, e.g. cryptoshredding).

### 2.4.3 Data Destruction
- Data remanence = residual representation after attempts to securely delete. Categories of sanitization — destruction, purging, clearing; secure removal in cloud.
- Destroy — physical destruction, most effective; Purge — logical/physical, data cannot be reconstructed; Clear — logical, data may be reconstructed, least effective.
- NIST SP 800-88 Rev1 (most to least effective): Media Destruction (Incinerate), Shred/Disintegrate/Drill, Degauss (strong magnetic field to magnetic media), Encryption (Crypto Shredding/Erase), Overwrite/Wipe/Erasure (write all zeroes/ones/combination), Format — least effective.
- Object reuse: overwriting = 'clearing' NOT 'purging'. SSD: data remanence problems, some manufacturers provide sanitization/crypto erasure, best option always physical destruction. Encryption: crypto shredding best method for data remanence in Cloud (physical destruction best but costly/unavailable/infeasible, so crypto shredding).

### 2.5.1 Data Archiving
- Archiving requirements: media type, security, availability, retention period, associated costs.
- Policy: based on laws/regulations/industry standards/business needs, classify records accordingly, educate employees + tools. Questions: Who needs access? Do access requirements change over time? How long kept? Disposal requirements?

### 2.6.1 Protecting Data at Rest
- Methods: encryption, access control, backup/restoration. Data at rest = stored somewhere, files on hard drive, etc.
- As orgs migrate to cloud, data should first be encrypted. Best way to protect confidentiality of data being migrated to cloud: encryption before migration.

### 2.6.2 Protecting Data in Transit
- Methods: end-to-end, link, onion network. Data in transit = data in motion moving across networks internal/internet.
- End-to-End: data portion of packet encrypted immediately upon transmission. Link: packet header AND data encrypted between each node; hides routing info; performed by service providers. Onion: very effective, anonymity + protection, confidentiality + anonymity, difficult to determine sender/receiver.

### 2.6.3 Information Obfuscation
- Obfuscation/masking makes something harder to understand. Concealing data (completely removes access…), Information Pruning (nonproduction, removal…), Fabricating data (fake data replace real, full functional testing; prevents unauthorized access/viewing actual), Trimming data (removes part of attribute value), Encrypting data (ciphertext, attribute/table/database levels).

### 2.6.4 Scoping & Tailoring
- VIDEO ONLY, no Guidebook.

### 2.6.5 DLP, DRM, IRM & CASB
- DRM protects IP/rights owners; Legal basis US DMCA. DLP identification/monitoring/protection; DLP 3 contexts: in use / in motion / at rest.
- DRM NIST SP 500-241: system of IT components/services + law/policy/procedures to ensure rights holders can use content, protect content IP. IP includes movies, video games, digital music, eBooks, cable/satellite.
- DRM techniques: Licensing agreements restrict access, Encryption, Embedding digital tags tie content to license holders, related tech restrict copying/viewing. DMCA 1998 US. IRM subset of DRM.
- DLP NIST: system's ability to identify/monitor/protect data in use (endpoint), in motion (network), at rest (storage).

---

## DOMAIN 3 — SECURITY ARCHITECTURE AND ENGINEERING (71 topics)

### 3.1.1 Security in Design and Build
- Security must be involved in all phases of designing/building, from beginning to end. Architecture = building/design/diagram/structure; Security architecture = each individual component must be secured/protected; Enterprise security architecture = entire organization, protect each component based on value; Engineering = designing/building a solution walking through a series of steps/processes.

### 3.1.2 Secure Design Principles
- Examples: Threat modeling, Least privilege, Defense in depth, Secure defaults, Fail securely, Separation of duties, Keep it simple and small, Zero trust and trust but verify, Privacy by Design, Shared responsibility, Secure access service edge (SASE).
- Zero Trust, 8 principles: 1. Know your architecture, 2. Know your user/service/device identities, 3. Know health of users/devices/services, 4. Use policies to authorise requests, 5. Authenticate everywhere, 6. Focus monitoring on devices/services, 7. Don't trust any network including your own, 8. Choose services designed for zero trust.
- Privacy by Design, 7 principles: Proactive/preventive not reactive/remedial; Privacy as default; Privacy embedded into design; Full functionality – positive-sum; End-to-End Security; Visibility and Transparency; Respect for User Privacy.
- Cyber Kill Chain, 7: Reconnaissance, Weaponization, Delivery, Exploitation, Installation, Command and control (C&C), Actions.

### 3.2.1 Security Models Importance
- Model = representation of something real; Security model = representation of what security should look like in an architecture. Protection must break architecture into individual components, each protected according to value.

### 3.2.2 Enterprise Security Architecture
- Frameworks: Zachman (1970s, how/where/who/when/why), SABSA 1995 (security architecture risk, embed security in IT, open-source, scalability, compliance, response prioritization), TOGAF (efficient resource utilization, cost minimization, modular, content framework consistency, architectural flexibility).
- Layer/Lattice-based — Bell-LaPadula, Biba; Rule-based — Information Flow, Clark-Wilson, Brewer-Nash (Chinese Wall), Graham-Denning, Harrison-Ruzzo-Ullmann.

### 3.2.3 Layer Based Models
- Layer = lattice; Bell-LaPadula only confidentiality; Biba only integrity; Lipner is not a model, an implementation combining the best of both.
- Bell-LaPadula: 1. Simple security "no read up"; 2. Star (*) "no write down"; 3. Strong star — both read+write, subject should only read/write at same level.
- Biba: 1. Simple integrity "no read down"; 2. Star integrity "no write up"; 3. Invocation — subject can't send info to someone rated at a higher layer.

### 3.2.4 Rule Based Models
- Info flow models track flow, uncover covert channels; Covert channels unintentional, storage + timing; Clark-Wilson integrity, 3 goals + 3 rules; Brewer-Nash Chinese Wall prevents conflicts of interest.
- Covert: Storage — process writes sensitive data to RAM, remains after process completes; Timing — web server responds to existing username within 3 sec, while non-existing differs.
- Clark-Wilson goals: 1. Prevent unauthorized subjects making any changes, 2. Prevent authorized subjects making bad changes, 3. Maintain consistency.
- Clark-Wilson rules: Well-Formed Transactions; Separation of Duties; Access Triple Subject|Program|Object — subject cannot directly access object, must go through program.
- Brewer-Nash: info flow, primary goal prevent conflicts, like Bell-LaPadula addresses confidentiality. Graham-Denning, Harrison-Ruzzo-Ullman: rule-based integrity. Remember all security models are either lattice-based or rule-based.

### 3.2.5 Certification & Accreditation
- Certification = comprehensive technical analysis confirm meets desired needs; Accreditation = management official sign-off for predetermined time.

### 3.2.6 Evaluation Criteria ITSEC & TCSEC
- TCSEC Orange Book first; ITSEC followed, Europeans, includes Orange Book + other; ITSEC networked, measures functional and assurance separately.
- Orange Book high→low: A1 Verified design; B3 Security labels, verification no covert channels, must stay secure during start-up; B2 Security labels + verification no covert channels; B1 Security labels; C2 Strict login procedures; C1 Weak protection; D1 Failed / not tested. Only measures confidentiality, single-box.
- ITSEC: E6 Formal end-to-end + source code reviews; E5 Semiformal system+unit tests + source code review; E4 Semiformal system+unit tests; E3 Informal system+unit tests; E2 Informal system tests; E1 System in development; E0 Inadequate assurance. Replaced by Common Criteria in 2005.

### 3.2.7 Common Criteria (Importance 5/5)
- "Memorize the Common Criteria steps." Best/most popular evaluation system; globally recognized rating; EAL rating levels. ISO 15408, most used.
- Process steps IN ORDER: 1. PP Protection Profile — specification of functional and assurance requirements for a specific type of security product; 2. TOE Target of Evaluation — specific product/system to be evaluated; 3. ST Security Targets — written statement by vendor explaining how functional and assurance specs of product meet…; 4. Security Functional Requirements — ST evaluated functionally; 5. Security Assurance Requirements — ST evaluated from assurance perspective; 6. Evaluate — consider all components together; 7. Assign EAL (1–7).
- EAL high→low: EAL7 Formally verified, designed, and tested; EAL6 Semi formally verified, designed, & tested; EAL5 Semi formally designed and tested; EAL4 Methodically designed, tested, and reviewed; EAL3 Methodically tested and checked; EAL2 Structurally tested; EAL1 Functionally tested. Notes: EAL7 not necessarily best; higher complexity → more vulnerable; after evaluation, if patched/upgraded, EAL level remains same [as the guide states].

### 3.3.1 Security Control Frameworks
- COBIT (IT governance/assurance, audits/gap, ISACA), ITIL (processes well-run IT dept), NIST SP 800-53 (best practice controls for federal systems), PCI DSS (credit cards), ISO 27001 (international, certifiable, Annex A 14 domains: 1 Information Security Policies, 2 Organization of Information Security, 3 Human Resource Security, 4 Asset Management, 5 Access Control, 6 Cryptography, 7 Physical and Environmental Security, 8 Operations Security, 9 Communications Security, 10 Systems Acquisition, Development and Maintenance, 11 Supplier Relationships, 12 Incident Management, 13 Business Continuity Management, 14 Compliance), ISO 27002 guidance implementing ISO 27001 controls, COSO, HIPAA (PHI), FISMA 2002, FedRAMP, SOX. Understand major frameworks at high level, especially ISO 27001/02.

### 3.4.1 RMC, Security Kernel and TCB
- RMC is a concept; implementation of RMC is security kernel; Security kernel 3 properties: completeness, isolation, verifiability; TCB = all protection mechanisms within architecture.
- Subjects = active entities; Objects = passive. RMC: Must mediate all access, Be protected from modification, Be verifiable as correct, Always be invoked.
- Completeness — Impossible to bypass; Isolation — Mediation rules tamperproof; Verifiability — Logging/monitoring/testing ensure functioning correctly. TCB components: Processors, Memory, Primary storage, Secondary storage, Virtual memory, Firmware, Operating systems, System kernel.

### 3.4.2 Processors (CPUs)
- CPU: 4-step Fetch, Decode, Execute, Store; 2 states supervisor/problem. Supervisor — Higher privilege, typically system kernel, full access; Problem — Lower privilege, limited access, standard operating mode.

### 3.4.3 Process Isolation
- Two primary methods memory segmentation and time-division multiplexing. Memory segmentation ensures memory assigned to one app only accessible by that app. Time-division: CPU allocates very small time slots to each process.

### 3.4.4 Types of Storage
- Primary — Fast, Volatile, Small, Cache/Registers/RAM. Secondary — Slow, Non-volatile, Large, Magnetic drives, Optical media, Tapes, SSD. Virtual memory when RAM fills up.

### 3.4.5 Firmware & System Kernel
- System kernel is core OS with complete control; System kernel ≠ security kernel (security kernel = implementation of reference monitor); Relies on privilege levels.

### 3.4.6 Privilege levels
- User mode lower trust, small subset; Privileged/kernel mode higher trust, more capabilities; Ring protection model. Ring 0 most critical. GAP: assignments beyond Ring 0 were not fully transcribed — guide extract did not give full detail there.

### 3.4.7 Middleware
- Intermediary between two applications; speaks languages of two disparate applications to facilitate communication; enables interoperability (glue).

### 3.4.8 Abstraction & Virtualization
- Abstraction = underlying complexity/details hidden. Virtualization extends computing example further. Hypervisor layer.

### 3.4.9 Layering / Defense in depth
- Protection never rely on just one control; multiple layers, control at each layer.

### 3.5.1 Vulnerabilities in Systems
- SPOF, TOCTOU race condition short window between check and use, emanations. Emanation Protection: Shielding (TEMPEST) — Walls, Faraday cages, copper-lined envelopes; White Noise — strong random noise; Control Zones — prevent access/proximity.

### 3.5.2 Hardening
- Secure each component to reduce overall vulnerability. Examples: AV, host IDS/IPS + firewall, device config reviews, full-disk encryption, strong passwords, routine backups, logging/monitoring.

### 3.5.3 Risk in Mobile Systems
- MDM/MAM; reduce risk: Policies, lost/stolen process notify + remote wipe, remote access VPN+2FA by default, endpoint AV/malware DLP, app whitelisting.

### 3.5.4 OWASP Mobile
- OWASP Mobile Top 10: M1 Improper Credential Usage, M2 Inadequate Supply Chain Security, M3 Insecure Authentication/Authorization, M4 Insufficient Input/Output Validation, M5 Insecure Communication, M6 Inadequate Privacy Controls, M7 Insufficient Binary Protections, M8 Security Misconfiguration, M9 Insecure Data Storage, M10 Insufficient Cryptography.
- MSTG = Mobile Application Security Testing Guide, MASVS = Mobile Application Security Verification Standard. Blue blurbs: "What are top vulnerabilities on mobile devices?" and "What is OWASP Mobile Security Testing Guide?"

### 3.5.5 Distributed Systems
- DFS files spread multiple hosts shared via network; Grid systems interconnected working together to solve a specific usually very complex problem. Blue blurb: "What is an underlying risk related to distributed file systems (DFS)?" GAP: full DFS risk wording was not completely captured. Grid risk: data integrity/validation; inappropriate use.

### 3.5.6 Inference & Aggregation
- Data warehouse: analytics from multiple sources, SPOF availability + confidentiality risk. Big Data: Variety, Volume, Velocity. Tools Hadoop, MongoDB, Tableau. Aggregation = collecting/combining data for statistical analysis; Inference = deducing info from evidence/reasoning rather than explicit statements. Reduce risk: polyinstantiation.

### 3.5.7 Industrial Control Systems
- ICS: 3 types SCADA, DCS, PLC; best reduce risk: keep offline — air gap. OT broader than ICS, ICS subset of OT. Alternatives: nonstop logging/monitoring/anomaly detection, regular vuln assessments, VLANs/zoning, privileged access management.

### 3.5.8 Internet of Things (IoT)
- Devices like home appliances connected to internet; risky; reduce risk via purchase decisions, precautions installing, keeping tech up to date. DDoS context (IoT botnets).

### 3.5.9 Cloud Computing Characteristics
- 6 characteristics: on-demand self-service, broad network access, resource pooling, rapid elasticity/scalability, measured service, multitenancy.

### 3.5.10 Cloud Service & Deployment Models
- Service models IaaS, PaaS, SaaS, CaaS, FaaS; Deployment Public, Private, Community, Hybrid. SaaS rented app; IaaS virtual data center; PaaS custom app marketplace; CaaS container; FaaS serverless/microservices.
- Shared responsibility always, customer always accountable for data/assets in cloud. Public — Third-party, Off-premises, Everyone (Untrusted); Private/Community — Org or third-party, On- or off-premises, Trusted; Hybrid — Both, Both, Both.
- Blue blurb: "What should be a primary concern of an organization considering a move to the cloud?" — protection/privacy of data.

### 3.5.11 Cloud Computing Roles
- Consumer, provider, partner, broker; consumer always accountable; responsibility can be delegated; controller=owner=customer=accountable; processor=cloud provider/other agent=responsible.
- Accountability — where the buck stops, only one entity can be accountable, sets rules; Responsibility — the doer, multiple entities can be responsible, develops plans/makes things happen.

### 3.5.12 Hypervisors and VMs
- Hypervisor = VMM, allows multiple OS to share single physical machine. Best point of attack for multiple VMs: compromising hypervisor.
- VM Pros — isolated security, heavy stand-alone; Cons — time, storage, admin overhead. Containers Pros — lightweight/efficient, portable, less overhead; Cons — share same OS/infra, public containers could be malicious.

### 3.5.13 Containers
- No Core Concepts box. Monolithic — all functionality wrapped in single unit; Microservices — divided into smaller self-contained services.

### 3.5.14 Serverless
- FaaS/serverless = microservices in cloud, AWS Lambda, no server provisioning, only actual compute time charged, zero cost if unused.

### 3.5.15 Cloud Migration & Protocols
- Vendor lock-in significant risk. Blue blurb: "Among cloud migration risk, what is one of the most important things to consider?" — vendor lock-in.

### 3.5.16 Edge Computing, Embedded & HPC
- No Core Concepts box. Edge computing distributed, reduce latency, processing closer to source. Ingress (traffic entering), Egress (traffic exiting), Peering (interconnection of separate networks without Internet). SASE pronounced "sassy".

### 3.5.17 XSS & CSRF
- XSS malicious script injected into trusted website; CSRF relies on persistence facilitated by cookies; XSS target user's browser; CSRF target web server.
- Persistent/Stored — code stored on server; Reflected — code passed via URL, most common; DOM-based — client-side DOM modified. Best prevention server-side input validation.

### 3.5.18 SQL Injection
- Input validation best prevention. Example: ' OR 1=1 -- . Mitigation: validate/sanitize, prepared statement/parameterized queries + stored procedures.
- SQL commands DO NOT need to be memorized (explicit in guide), but be able to recognize SQL code: CREATE ALTER DROP TRUNCATE RENAME; SELECT INSERT UPDATE DELETE MERGE LOCK TABLE; GRANT REVOKE; COMMIT ROLLBACK SAVEPOINT.

### 3.5.19 Input Validation
- Server-side validation reduces web vulnerabilities + XSS/SQLi risk; Whitelist only allows acceptable input.
- Blue blurbs: "What is best way to mitigate web-based vulnerabilities?" — server-side input validation, prevents XSS/SQLi. "What is risk associated with client-side input validation?" — client-side may be bypassed. Deny list (blacklist) discards malicious characters.


### 3.6.1 Intro to Cryptography
- History ~4000 years; most critical = key management; 5 services confidentiality, integrity, authenticity, nonrepudiation, access control.
- Evolution: Manual, Mechanical, Electro-mechanical, Electronic, Quantum (experimental).
- Confidentiality — prevent unauthorized disclosure; Integrity — ensure not manipulated; Authenticity — verify message came from particular sender; Nonrepudiation — Origin sender cannot deny sent, Delivery receiver cannot deny received; Access Control — controlling distribution of ciphertext.

### 3.6.2 Cryptographic Terminology
- Plaintext/cleartext readable; Encrypt plaintext→ciphertext; Key string of bits, secret; Key clustering avoid; Work factor — estimated time/effort to break, higher more secure; IV/nonce — random number with key prevent patterns (GAP: weaknesses detail not fully captured); Confusion — key→ciphertext, 1 bit key change ~half ciphertext bits change; Diffusion — plaintext→ciphertext, 1 bit plaintext change ~half bits change; Avalanche — degree of confusion+diffusion; Key Space — 2-bit = 4 keys; DES 56-bit = 2^56 keys; today symmetric 128- or 256-bit.

### 3.6.3 Substitution & Transposition
- Substitution GUBBINS>JXEELQV, Transposition GUBBINS>BINBUGS; Frequency analysis: E most common letter, "the" most common 3-letter, "that" most common 4-letter; One-time pad only unbreakable if used correctly, key never reused.
- Stream 1 bit at a time, faster, RC4; Block chunks, AES 128-bit block, more versatile slower.
- Block modes: ECB least secure no IV fastest, only short random non-repeating e.g. PIN; CBC uses IV good email; CFB uses IV good email; OFB uses IV good email; CTR uses counter, almost most secure + fast, best balance, most commonly used.

### 3.6.4 Symmetric Cryptography
- Fast; disadvantages key distribution/scalability; Scalability formula n×(n−1)/2 keys, 1,000 people = 499,500 keys. Advantages: Fast/efficient, Strong; Disadvantages: key distribution, scalability, no authenticity/integrity/nonrepudiation.
- Weakest→strongest (key, block): RC2-40 (40, 64), DES (56, 64), RC5-64/16/7 (56, 128), RC5-64/16/10 (80, 128), Skipjack (80, 64), RC2-128 (128, block shown as "8?" — unclear in extract), RC5-64/12/16 (128, 128), IDEA (128, 64), Blowfish (128, 64), 3DES (168=112 effective, 64), RC5-64/12/32 (256, 128), Twofish (256, 128), RC6 (256, 128), Rijndael/AES (128/192/256, 128). DES: 56-bit key, 16 rounds, 64-bit block, 3DES effective 112 bits (not 168).

### 3.6.5 Asymmetric Cryptography
- Solves key exchange, enables signatures/certs/authenticity/nonrepudiation, key pairs public+private, hard math factoring & discrete logs, RSA factoring, ECC discrete log shorter keys same security, Diffie-Hellman discrete log.
- Confidentiality = receiver's public key encrypt; Authenticity/proof of origin = sender's private key encrypt / sign.

### 3.6.6 Hybrid Key Exchange
- Diffie-Hellman (discrete logs) asymmetric used primarily for symmetric key exchange. Hybrid: Alice encrypts symmetric key with Bob's public key, Bob decrypts with private, then symmetric for message. DH example result 42 in guide example.

### 3.6.7 Steganography & Null Ciphers
- Steganography hiding info within something else; Null cipher hiding plaintext within another plaintext. Slack space leftover storage.

### 3.6.8 Message Integrity Controls
- Hashing very effective MIC, fixed length output. Hashing properties: Fixed length, One-way, Deterministic, Calculated on entire message, Uniformly distributed, Collision resistant.
- Hash algorithms: MD5 128-bit, SHA-1 160-bit, SHA-2 224/256/384/512, SHA-3 224/256/384/512. Birthday paradox illustrates collisions.

### 3.6.9 Digital Signatures
- Provide integrity, authenticity, nonrepudiation. Creating: 1. hash message, 2. sign hash with sender's private key. Verifying: verify signature with public key, hash received message, compare hashes.

### 3.6.10 Digital Certificates
- Bind individual to public key; all CAs conform X.509; root of trust = root CA. Creation: 1. Alice generates file with info/public key, 2. sends to CA, 3. CA confirms identity, 4. CA signs with CA private key.
- Replacement — regular replacement of expired certs; Revocation — when private key compromised. CRL — client downloads/searches list of revoked serials; OCSP — client queries CA for specific serial, better/newer.
- Life cycle: Enrollment (CSR), Issuance (RA identity proofing), Validation, Revocation, Renewal (~12 months). Certificate Pinning: coding cert into app / pin on first visit.

### 3.6.11 Public Key Infrastructure
- Standard X.509; components: CA — Root of trust; RA — Identity proofs on behalf of CA; Intermediate/Issuing CA — Issues certs on behalf of CA; VA — Responds to revocation queries; Certificate DB — List of certs issued + revocation list; Certificate Store — Repository of certs + user's private key. Without PKI cannot verify identity of sender.

### 3.6.12 S/MIME
- Requires PKI. Services: Authentication, Nonrepudiation of origin, Message integrity, Confidentiality; Optional: Signed receipts, Security labels, Secure mailing lists.

### 3.6.13 Key Management
- Kerckhoffs principle (system secure even if everything except key public); activities: generation, distribution, storage, change/rotation, disposition/destruction, recovery.
- Distribution — out-of-band + key wrapping KEK; Storage — TPM (chip on motherboard) vs HSM (physical network device for many devices); Destruction — crypto shredding + key destruction; Recovery — split knowledge, dual control (two keys same time), key escrow (trusted third party).

### 3.6.14 Putting Cryptography Together
- Video summary only, no Guidebook.

### 3.7.1 Cryptanalysis Importance
- Main purpose deduce key. Cryptanalytic: Ciphertext only, Known plaintext, Chosen plaintext, Chosen ciphertext, Linear and Differential, Factoring. Cryptographic: Man-in-the-middle, Replay, Temporary files, Implementation, Side channel, Dictionary, Rainbow table, Birthday, Social engineering.

### 3.7.2 Cryptanalytic Attacks
- Brute-force typically not effective unless key very short (56 bits or less). Ciphertext only — most difficult; Known plaintext — pair available; Chosen plaintext — plaintext attacked; Chosen ciphertext — ciphertext attacked. Easiest = chosen plaintext/ciphertext.

### 3.7.3 Cryptographic Attacks
- MITM, Replay, Pass-the-Hash, Temporary Files, Implementation, Side Channel (Timing, Radiation Emissions, Power), Dictionary, Rainbow Tables (reduce risk salt), Birthday, Social engineering, Kerberos golden (forged TGT) / silver (forged TGS) tickets, Ransomware, Fault injection.

### 3.8.1 Intro to Physical Security
- Primary goal safety/protection human life. Physical Controls: Deter/Prevent, Delay, Detect, Assess, Respond. Threats: Theft, Espionage, Dumpster diving, Social engineering, Shoulder surfing, HVAC. Blue blurb: "Know the primary goal of physical security" — safety/protection of human life.

### 3.8.2 Layered Defense Model
- Least valuable outside, most valuable centre.

### 3.8.3 Security Survey
- Threat Definition, Target Identification, Facility Characteristics; Life (number one priority), Property, Operations. High-Value Areas: Wiring Closets, Media Storage, Evidence Storage, Server Rooms, Restricted Work Areas. CPTED.

### 3.9.1 Perimeter Importance
- Landscaping, grading (slope away), fences, gates, bollards. Less access points, better security.

### 3.9.2 CCTV
- Primarily detective, also deter/monitor. Blue blurb: "What primary type of control are CCTV cameras?" — detective.

### 3.9.3 Passive Infrared Devices
- PIR detects motion by infrared light; sensitive to temperature; must recalibrate. Blue blurb: "How a passive infrared device works".

### 3.9.4 Lighting
- Deterrent + safety; allows CCTV better visibility.

### 3.9.5 Doors
- Mantraps prevent tailgating/piggybacking. Blue blurb: "What do mantraps prevent?" — tailgating.

### 3.9.6 Locks
- Locks delay not prevent; mechanical/electronic. Blue blurb: "What determines security of a combination lock?" — complexity of combination.

### 3.9.7 Windows
- Shock sensors vibrations useful noisy; Sound/frequency useful quiet; Glass break microphones tuned to glass. Blue blurb: "What type of sensor is effective in a noisy environment?" — shock sensors.

### 3.9.8 Walls
- Wall should extend floor to true ceiling, not drop ceiling; data centers raised floors, walls extend actual floor to true ceiling.

### 3.9.9 Skimming
- Antitampering best to prevent. Detect: 1. Pull keypad/card insert, 2. Look at spelling, 3. Errors during transaction could be a sign.

### 3.9.10 Power
- Short (ms) vs Long: No power — Fault / Blackout; Not enough — Sag/Dip / Brownout; Too much — Spike / Surge.

### 3.9.11 HVAC
- ASHRAE: Temperature 64.4°F / 18°C to 80.6°F / 27°C; Humidity 40% to 60% RH. Positive pressurization keeps contaminants out. Humidity too low static, too high condensation corrosion/shorts.

### 3.9.12 Fire
- Requires fuel, oxygen, heat. Detection: Flame (IR/UV), Smoke Ionization (faster flaming), Photoelectric (faster smoldering), Dual, VESDA (most expensive, very early, incipient), Heat rate-of-rise.
- Water: Wet pipe — filled always, leaks/freeze risk; Dry pipe — not filled; Pre-action — detection triggers, eliminates false activation damage; Deluge — massive water at once, all heads open.
- Gas: INERGEN, Argonite (argon+nitrogen), FM-200 (clean agent safe for humans), Aero-K. Halon illegal never use.
- Extinguishers: A common combustibles — Water, foam, dry chemicals; B liquid — Gas, CO2, foam, dry chemicals; C electrical — Gas, CO2, dry chemicals; D combustible metals — Dry powders; K commercial kitchens — Wet chemicals. CO2: too much can kill, removes oxygen.

### 3.10.1 IS Lifecycle Importance
- No Core Concepts box. IS lifecycle = system life cycle in 8.1.2, slight difference in steps/names; Integration testing is part of development, verification and validation are parts of overall testing.

---

## DOMAIN 4 — COMMUNICATION AND NETWORK SECURITY (38 topics)

### 4.1.1 OSI Model
- 7 layers, PDU: 7 Application Data, 6 Presentation —, 5 Session —, 4 Transport Segments/Datagrams, 3 Network Packets, 2 Data Link Frames, 1 Physical Bits.
- Mnemonics: "All People Seem To Need Data Processing" and "Please Do Not Throw Sausage Pizza Away".
- OSI vs TCP/IP: 7 App / TCP/IP App; 6 Presentation formatting; 5 Session interhost; 4 Transport TCP/UDP / TCP/IP Transport; 3 Network routers, IP ICMP NAT / Internet; 2 Data Link switches, MAC / Link; 1 Physical hubs, NICs.

### 4.1.2 Layer 1 Physical
- Bits 0s/1s. Wired: Twisted Pair, Coaxial, Fiber Optic; Wireless: Radio Frequency, Infrared/Optical, Microwave. Fiber uses light, no cross talk.

### 4.1.3 Transport Architecture
- VIDEO ONLY.

### 4.1.4 Network Topologies
- Bus, Tree, Star, Mesh, Ring. Data plane (doer), control plane (intelligence), management plane (manages/monitors). Cut-through forwards as soon as reads destination; Store-and-forward waits entire packet.

### 4.1.5 Transmission Methods
- Unicast One-to-One, Multicast One-to-Many, Broadcast One-to-All, Anycast Nearest or best. Geocast = specific geographical region.

### 4.1.6 Traffic Flows
- No Core Concepts box. North-south (in/out of data center) vs East-west (between devices within data center).

### 4.1.7 Dealing with Collisions
- Token-based, Polling, CSMA. CSMA/CA avoids (wireless), CSMA/CD detects after (wired Ethernet, past).

### 4.1.8 Physical Segmentation
- No Core Concepts box. In-band (less secure), Out-of-band (separate network), Air-gapped (physically isolating). Logical: VLANs, VPNs, VRF, Virtual domains.

### 4.1.9 Performance Metrics
- Bandwidth — max; Throughput — actual; SNR — signal vs noise, higher allows higher rates; Latency — round-trip ms; Jitter — variation in delay, ideally low.

### 4.1.10 Layer 1 Devices
- Hubs (broadcast to all, same collision domain), repeaters, concentrators, NICs.

### 4.1.11 Layer 2 Data Link
- Frames, MAC, bridges/switches, L2TP/PPTP/ARP. ARP IP→MAC, RARP MAC→IP. PPTP auth PAP (least, plaintext), CHAP (encrypted), EAP (most robust).

### 4.1.12 Authentication Protocols
- EAP best, PEAP encapsulates EAP within encrypted/authenticated TLS tunnel. EAP-TLS Cert/Cert High/High; EAP-TTLS ID&Pwd/Cert Medium/Medium; EAP-PEAP ID&Pwd/Cert Medium/High; LEAP ID&Pwd/ID&Pwd Low/High; EAP-MD5 ID&Pwd/— Low/Low.

### 4.1.13 Layer 3 Network
- Packets, routers/L3 switches, ICMP, IGMP, IPsec, OSPF. Blue blurbs: "What protocol is often used to quickly determine if network communication problems exist?" (ICMP ping) and "Know what layer routers operate at" (L3).

### 4.1.14 Logical Addressing
- IPv4 = 32 bits, IPv6 = 128 bits; private not routable. Wired IEEE 802.3, Wireless IEEE 802.11, VLAN IEEE 802.1Q.
- Private RFC 1918: 10.0.0.0–10.255.255.255, 172.16.0.0–172.31.255.255, 192.168.0.0–192.168.255.255.
- Classes usable: A 16,777,214; B 65,534; C 254; D multicast; E reserved. Blue blurbs: "Be able to differentiate public vs private" and "Know max number of Class A, B, C IP addresses".

### 4.1.15 Layer 4 Transport
- TCP/UDP, 3-way handshake SYN, SYN-ACK, ACK, Ports. 20 FTP data, 21 FTP control, 22 SSH, 23 Telnet, 25 SMTP, 80 HTTP, 443 HTTPS. Port classes Well-known, Registered, Dynamic/Private/Ephemeral. Blue blurb: "Be familiar with port ranges and common ports…"

### 4.1.16 Layer 5 Session
- Session/dialog/control/management, PAP/CHAP/EAP/NetBIOS/RPC, circuit proxy firewall.

### 4.1.17 Layer 6 Presentation
- Formatting/encryption, translation/compression. Codec = coder/decoder.

### 4.1.18 Layer 7 Application
- Most breaches/attacks; protocols HTTP 80, HTTPS 443, FTP 20/21 vulnerable, SFTP 22, TFTP UDP 69 insecure, DNS TCP/UDP 53, Telnet 23, SSH 22, SMTP 25, SNMP UDP 161/162.

### 4.1.19 Convergence & VoIP
- Convergence = native IP carry non-IP via FCoE, iSCSI, VoIP; VoIP SRTP + SIP; Vishing = voice phishing.

### 4.1.20 Network Security Attacks
- Attack phases: recon, enumeration/scanning, vulnerability analysis, exploitation. SYN scan, SYN flood, DoS/DDoS, MITM, Spoofing, ARP poisoning (best prevented by monitoring network segments). Smurf (ICMP), Fraggle (UDP similar), Teardrop. Tools: Ping, Traceroute, Nmap, etc.

### 4.1.21 Wireless
- IEEE 802.11, TKIP replace WEP due to weak IV, protect wireless need 4: access control, authentication, integrity, encryption. WEP/WPA timeline 1997/2003/2004/2018, WEP/TKIP-RC4/CCMP-AES.

### 4.1.22 Common Network Tools
- VIDEO ONLY.

### 4.1.23 VLAN & SDN
- VLAN IEEE 802.1Q, SDN app/control/data planes, northbound app↔control, southbound data↔control. Blue blurb: "Understand the basic premise and use of VLANs".

### 4.1.24 Third-party Connectivity
- VIDEO ONLY.

### 4.1.25 Wide Area Networks
- WANs connect multiple LANs over large distances; dedicated leased lines, dial-up, satellite, wireless, packet carrier; protocols X.25, Frame Relay, ATM, MPLS. Blue blurb: "Know common WAN protocols and key features of each".

### 4.1.26 Monitoring and Management
- No Core Concepts box. Network observability, Traffic flow and shaping, Capacity management, Fault detection and handling.

### 4.2.1 Network Segmentation
- Defense in depth, Partitioning, Network Perimeter (choke point), Segmentation, Bastion Host / DMZ, Microsegmentation. Technologies: Network overlays, Distributed firewalls/routers, IDS/IPS, Zero trust.

### 4.2.2 Proxy, NAT & PAT
- Proxies act on behalf of someone else; NAT changes IP, PAT keeps track via unique port numbers. Blue blurb: "Understand NAT and PAT".

### 4.2.3 Firewall Technologies
- Simple packet, stateful packet (L3), circuit-level proxy (L5), application proxy (L7).

### 4.2.4 Firewall Architectures
- Packet filtering; Dual-homed host (two NICs, traffic never passes directly); Screened host (packet-filtering router in front of bastion host); Screened subnet (router at perimeter AND internal side of DMZ); Three-legged firewall (Internet, DMZ, trusted).

### 4.2.5 Intrusion Detection and Prevention
- Signature-based — known attacks, low false positives, cannot catch unknown; Anomaly — can catch unknown, can cause false positives; Host-based — only that host, can detect insider; Network — distributed, less effective with encrypted traffic; IDS is detective, IPS is preventative (inline).
- Blue blurbs: similarities/differences IDS/IPS, network vs host pros/cons, typical placement, mirror/span/promiscuous port (copies traffic to IDS, NIC receives all traffic), two analysis engines (signature/anomaly), allow list (only known good) vs deny list (block known bad).

### 4.2.6 Sandbox
- Sandbox = isolate/run untrusted code. True Positive — threat, correctly alerts; True Negative — no threat, correctly doesn't alert; False Positive — no threat, but alerts; False Negative — threat, fails to alert. Blue blurb: false negative is worst (silent miss).

### 4.2.7 Honeypots & Honeynets
- Honeypot = decoy to attract/study attackers; Honeynet = network of honeypots. Enticement — legally inviting; Entrapment — inducing (the 'no'). Blue blurb: "What type of control?" — technical detective.

### 4.2.8 Endpoint Security
- Best practices: Antivirus; Updates; Local firewall; DLP; VPN; NAC. Blue blurb: NAC — after health check, grants access or redirects to quarantine.

### 4.3.1 Tunneling & VPNs
- VPN protocols PPTP, L2F, L2TP, GRE, SOCKS, SSL, SSH, IPSec; GRE tunneling only; L2TP no encryption by default, uses IPsec; Auth PAP (least), CHAP, MS-CHAP, EAP (most secure).
- Blue blurbs: VPN types (remote access, site-to-site, Intranet trusted, Extranet outside trusted) and "Know common tunneling protocols".

### 4.3.2 IPSec
- AH authenticates only, protocol 51; ESP authentication + confidentiality, protocol 50; Transport Mode — encrypts only data, faster; Tunnel Mode — encrypts header and data, more secure, default in VPNs; IKE generates session key / key exchange. Blue blurb: "What protocol is used to exchange keys with an IPsec VPN?" — IKE. SA attributes: SPI, Protocol, Algorithms, Sequence number, Life cycle.

### 4.3.3 SSL / TLS
- Handshake: client hello, server hello, creation/sharing session key, establish. Asymmetric encrypts symmetric session key client created. DROWN major threat to SSLv2. TLS VPN — easy, browser, only particular connection; IPsec VPN — corporate, can protect entire network, harder to deploy.

### 4.3.4 Remote Authentication
- RADIUS (UDP 1812/1813, encrypts password only, multi-vendor); TACACS+ (TCP 49, encrypts entire packets, Cisco proprietary); Diameter (TCP 3868, successor of RADIUS, supports EAP, IPv4+IPv6, stateful failover, mobile/VoIP). Diameter = "twice the radius". Blue blurb: similarities/differences between remote authentication protocols.

---

## DOMAIN 5 — IDENTITY AND ACCESS MANAGEMENT (31 topics)

### 5.1.1 Access Control Principles
- Need to Know — only information they need; Least Privilege — only privileges they need; Separation of Duties — no one individual can carry out a critical function alone. Access modes: Create, Update, Read, Read-Write, Execute, Delete.
- Groups — static, created by IT; Roles — based on job function, created by business. Reference Monitor mediates all access. Blue blurb: "Understand the fundamental access control principles and how they might be applied".

### 5.1.2 Administration Approaches
- Centralized — all through one authority, strong control, easy, single point of failure; Decentralized — multiple authorities, less consistent, more adaptable. Blue blurb: "Know the difference between centralized and decentralized administration and pros/cons of each".

### 5.2.1 Access Control Services
- Four services: Identification (claims identity), Authentication (proves identity), Authorization (what access given), Accountability (account for actions, auditing/logging). Accountability also known as Principle of Access Control. Blue blurb: "Understand the four access control services".

### 5.2.2 Identification
- Guidelines: unique identifiers, nondescriptive of job/role, secure issuance. Factors: Knowledge = something you know; Ownership = something you have; Characteristic = something you are.

### 5.2.3 Authentication by Knowledge
- Passwords best practice 8–16 characters, upper/lower, numbers, symbols, do not reuse; static vs dynamic (one-time); Passphrase more secure because easier to remember longer.

### 5.2.4 Authentication by Ownership
- OTP generated using seed + time/counter; Soft tokens (phone app); Hard tokens (RSA SecureID); Smart cards — IC chip, certificates/keys, crypto processor; Memory cards — magnetic strip, static data.
- Synchronous OTP — time-based or event-based; Asynchronous — challenge/response with a nonce. Blue blurbs: async vs sync OTP, smart cards vs memory cards.

### 5.2.5 Authentication by Characteristics
- Physiological + behavioral. CER (crossover error rate) intersection of Type 1/Type 2 measures accuracy, lower = more accurate.
- Physical: fingerprints, hand geometry, facial, eyes retina/iris; Behavioral: writing, gait, voice, typing.
- Type 1 = False Rejection Rate (authorized incorrectly rejected — inconvenience); Type 2 = False Acceptance Rate (unauthorized incorrectly accepted — much more serious).
- Enrollment, verification 1:1, identification 1:N. Retina scan most accurate, also invasive.

### 5.2.6 Factors of Authentication
- 3 factors: know, have, are. SFA = 1 factor; MFA = 2+ DIFFERENT factors. Trap: RSA token + Microsoft token = both ownership = still single-factor; password + challenge question = both knowledge = still single-factor; password + RSA token = MFA.

### 5.2.7 Password-less Authentication
- Biometrics, hardware tokens (FIDO2), magic links, one-time codes. Reduces friction, weak passwords, phishing.

### 5.2.8 Single Sign-on (Kerberos)
- SSO authenticate once, access multiple; disadvantage single point of failure. Kerberos components: KDC (= AS + TGS), AS, TGS, TGT, Service Ticket.
- Steps: 1. User requests ticket from AS, 2. AS issues TGT encrypted with user's key, 3. User presents TGT to TGS, 4. TGS issues service ticket, 5. User presents service ticket to service. Kerberos disadvantages: only symmetric, TOCTOU vulnerable. SESAME improved, not widely adopted, supports symmetric+asymmetric.

### 5.2.9 Authenticator Assurance Levels (AAL)
- AAL1 — Some assurance, Single-factor, Secure protocol; AAL2 — High confidence, MFA, Secure protocol, Approved crypto; AAL3 — Very high confidence, MFA, Secure protocol, "Hard" crypto authenticator, proof of possession + impersonation resistance. Blue blurb: "Understand AAL ratings and elements of each".

### 5.2.10 Session Management
- Session hijacking: attacker steals session ID/cookie. Prevention: terminate after inactivity, re-authenticate, secure cookies, logout. Termination methods: Schedule Limitations, Login Limitation, Time-outs, Screensavers.

### 5.2.11 Registration and Proofing of Identity
- Identity proofing is confirming somebody is who they claim; RA proofs identity prior to issuance. Blue blurb: "What is identity proofing, and when does it take place?"

### 5.2.12 Federated Identity Management (FIM)
- SSO within one org, FIM across orgs; 3 components: principal/user, identity provider, relying party (service provider). Blue blurb: "Understand the basis of FIM and the three components".

### 5.2.13 Federated Access Standards
- SAML, WS-Federation, OpenID (authentication), OAuth (authorization); SAML assertions in XML. SAML components: Assertion, Protocol, Bindings, Profiles. Blue blurb: "Understand the importance of SAML and its relation to FIM".

### 5.2.14 Just-In-Time Access
- JIT = elevation for short period for infrequent tasks; minimizes long-term elevation risk.

### 5.2.15 Principle of Access Control
- Accountability = Principle of Access Control. Achieve via: 1. Users uniquely identified, 2. properly authenticated, 3. properly authorized, 4. all actions logged and monitored.

### 5.3.1 Identity as a Service (IDaaS)
- Services: Provisioning, Administration, SSO, MFA, Directory Services. Identities: Cloud, Synced, Linked, Federated. Risks: availability outage, protection of PII, entrusting third party.

### 5.4.1 Authorization Mechanisms
- DAC owner determines; Rule-based granular; RBAC roles; ABAC very granular attributes, XACML defines/enables; other context-based, risk-based. Categories Discretionary, Mandatory, Non-discretionary.

### 5.4.2 Discretionary Access Control (DAC)
- Owner determines who can access; 3 primary types rule-based, role-based, attribute-based. Blue blurbs: premise of DAC + 3 types, differences/why each used.

### 5.4.3 Groups, Roles and RBAC
- No Core Concepts box. RBAC users assigned one or more roles; roles mirror org chart, "best practice"; most orgs use Limited or Hybrid-RBAC.

### 5.4.4 Rule-based Access Control
- No Core Concepts box. Set of rules governs access; granular but much more administration.

### 5.4.5 Attribute Based Access Control (ABAC)
- No Core Concepts box. XACML defines/enables ABAC; blue blurb "Understand the purpose of XACML". Risk-based: IP, time, connection elements.

### 5.4.6 Mandatory Access Control (MAC)
- Rare, typically government, confidentiality primary; requires every asset classification + every user clearance; access based on clearance + classification. Blue blurb: defining characteristics and where/why typically used.

### 5.4.7 Non-Discretionary Access Control
- Somebody other than asset owner determines access; should be avoided if possible.

### 5.4.8 Access Control Summary
- VIDEO ONLY.

### 5.4.9 Access Policy Enforcement
- No Core Concepts box. PEP receives requests, gatekeeper, sends to PDP, enforces decision; PDP makes decisions based on rules, generally centralized.

### 5.5.1 Provisioning Lifecycle Importance
- Identity Life Cycle 3 parts: provisioning (hire + role change), review (as often as necessary, more for privileged), revocation (termination). Blue blurb: "Understand the Identity Life Cycle and what happens at each stage".

### 5.5.2 User Access Review
- At least annually, role change = review at time of change, privileged more frequently (admin perhaps weekly). Termination = remove all access.

### 5.5.3 Service Accounts
- Limit to single purposes, reduce privileges; risks privilege escalation and spoofing; human oversight required.

### 5.6.1 Implement Authentication Systems
- Popular: OIDC, OAuth, SAML, Kerberos, RADIUS, TACACS+. OIDC = identity layer on OAuth 2.0; OAuth = access delegation standard.

---

## DOMAIN 6 — SECURITY ASSESSMENT AND TESTING (19 topics)

### 6.1.1 Intro to Testing
- No Core Concepts box, no blue blurb visible. Ensure security requirements/controls are defined, tested, operating effectively; assurance pillar (functional + assurance).

### 6.1.2 Validation & Verification
- Validation — Are we building the right product? Verification — Are we building the product right? 3 Cs: Completeness, Correctness, Consistency. Blue blurbs: difference between validation/verification; verification stopping point — GAP: stopping-point answer was not in the visible extract.

### 6.1.3 Effort to Invest in Testing
- Effort proportionate to value. Blue blurb: "How much testing is enough?" — proportionate to value. Strategies internal/external/third party; locations on-premise/cloud/hybrid.

### 6.1.4 Location of Assessment
- No Core Concepts box. Blue blurb: "Understand the role of a security professional" — Identify risk, Advise testing, Provide advice/support; security team should not perform testing alone.

### 6.2.1 Testing Overview
- Testing stages: Unit (component in isolation), Interface, Integration (combined units), System (whole incl. hardware/software). Static: source-code, inspections, code review. Dynamic: input/output. White-box: access to source/internals. Black-box: no access to internals.
- Manual — exploratory/UI, flexible, time consuming; Automated — upfront investment, predictable, necessary for large/complex + regression.
- SAST = static, tests source code, does NOT execute, fast, many false positives; DAST = dynamic, executes code, real-time, slow, requires running server; Mutation fuzzer modifies known good input; Generation fuzzer creates input from scratch.
- Positive = expected results; Negative = errors/unexpected; Misuse = tries to exploit.
- Equivalence Partitioning — inputs into groups (password 0–7 reject, 8–16 accept, 17+ reject); Boundary Value Analysis — values at boundaries (7, 8, 16, 17); Decision Table; State-based; Coverage = covered/total, e.g. 50/100 = 50%.
- Blue blurbs: SAST vs DAST vs fuzz, black box vs white box, positive/negative/misuse, equivalence partitioning vs boundary value analysis.

### 6.2.2 Testing Techniques
- VIDEO ONLY.

### 6.2.3 Vulnerability Assessment & Penetration Testing
- VA automated minutes/hours/days, pen test manual several days. Phases: 1. Reconnaissance (passive), 2. Enumeration (active), 3. Vulnerability analysis, 4. Execution/Exploitation (pen test only — differentiates them), 5. Document/Reporting. Blue blurbs: purpose of VA, VA vs pen test differences, process and key differentiating step.

### 6.2.4 Red, Blue and Purple Teams
- Red = attackers, simulate threats; Blue = defenders, evaluate/monitor/respond; Purple = collaboration between red+blue, not distinct teams.

### 6.2.5 Vulnerability & Pen Testing Techniques
- No Core Concepts box; Blue blurb "Understand testing technique perspectives, approaches, and knowledge types" — internal vs external, blind vs double-blind, zero/partial/full knowledge.

### 6.2.6 SCAP & Breach Attack Simulation
- VIDEO ONLY.

### 6.2.7 Log Review & Analysis
- Log what is relevant, review, identify errors/anomalies; synchronized log times critical, NTP used. Log lifecycle: Generation, Transmission, Collection, Normalization, Analysis, Retention, Disposal. Blue blurb: "Understand importance of timely log review and analysis".

### 6.2.8 Limiting Log Sizes
- Circular overwrite limits max size by overwriting earliest; Clipping levels log based on threshold settings (more valuable information). Blue blurb: difference between circular overwrite and clipping levels.

### 6.2.9 Operational testing — Synthetic transactions & RUM
- Synthetic transactions = scripted activities to validate system performing as expected, used after changes; RUM (Real User Monitoring) = actual users, real data, production, can't cover all scenarios.

### 6.2.10 Regression Testing
- Verifies previously functional software still works after updates/patches. Blue blurb: "What is regression testing, and why is it important?" Report: objective pass/fail, right detail for right audience, metrics that matter.

### 6.3.1 Key Risk & Performance Indicators
- KRI forward-looking aid risk decisions; KPI backward-looking historical performance; SMART = Specific, Measurable, Achievable, Relevant, Timely.

### 6.4.1 Test Output Importance
- Remediation, Exception handling, Ethical disclosure (to vendor first, if not patched publish to public/CVE with PoC).

### 6.5.1 Audit Approaches
- Internal = employees, organizational processes; External = employees, vendor processes; Third-party = independent auditors, vendor processes.
- Audit plan: define objective, define scope, conduct audit, refine process. Typical process: goals, involve business leaders, scope, choose team, planning, conducting, documenting, communicating. Blue blurbs: components of audit plan, different audit approaches.

### 6.5.2 SOC Reports
- SAS70 → SSAE16 → SSAE18; SOC 1 basic financial reporting risks; SOC 2 five trust principles (security, availability, confidentiality, processing integrity, privacy); SOC 3 stripped-down SOC 2 for marketing; Type 1 point in time design; Type 2 period of time design + operating effectiveness (typically a year); SOC 2 Type 2 most desirable. Blue blurbs: SOC 1/2/3 difference, Type 1 vs Type 2.

### 6.5.3 Audit Roles & Responsibilities
- Executive (senior) management, audit committee, security officer, compliance manager, internal auditors, external auditors; tone from top.

---

## DOMAIN 7 — SECURITY OPERATIONS (36 topics)

### 7.1.1 Securing the Scene
- Sealing off access, photographing, documenting location of evidence, avoiding touching anything; contaminated evidence can't be decontaminated.

### 7.1.2 Evidence Collection and Handling
- Forensic process: identification/securing scene, collection preserving integrity + chain of custody, examination, analysis of most compelling, final reporting.
- Chain of custody = who handled what, when, where. MOM = Motive, Opportunity, Means.
- Evidence types: Real (tangible physical), Direct (speaks for itself — eyewitness, confessions), Circumstantial/indirect (implication/inference), Corroborative (supports other facts), Hearsay (not present, no firsthand proof), Best evidence rule (original rather than copy), Secondary (reproduction e.g. printout of logs).
- Blue blurb: "Understand the steps of the forensic investigation process" — identify/secure → collect → examine/analyze → report.

### 7.1.3 Locard's Exchange Principle
- With every crime, something is taken and left behind; every interaction, some transfer occurs. Blue blurb: "Understand what is meant by Locard's exchange principle".

### 7.1.4 Digital Forensics
- Live evidence = data in running system (RAM, cache, buffers), volatile, system must remain on; Forensic copies = identical bit-for-bit, prove with hash values; Mobile forensics very hard, evolving, lack of standards; Artifacts = remnants/breadcrumbs of breach.

### 7.1.5 Chain of Custody
- Control of evidence to maintain integrity for court; established immediately and maintained; who collected/handled what, when, where; tag, bag, carry evidence.

### 7.1.6 Five Rules of Evidence
- Five rules: Authentic, Accurate, Complete, Convincing/Reliable, Admissible. Blue blurb: "Understand the five rules of evidence and their meaning".

### 7.1.7 Types of Investigations
- No Core Concepts box. Criminal (legal punishment, law enforcement), Civil (disputes, fine/monetary), Regulatory (violations of regulated activities, regulatory body), Administrative (internal policy violations, the organization). This is the Domain 7 content cross-referenced from Domain 1, 1.5.1.

### 7.2.1 SIEM Importance
- SIEM ingests logs, capabilities: aggregation, normalization, correlation, secure storage, analysis/reporting. Sources: appliances, network devices, DLP, applications, OS, servers, IPS/IDS. Threat Intelligence, UEBA.

### 7.2.2 Continuous Monitoring
- Technology, processes, people; routinely updated. Blue blurbs: concept/value of continuous monitoring, what it encompasses.

### 7.3.1 Asset Inventory Importance
- Secure provisioning (never deploy with default settings — harden); update inventory when asset added/removed; without current inventory low chance of patching/configuring/scanning.

### 7.3.2 Configuration Management Importance
- Steps: Identify assets → Configure → Document → Verify. Changes planned, approved, documented, evaluated, implemented, verified. Blue blurb: "Understand the value and key benefits of configuration management".

### 7.4.1 Foundational Security Operations Concepts
- Need to Know (restricting KNOWLEDGE/access) vs Least Privilege (restricting ACTIONS/PRIVILEGES); PAM — separate regular + privileged accounts, MFA required, increased logging; Job rotation fraud detection/deterrent + cross-training; SLA legal contract. Blue blurb: "Understand foundational security operations concepts".

### 7.5.1 Protecting Media Importance
- MTBF important criterion; media types paper, microforms, magnetic, flash, optical; no media lasts forever.

### 7.6.1 Incident Response Process Importance
- Event = observable occurrence; Incident = adverse event; Not all events are incidents. Blue blurbs: event vs incident, IR process and each step.
- IR steps: Preparation, Detection, Response (impact assessment), Mitigation (containment), Reporting, Recovery (return to normal), Remediation (prevention), Lessons Learned (improve process).

### 7.7.1 Malware Importance
- Virus (triggered by user), Worm (self-propagate), Logic bomb (logic trigger), Trojan horse (looks harmless), Polymorphic (changes to evade), Ransomware (encrypts + ransom), Rootkit (masks presence), Zero-day (never seen, no detection), plus Companion, Macro, Multipartite (Stuxnet), Botnet, Boot sector, Hoaxes, Stealth, Data diddler (salami attack). Blue blurb: "Understand different types of malware and characteristics of each".

### 7.7.2 Anti-malware
- VIDEO ONLY.

### 7.7.3 Machine Learning and AI-based tools
- Guidebook exists (button looked greyed but loads). ML subset of AI, learns from data without explicit programming; applications threat detection/classification, network risk scoring, automation, response to cybercrime.

### 7.8.1 Patch Management
- Guidebook exists (button looked greyed but loads). Fixes known vulns only; Agent = update software on devices; Agentless = remotely connect; Passive = monitor traffic to infer patch levels. Blue blurb: "Understand why timely and consistent application of patches is beneficial and important".

### 7.9.1 Change Management Importance
- Guidebook exists (button looked greyed but loads). Process: Change request → Assess impact → Approval (CAB) → Build and test → Notification → Implement → Validation → Version and baseline. Blue blurb: "Understand the change management process and what happens at each step".

### 7.10.1 Failure Modes
- Fail-soft (fail-open): less security, e.g. firewall allowing all traffic if it fails; Fail-secure (fail-closed): same/greater security, e.g. firewall blocking all; Fail-safe: prioritize safety of people, e.g. doors unlock in fire alarm. Blue blurb: "Understand the three types of failure modes and what each one prioritizes".

### 7.10.2 Backup Storage Strategies
- Archive bit 0=no backup, 1=modified/backup required; Mirror exact copy, fastest backup+restore, high storage; Full ALL data, slowest backup, fast restore, high storage; Differential changes since last full, moderate; Incremental changes since last backup, fast backup, slow restore, lowest storage. Rotations FIFO, grandfather-father-son, Tower of Hanoi.

### 7.10.3 Spare parts
- Cold — parts on shelf, offline, downtime, least expensive; Warm — installed not powered, back online quickly, costs a bit more; Hot — installed, powered, instantly takes over, expensive.

### 7.10.4 RAID
- RAID 0 striping speed, min 2, no resiliency, highest read/write; RAID 1 mirroring redundancy, min 2, moderate, great resiliency; RAID 10 (1+0) min 4, striping+mirroring, most expensive, highest; RAID 5 parity, min 3, balance, parity from XOR. Blue blurb: "Understand the primary types of RAID and pros and cons of each".

### 7.10.5 Clustering & Redundancy
- Clustering = group working together to handle load; Redundancy = primary + secondary standby; Availability = fault tolerance; Resilience = quickly return after failure. Blue blurb: "Understand differences between clustering and redundancy".

### 7.10.6 Recovery Site Strategies
- Cold site $ Weeks (shell, no equipment); Warm $$ Days (hardware installed, data not current); Hot $$$ Hours (hardware + data current); Mobile $$$ Days/Hours; Redundant $$$$ Instant/Seconds. Reciprocal agreement (two companies support each other); Resource capacity agreements; Multiple processing sites.

### 7.11.1 Disaster Recovery
- Disaster declared when MTD going to be exceeded. Personnel: Exec/senior mgmt, Legal, HR, IT, PR. Blue blurb: "Understand role MTD plays in declaration of a disaster". Note: 7.11.1 and 7.11.6 present the same material.

### 7.11.2 BCM, BCP & DRP
- BCP = survival of business processes, strategic, processes; DRP = recovery of technology/systems, tactical, systems. BCM creates/maintains/tests both.
- BCP/DRP 7 steps: 1. Develop Contingency Planning Policy, 2. Conduct BIA, 3. Identify controls, 4. Create contingency strategies, 5. Develop contingency plan, 6. Ensure testing, training, and exercises, 7. Maintenance. Blue blurbs: "BCP versus DRP" and "Understanding MTD, RTO, RPO, WRT".

### 7.11.3 Business Impact Assessment (BIA)
- Most important step in BCP. BIA steps: 1. Determine mission/business processes and recovery criticality, 2. Identify resource requirements, 3. Identify recovery priorities. Blue blurbs: Purpose of BIA; Steps in BIA.

### 7.11.4 RPO, RTO, WRT & MTD
- RPO = max tolerable data loss measured in time; RTO = max tolerable time to recover systems to defined service level; WRT = max tolerable time to verify system/data integrity; MTD/MAD = max time disrupted before unacceptable consequences, also called AIW; Golden rule RTO should never exceed MTD; MTD = RTO + WRT; lower RPO/RTO = more expensive.

### 7.11.5 External Dependencies
- VIDEO ONLY.

### 7.11.6 Declaring and Disaster
- No Core Concepts box. Declaration + activation by CEO or Business Continuity Board/Committee; follow IR first, if MTD will be exceeded declare disaster. Same material as 7.11.1. Blue blurb: "Understand the what constitutes a disaster" [sic].

### 7.11.7 Restoration Order
- BIA determines order — most critical recovered first at recovery site; when restoring to primary site, least critical restored first to make sure site works. Blue blurb: "Understand how a dependency chart informs restoration order".

### 7.12.1 BCP & DRP testing
- DRP tests IN ORDER: read-through/checklist (least impact), walkthrough, simulation, parallel, full-interruption/full-scale (most impactful/riskiest). Full-interruption only after mgmt approval + other tests successful. Blue blurbs: "Know the order of DRP testing and which test is least/most impactful", "When should a full-scale, full-interruption test be conducted?"

### 7.13.1 Goals of Business Continuity Management
- BCM three primary goals: 1. Safety of people, 2. Minimization of damage, 3. Survival of business; #1 goal safety of people. Blue blurbs: "Understand the three goals of BCM" and "Understand the number one goal of BCM".

### 7.14.1 Implement and manage physical security
- Cross-reference to Domain 3 physical security (3.8, 3.9). No Core Concepts box.

### 7.15.1 Address personnel safety and security concerns
- No Core Concepts box; safety of humans paramount; Travel and Duress; duress = threats/violence/constraints to do something against will; travel — org still responsible, may include medical/travel insurance, action plan, companies like International SOS.

---

## DOMAIN 8 — SOFTWARE DEVELOPMENT SECURITY (18 topics)

### 8.1.1 Security's Involvement in Development
- Security involved at every phase, from beginning through deployment/use to retirement; end-of-life → archival/disposal. Blue blurb: "Understand when security should be considered as part of the SDLC" — from the beginning, through deployment/use, to retirement.

### 8.1.2 SDLC & SLC
- SLC phases: Initiation, Development/Acquisition, Implementation (Certification & Accreditation), Operation/Maintenance, Disposal.
- SDLC phases: Initiation (Plan + Mgmt Approval) → Requirements (Risk Analysis, threat modeling) → Architecture & Design (Define security requirements) → Development (Build security functionality) → Testing (Test security functionality) → Release/Deployment (Secure deployment & baselines) → Operation (Ongoing maintenance & vulnerability assessment) → Disposal (Secure disposal of data).
- Waterfall: phased step-by-step, can't go backward, design frozen, changes via change management. Blue blurbs: flow of SDLC/SLC, phase threat modeling takes place (Requirements).

### 8.1.3 Development Methodologies
- Waterfall (complete each phase before next, no revisiting), Structured Programming Development, Agile (rapid iterations), Scaled Agile framework, Spiral (risk-driven iterative + waterfall), Cleanroom (certifiable reliability).
- Scrum master: shields team from external interference, enforces scrum principles, facilitator/removes barriers, enables cooperation, improves productivity. Blue blurbs: development methodologies characteristics, waterfall vs agile priorities, role of scrum master.

### 8.1.4 DevOps
- IPT = integrated product team = DevOps (development, operations, QA); with security = DevSecOps. Incorporating security: Plan for security; Strong engagement dev/ops/security; Engage developers; Secure techniques/frameworks; Automate security testing (CI/CD); Use traditional techniques sparingly. Blue blurb: "Know when security should be involved with DevOps".

### 8.1.5 Canary Testing & Deployments
- Canary = pushing changes to small subset of users before full release, early warning like canary in a coal mine. Smoke testing = quick preliminary testing after a change for simple failures of most important functionality. Blue blurb: "Understand what is meant by canary testing and deployment".

### 8.1.6 Maturity Models
- CMMI 6 levels: 0 Incomplete (unknown/ad hoc), 1 Initial (reactive/unpredictable, over budget/late), 2 Managed (projects managed/planned, metrics taken), 3 Defined (proactive, standards across org), 4 Quantitatively Managed (controlled/measured, data-driven), 5 Optimizing (flexible/stable, continually improving, able to pivot).
- SAMM 3 levels: 1 Initial Implementation, 2 Structured Realization, 3 Optimized Operation; 5 business functions: Governance, Design, Implementation, Verification, Operations. Blue blurb: "Know the name and characteristics of each level of CMMI".

### 8.1.7 Operation and Maintenance & Change Management
- No Core Concepts box; O&M = monitoring, periodic evaluation, patching; change mgmt review (7.9.1); RFC process.

### 8.2.1 Software Development
- VIDEO ONLY.

### 8.2.2 Code Obfuscation
- Hiding/obscuring code; 3 types: Lexical (modifies look — comments, debugging info, format; easiest but weakest), Data (modifies data structure), Control Flow (modifies flow — reordering, loops, irrelevant conditionals).
- Blue blurbs: term + three types; significant disadvantage — disaster: little to no recourse to bring application back online quickly; software vault should store unaltered source code. Separate dev/test/prod is best practice.

### 8.2.3 DBMS, Concurrency & Locks
- Columns/fields=attributes, records/rows=tuples; primary key uniquely identifies tuple, foreign key refers to primary key in another table; ACID = Atomicity (all or none), Consistency (consistent with rules), Isolation (invisible until complete), Durability (completed changes will not be lost). Blue blurbs: primary/foreign keys + referential integrity, ACID, concurrency/locks.

### 8.2.4 Metadata
- "Metadata is data about other data" — creation date, last modified, owner, file size, etc.

### 8.3.1 Software Security Assessment Methods
- Risk analysis and mitigation, Auditing and logging of changes, Logging and monitoring, Internal and external audit, Procurement process, Certification and accreditation, Testing and verification, Code signing. Certification = technical analysis; Accreditation = management's formal authorization.

### 8.4.1 Acquiring Software Importance
- Software assurance phases: planning/requirements, contracting, acceptance, monitoring and follow-on. Ways: COTS, open source, third party, managed services.
- COTS pros: functionality verified, comparisons, third-party evaluation, existing customers, updates readily available; cons: no white-box testing, vendor going out of business, support issues, missing features, vulns widely exploited.
- Open source: control, training, security (vulns identified sooner), stability. MSPs assess via SOC reports, site visits, existing customers. Blue blurb: "understand what steps should be included first when considering any acquisition of software".

### 8.5.1 Secure Coding Guidelines
- No Core Concepts box. Weaknesses: Covert Channels (timing and storage), Buffer Overflows, Memory/Object Reuse, Executable Mobile Code, TOCTOU (race condition), Backdoors/Trapdoors, Malformed Input, Citizen Developers. Frameworks: OWASP Top 10, NIST, CIS.

### 8.5.2 Buffer Overflow
- Input exceeds buffer capacity; exploitable to elevate privileges / launch malicious code; ASLR randomizes memory location; other mitigations: parameter/bounds checking, thorough code review / improved development process, runtime checking, safe programming languages and library functions. Blue blurbs: what buffer overflow is / how it works, mitigation through ASLR, other protections.

### 8.5.3 Application Programming Interfaces (APIs)
- REST newer, flexible/lighter-weight, HTTP-based, fast, output CSV/JSON/RSS/XML; SOAP older, rigid/standardized, XML-based, strong error handling.
- API security: authentication/authorization (tokens/OAuth), Encryption (TLS), Data validation, API gateways, Quotas and throttling, Testing and validation. Blue blurbs: what an API is, two most common formats, techniques to secure APIs.

### 8.5.4 Secure Coding Practices
- Practices include: input validation, authentication and password management, session management, cryptographic practices, error handling and logging, system configuration, file/database security, memory management.
- Low coupling + high cohesion optimal. Polyinstantiation = instantiated into multiple separate instances, prevents unauthorized inference, allows same data at different classification levels. Blue blurbs: cohesion and coupling ideal combination, polyinstantiation and what it prevents.

### 8.5.5 Software Development Vulnerabilities
- Arise from: insecure coding practices; citizen developers; Between-the-lines attack (= man-in-the-middle, intercepts/modifies communication); Memory reuse (object reuse).

---

## NOTES, GAPS AND CAUTIONS

- Video-only topics (no Guidebook, so no Core Concepts / blue blurbs exist to extract — video content was not transcribed): D1: 1.5.1, 1.9.6, 1.9.8, 1.9.10; D2: 2.4.1, 2.6.4; D3: 3.6.14; D4: 4.1.3, 4.1.22, 4.1.24; D5: 5.4.8; D6: 6.2.2, 6.2.6; D7: 7.7.2, 7.11.5; D8: 8.2.1. (1.7.1 and 1.5.1 are cross-references to Domain 7, not missing content.)
- Several Guidebook buttons look greyed/disabled in the portal (e.g. 7.7.3, 7.8.1, 7.9.1, 7.10.1, 6.1.1) but DO load full Guidebook content when clicked. Those were all re-checked and included above.
- Full detail not captured in a few items, flagged in place: 3.4.6 ring assignments beyond Ring 0; 3.5.5 DFS risk wording; 3.6.2 IV/nonce weaknesses; 3.6.4 RC2-128 block size shown as "8?"; 6.1.2 verification stopping point; table checkmarks that render as "?" in text extraction. Nothing was invented to fill those gaps.
- Guide numbering mismatches exist in the source; the guide's own numbering was preserved, not corrected.
- 7.11.1 and 7.11.6 present the same declaring-a-disaster material; 7.14.1 is only a cross-reference to Domain 3 physical security.
- No domain guide was inaccessible. All 8 domains were accessed and scanned topic by topic in the new portal at new.my.destcert.com; app.destcert.com loaded only a spinner, so work continued in the new portal.
