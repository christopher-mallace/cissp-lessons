# Missed Questions Appendix — the source questions behind the profile

Companion to `CISSP_Master_Learning_Profile.md`. Added 2026-11-09 at Christopher's direction, because the profile alone only named topic clusters — Rain could not identify the actual questions Christopher got wrong that spurred each review/lesson.

Every question Christopher missed on Quantum Exams "CISSP: 10 Question Quiz" (15 attempts, Oct 3 – Nov 5, 2026; 72 missed of 150) is listed here with a stable ID (MQ-01 … MQ-72, in attempt order), the attempt and question number, a short summary of what was asked (in Darla's words, not a verbatim copy), what Christopher picked, the correct answer, and the site feedback's key point. Domains are Darla's mapping to the DestCert Review Guide domains, as in the profile. Per-domain totals reconcile with the profile: D1 = 26, D3 = 14, D8 = 9, D6 = 6, D7 = 5, D2 = 4, D5 = 4, D4 = 4.

**Rule for Rain:** at the top of every lesson, cite the MQ IDs that spurred it. When Christopher asks which question(s) he got wrong behind a lesson or priority, answer from this appendix.

## Lesson 1 source questions (Domain 1 — BCP/BIA/DR decision order)
MQ-12 (HA guarantee — UPS not connected), MQ-27 (BCP reliability — regular testing/updates), MQ-34 (alternative site — calculated risk + scope of threat), MQ-35 (BIA definition), MQ-39 (power fault = short-term loss), MQ-41 (data quality/availability in a disaster), MQ-45 (HA/SLA — review the SLA first), MQ-46 (BCP vs DRP), MQ-51 (BIA review — engage business process owners), MQ-59 (UPS vs warm site), MQ-63 (MTD)

## By priority — source question IDs
1. Domain 1 BCP/BIA/DR cluster: MQ-12, MQ-27, MQ-34, MQ-35, MQ-39, MQ-41, MQ-45, MQ-46, MQ-51, MQ-59, MQ-63
2. Domain 1 due care vs due diligence: MQ-11, MQ-24, MQ-36 (risk order: MQ-19, MQ-49)
3. Domain 3 side-channel + crypto distinctions: MQ-04, MQ-18 (side-channel); MQ-07, MQ-20, MQ-37, MQ-50, MQ-72 (crypto)

## All 72 missed questions, by attempt

### Attempt 1 — Oct 3, 2026 — 3/10 — 7 missed
- **MQ-01** [D7] Q1 — After a 3rd ransomware attack in 6 months, reviewing prior incidents: which incident-response part was most likely not done correctly? You picked: Lessons Learned. Correct: Remediation. Why: root-cause analysis sits in remediation; a repeat attack means it was not done correctly.
- **MQ-02** [D6] Q3 — CISO worried about an internal attack wants to audit "trusted actors" / insider misuse: which audit type fits best? You picked: Third-party audit. Correct: Internal audit. Why: internal audits concentrate on authorized/trusted actors.
- **MQ-03** [D8] Q6 — Webpage flaw where JavaScript lets an attacker inject malicious code into a user's browser: which vulnerability? You picked: CSRF. Correct: DOM-based XSS. Why: DOM XSS is common in JS frameworks/single-page apps that dynamically include attacker-controlled content.
- **MQ-04** [D3] Q7 — Flaw letting an attacker infer sensitive information by observing system behaviour: what is it? You picked: Covert channel. Correct: Side-channel attack. Why: a side channel infers sensitive information just by observing how a system works.
- **MQ-05** [D4] Q8 — Small, limited-budget organisation wants services accessible from the internet while protecting its internal network: which device is best? You picked: Firewall. Correct: Bastion host. Why: a bastion host is deliberately exposed on a public network.
- **MQ-06** [D7] Q9 — Which e-discovery phase ensures information is well-organised? You picked: Discovery. Correct: Information governance. Why: information governance is the phase ensuring information is well-organised.
- **MQ-07** [D3] Q10 — Top-secret information needing unbreakable encryption: which method is best? You picked: ECDH. Correct: Vernam cipher (one-time pad). Why: the one-time pad is the only theoretically unbreakable encryption.

### Attempt 2 — Oct 25, 2026 — 5/10 — 5 missed
- **MQ-08** [D8] Q2 — Best example of a functional requirement? You picked: Capacity. Correct: Authentication. Why: authentication is functional; scalability, capacity and availability are non-functional.
- **MQ-09** [D3] Q3 — Greatest security risk of deploying IoT devices across manufacturing plants? You picked: Limited device processing power. Correct: Lack of network segmentation. Why: without segmentation a compromised IoT device is an entry point to critical systems.
- **MQ-10** [D7] Q4 — Cost-conscious CISO wants a cost-efficient, quick backup solution: what should be used? You picked: RAID 1. Correct: Full backups. Why: RAID is redundancy, not a backup.
- **MQ-11** [D1] Q6 — Practitioner assessing security finds a potential vulnerability from inadequate data-lifecycle policies: what is he most likely doing? You picked: Due care. Correct: Due diligence. Why: assessing/verifying effectiveness of policies is due diligence; due care is the actions taken to resolve.
- **MQ-12** [D1] Q10 — Cloud provider guaranteeing 100% high availability; with a power disruption, greatest risk to that guarantee? You picked: Lack of a generator. Correct: UPS not connected to vital equipment. Why: a UPS gives continuous power; a generator is for long-term outages and starts after one begins.

### Attempt 3 — Oct 25, 2026 — 8/10 — 2 missed
- **MQ-13** [D1] Q5 — Solution so assets are only updated by appropriate Data Processors: which CIA aspect is most addressed? You picked: Confidentiality. Correct: Integrity. Why: the goal is that only authorised individuals can modify the data.
- **MQ-14** [D8] Q6 — In which SDLC phase are customer-specific requirements most likely addressed? You picked: System requirements. Correct: Functional architecture. Why: functional requirements describe the particular operation of a system.

### Attempt 4 — Oct 27, 2026 — 6/10 — 4 missed
- **MQ-15** [D3] Q1 — Vendor disposing of outdated hardware; worried about data remanence/disclosure: what best prevents disclosure? You picked: Crypto-shredding. Correct: Encryption. Why: encrypting data means the vendor cannot view it; an NDA deters but does not prevent.
- **MQ-16** [D8] Q2 — Project broken into sections, each released to customers when complete: which SDLC model? You picked: Agile. Correct: Incremental. Why: the incremental model designs, implements and tests a system a little at a time.
- **MQ-17** [D2] Q3 — Upgrading/reselling old storage devices, balancing effective data removal with cost efficiency: what is best? You picked: Overwrite + degaussing. Correct: Cryptographic erase before reselling. Why: overwrite + degaussing is overkill/not cost-efficient for usable resale devices.
- **MQ-18** [D3] Q9 — Practitioner notices specific sounds generated by a system/device: which attack type? You picked: Inference. Correct: Side-channel. Why: a side-channel attack is a passive, non-invasive way of observing a device's operation.

### Attempt 5 — Oct 28, 2026 — 8/10 — 2 missed
- **MQ-19** [D1] Q1 — Using a risk matrix; senior management has already approved the assessment: what is the next step? You picked: Analyze data. Correct: Create risk assessment taskforce. Why: order is request approval, form a team, analyse data, calculate risk, then countermeasures.
- **MQ-20** [D3] Q2 — Best technology for managing encryption keys and digital certificates in a cloud environment? You picked: ACLs. Correct: PKI. Why: PKI manages encryption keys and digital certificates.

### Attempt 6 — Oct 28, 2026 — 6/10 — 4 missed
- **MQ-21** [D6] Q5 — Legacy applications allow unauthenticated database queries: best immediate response? You picked: Perform risk analysis and compensating controls. Correct: Immediately restrict access and require proper authentication. Why: risk analysis does not address the immediate vulnerability.
- **MQ-22** [D8] Q6 — How best to ensure a secure product, security not as an afterthought? You picked: Conduct continuous process improvements. Correct: Perform perpetual analysis throughout the project. Why: security should be built in and analysed throughout, not bolted on.
- **MQ-23** [D8] Q7 — Financial institution adopting AI for fraud detection: highest-priority security consideration? You picked: Ensuring user data privacy. Correct: Protecting training data. Why: protecting training data ensures the AI's integrity and reliability.
- **MQ-24** [D1] Q9 — CEO mandated an unapproved vaccination after an outbreak; employees reacted severely and sued: what could best have prevented the lawsuit? You picked: More adequate due diligence re safety protocols. Correct: Proper due care to protect employees. Why: due diligence is informed decision-making; due care is implementing decisions with proper care.

### Attempt 7 — Oct 29, 2026 — 3/10 — 7 missed
- **MQ-25** [D2] Q1 — Third-party data stored on a central server; classification levels must be determined: at which data-lifecycle step is classification done? You picked: Usage. Correct: Storage. Why: data is classified during the storage stage.
- **MQ-26** [D6] Q3 — Financial-services company uses real-time monitoring and regular penetration tests: what practice is it demonstrating? You picked: Incident Response. Correct: Continuous Monitoring. Why: continuous monitoring is the ongoing observation of systems/networks to identify and respond to threats.
- **MQ-27** [D1] Q4 — A BCP is being developed to keep operations running: what is most important to ensure the plan is reliable? You picked: Identification of critical business functions. Correct: Regular testing and updates of the BCP. Why: a BCP must be tested to ensure it works when needed.
- **MQ-28** [D1] Q6 — Manager determining controls for high-value assets; categorisation is already done: what next? You picked: Categorise assets based on classification. Correct: Select controls that best meet the needs. Why: do due diligence on suitable controls and select them before implementing; categorisation has already passed.
- **MQ-29** [D3] Q7 — Researching fire detection for a network closet: which type is best for early-stage fire detection? You picked: Ionization monitoring. Correct: Aspirating sensors. Why: aspirating sensors provide incipient smoke detection of an early-stage fire.
- **MQ-30** [D4] Q8 — VPN that must work through NAT: which option is least likely to work? You picked: PPTP to work through NAT. Correct: Utilize IPsec AH. Why: IPsec AH is least likely to work with NAT because AH includes the original IP address in its header.
- **MQ-31** [D6] Q9 — Applications deployed in a virtualised environment, concerned about vulnerabilities in the images: best way to address? You picked: Monitoring runtime behaviour. Correct: Implementing a security scanning tool for image vulnerabilities. Why: scanning tools detect vulnerabilities in images before deployment.

### Attempt 8 — Oct 30, 2026 — 5/10 — 5 missed
- **MQ-32** [D5] Q1 — Biometrics easily replicated and generated PINs easily guessed, while assessing access controls/identity management: what are these threats targeting? You picked: MFA. Correct: Confidentiality of substantiation devices. Why: the threats exploit the confidentiality of authentication devices to enable disclosure.
- **MQ-33** [D1] Q2 — After a risk assessment, defining controls to remediate risk: what must the control set be based on? You picked: Countermeasures should be evaluated for effectiveness. Correct: Control set must be based upon risk capacity. Why: risk capacity is the risk you can afford to take, and surrounds risk appetite.
- **MQ-34** [D1] Q3 — Selecting an alternative site for contingency planning: on what should the choice be based? You picked: Calculated risk + likelihood. Correct: Calculated risk + specific scope of threat. Why: an alternative site is not one-size-fits-all; likelihood is hard to determine accurately.
- **MQ-35** [D1] Q4 — Which process best describes determining methods to reduce the impact of a disruption (determining critical assets and risks)? You picked: Risk Assessment. Correct: Business Impact Assessment. Why: a BIA determines critical assets, their risks and the impact of losing them.
- **MQ-36** [D1] Q7 — Firewall admin gets an email, apparently from the CIO, to open port 21 for foreign ingress; he checks with the CIO first: what best justifies this? You picked: FTP insecure passwords in clear text. Correct: Execution of prudency based on awareness. Why: being prudent — verifying before acting — protects against gross negligence.

### Attempt 9 — Nov 2, 2026 — 7/10 — 3 missed
- **MQ-37** [D3] Q1 — Implementing authentication algorithms for use with IPsec: which best suits? You picked: Diffie-Hellman. Correct: ECDSA. Why: ECDSA is DSA using ECC keys, an efficient public-key algorithm; Diffie-Hellman is primarily for IKE key agreement.
- **MQ-38** [D7] Q9 — In the e-discovery review phase, applicable data being checked against relevance: what should she do? You picked: Ensure protection of discoverable data. Correct: Perform a deep inspection. Why: deep inspection is performed in the review phase of e-discovery.
- **MQ-39** [D1] Q10 — Developing disaster-recovery plans addressing loss of power: which power-loss type is he most concerned with? You picked: Disruption from surge creating long-term loss of functionality. Correct: Disruption from a fault causing short-term power loss. Why: only a fault is a type of power loss (brownout = prolonged low voltage, surge = prolonged high voltage, spike = temporary high voltage).

### Attempt 10 — Nov 2, 2026 — 5/10 — 5 missed
- **MQ-40** [D1] Q4 — Cloud provider registering with the CSA STAR registry: which level covers third-party certification? You picked: Level Four. Correct: Level Two. Why: Level Two is Third-Party Certification.
- **MQ-41** [D1] Q6 — Which best ensures the quality/availability of data during a natural disaster? You picked: Remote Mirroring. Correct: Storage as a Service (SaaS). Why: with SaaS the data is stored where a natural disaster will not affect it.
- **MQ-42** [D1] Q7 — Which of these is NOT a breach of separation of duties? You picked: Project team performs QA testing. Correct: Computer user allowed to alter desktop configurations. Why: allowing a user to alter desktop configurations is not a breach of separation of duties.
- **MQ-43** [D6] Q9 — White-box test (tester has full knowledge of the system): which term/step applies? You picked: Validation. Correct: Leveraging. Why: "leveraging" is the site's term for this step in its listed white-box test steps.
- **MQ-44** [D1] Q10 — Certification and accreditation process governed by two US government standards: what is the correct order? You picked: Definition, Validation, Verification, Post Accreditation. Correct: Definition, Verification, Validation, Post Accreditation. Why: per the RMF/CNSS order, verification precedes validation.

### Attempt 11 — Nov 3, 2026 — 5/10 — 5 missed
- **MQ-45** [D1] Q1 — High-availability database hosted by a cloud provider not responding after hours for 15 minutes: what should she do first? You picked: Confirm incident and assess damage. Correct: Review SLA and verify uptime adhered to. Why: the SLA specifies availability; this may be a normal/scheduled outage, not an incident.
- **MQ-46** [D1] Q2 — Creating a set of procedures to follow for an adverse incident: what best describes the task? You picked: DRP. Correct: BCP. Why: a BCP is comprehensive, covering disruptions, procedures and roles; a DRP covers only recovery.
- **MQ-47** [D2] Q6 — Documenting the security program, wants to confirm proper classification of PII: who should he confer with? You picked: Data custodian (labeling). Correct: Information owner(s). Why: the information owner determines classification and protection of information.
- **MQ-48** [D6] Q9 — Using the Vulnerability Management Workflow: which of these would NOT be part of that workflow? You picked: Confirmation. Correct: Reporting. Why: per the site, the workflow parts are Detection, Validation and Remediation; Reporting is not part of it.
- **MQ-49** [D1] Q10 — Following NIST SP 800-30, after identifying threat sources/events and vulnerabilities: what is the next step? You picked: Identification of threat events. Correct: Determine likelihood of occurrence. Why: order is identify threat sources/events, identify vulnerabilities, determine likelihood, determine magnitude, then determine risk.

### Attempt 12 — Nov 3, 2026 — 5/10 — 5 missed
- **MQ-50** [D3] Q4 — Researching link vs end-to-end encryption: which statement about link encryption is correct? You picked: Link encryption only encrypts data/payload, leaving header unencrypted. Correct: Link encryption encrypts all data along the path, including header/routing information. Why: link encryption encrypts everything along the path, header included.
- **MQ-51** [D1] Q5 — Annual BIA review uncovers a discrepancy/missing systems: what should be done to confirm the findings? You picked: Perform risk assessments on newly identified systems. Correct: Engage with business process owners to confirm findings. Why: business process owners understand what the business has and needs.
- **MQ-52** [D1] Q6 — Designing/implementing administrative controls: which describes her work? You picked: Sourcing policies for senior management to review/implement. Correct: Producing policies to guide decisions and rational outcomes. Why: policies are high-level guidance for decisions.
- **MQ-53** [D1] Q7 — CISO notices suspicious activity apparently from a senior network administrator's account: what should she do? You picked: Perform log analysis. Correct: Provide paid vacation to the senior network administrator and investigate. Why: mandatory paid vacations are a prudent control, giving an opportunity to investigate.
- **MQ-54** [D5] Q10 — Securing the corporate network against unauthorised access, weak passwords a concern: best first step? You picked: Conduct training sessions on password security. Correct: Develop a strict password policy. Why: a strict password policy is essential to establish password guidelines.

### Attempt 13 — Nov 4/5, 2026 — 6/10 — 4 missed
- **MQ-55** [D7] Q4 — Manager cannot open last month's payroll database files due to corruption, needs them restored by tomorrow: which restore method best expedites recovery? You picked: Restore via differential backup. Correct: Restore via full backup. Why: a full backup is the fastest to restore from (a single backup set).
- **MQ-56** [D4] Q6 — New VoIP installed on its own VLAN, with SRTP and static IP addresses: which attack is least likely to be a concern? You picked: Phishing. Correct: Eavesdropping. Why: SRTP encrypts voice traffic, so eavesdropping is the least likely concern.
- **MQ-57** [D5] Q7 — Implementing access controls across a dispersed workforce; after provisioning accounts, what is the next step? You picked: Establish entity records. Correct: Provision Access. Why: the sequence is 1) Create Identity, 2) Provision account, 3) Provision access.
- **MQ-58** [D3] Q8 — Illegal transactions succeed despite controls on a database: which database property is at fault? You picked: Database lacked Atomicity. Correct: Database has a consistency issue. Why: consistency means a transaction changes affected data only in allowed ways; atomicity is all-or-nothing.

### Attempt 14 — Nov 5, 2026 — 4/10 — 6 missed
- **MQ-59** [D1] Q2 — Senior management finds a mirrored site too cost-prohibitive: which control best ensures clients do not lose access to data during a power outage? You picked: Warm site. Correct: UPS. Why: a UPS keeps systems powered and accessible; a warm site can take up to 12 hours.
- **MQ-60** [D3] Q3 — Risk assessment at a critical-infrastructure facility (availability is the priority; findings include a SCADA password under a keyboard, no separation of duties, older power infrastructure causing daily spikes): which is the greatest risk? You picked: Separation of duties not enforced. Correct: Older power infrastructure causing spikes daily. Why: for ICS, availability is primary and power spikes threaten it.
- **MQ-61** [D8] Q4 — Characterising known threats based on the kinds of exploits leveraged: which methodology? You picked: PASTA. Correct: STRIDE. Why: STRIDE characterises known threats based on the kinds of exploits leveraged.
- **MQ-62** [D1] Q5 — Company has seen increased breaches and tasks him with creating a security-awareness program: what is the first step? You picked: Establish program objectives. Correct: Evaluate current security posture. Why: the first step is to evaluate the current security posture.
- **MQ-63** [D1] Q8 — Backup/restoration provider in a skyscraper loses electricity for 48 hours in a fire: as a customer, best course to avoid disruption? You picked: Activate DR and move to Hot site. Correct: Ensure MTD at an acceptable/manageable level. Why: MTD is the longest outage a business can tolerate before irreparable harm; hot/cold-site activation is a provider-side decision.
- **MQ-64** [D3] Q10 — In the server room terminating connections when he smells smoke / a fire starts: what should he do? You picked: Ensure all personnel safely out. Correct: Evacuate the building, notifying anyone he sees. Why: human life is the top priority — evacuate and notify others on the way out.

### Attempt 15 — Nov 5, 2026 — 2/10 — 8 missed
- **MQ-65** [D1] Q1 — Organisation breached after an employee fell for a malicious email; a gap-analysis consultant finds the incident was caused by a lack of security governance: what was most likely the issue? You picked: Best Practices. Correct: Cybersecurity Framework. Why: governance provides direction for the information-security framework.
- **MQ-66** [D5] Q2 — Implementing Type 3 (biometric) authentication devices, weighing accuracy and privacy/user comfort: which gives the best solution? You picked: Synchronous security token. Correct: Iris scan. Why: the iris is the coloured portion around the pupil used to establish identity.
- **MQ-67** [D3] Q3 — Patient records in a relational database show wrong/unreadable information in several parts: best reason for the incorrect data shown? You picked: Records protected via obfuscation / incorrect inference. Correct: Confidentiality protected through polyinstantiation (multiple instances). Why: polyinstantiation creates multiple instances of the same data to prevent a single version from being disclosed.
- **MQ-68** [D8] Q4 — Overseeing development of a new product, has just completed the architecture phase of the SDLC: what is the next step? You picked: Obtain customer requirements. Correct: Design backend software to assist creation of the product set. Why: having completed architecture, she moves to design.
- **MQ-69** [D4] Q5 — At which OSI layer does L2TP operate? You picked: Transport. Correct: Network. Why: L2TP has no native encryption and needs IPsec, which operates at the network layer.
- **MQ-70** [D2] Q6 — Finds data has been classified inappropriately: who is responsible for classification? You picked: Data Custodian. Correct: Data Owner. Why: data owners are responsible for classification and hold the legal rights to the data.
- **MQ-71** [D8] Q7 — Website giving the public information, files could be read dynamically based on user input: which control best prevents directory/path traversal? You picked: Use safe APIs and parameterized queries. Correct: Avoid reading files dynamically based on user input. Why: dynamic file reading based on user input can be exploited for directory traversal.
- **MQ-72** [D3] Q9 — Financial institution needs strong encryption with small key sizes for a new data-protection strategy: which algorithm is best? You picked: DSA. Correct: ECC. Why: ECC gives strong encryption with smaller keys than RSA; DSA is for signatures only and provides no encryption.
