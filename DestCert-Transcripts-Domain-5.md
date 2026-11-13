# DestCert CISSP — Domain 5 Video Lesson Summaries (Identity and Access Management)

Instructor layer for the DestCert track: metadata + content summaries (in the summariser's own words, not verbatim transcripts) for each main lesson video in Domain 5 of the CISSP MasterClass schedule at new.my.destcert.com/schedule, mapped to drill-list topics in the appendix. Guide wording in `DestCert-Need-To-Know-Drill-List.md` governs wherever a video summary and the guide differ. MindMap videos excluded. Pulled 2026-11-13 under the strict method (3-video batches, per-video block/line counts, reload check on every video).

---

---

## Video 1 — Introduction to Access Control
- Duration: 07:59
- Lesson: https://new.my.destcert.com/schedule/lesson/58499d7a-cc61-4edb-b2f2-2683d7dfe9c6
- Chapters: Introduction 00:00; What is Access Control? 00:50; Access Control Principles 01:46; Access Control Applicability 02:37; Access Control System 02:58; Logical Access Modes 03:33; Administration Approaches 04:33; Decentralized Administration Approach 04:46; Centralized Administration Approach 05:29; Pros & Cons of Approach Systems 06:02; Hybrid Approach 06:57; Centralized & Decentralized Access Summarized 07:31
- Transcript: 00:14–07:11; 17 blocks / 142 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Access control = ensuring only authorised people/entities reach particular resources, places or information, based on granted permissions; access follows legitimate business need. Three governing principles, explicitly framed as exam material: LEAST PRIVILEGE (only the permissions the job needs — a compromised/misused account can then do limited harm), SEPARATION OF DUTIES (split a sensitive process so no one person controls it end-to-end; fraud/error becomes detectable), NEED-TO-KNOW (see only the information the job requires). Applicability spans physical access, logical/computer access, systems, networks, databases, applications and data — not just computers. An access control system = the technologies, devices, processes and policies managing that access. Four logical access modes over an object: read-only, read/write, execute, no access. Administration approaches: DECENTRALISED (each system's owner/custodian decides — fine-grained and tailored, no single point of failure, but fragmented, inconsistent, hard to administer and hard to fully deprovision a leaver) vs CENTRALISED (one authority, consistent policy — simpler to administer/audit, easy add/remove, but a single point of failure, a bottleneck, and lacking local knowledge). HYBRID mixes them (central for the main environment, decentralised for legacy/specialised systems) and is common in real organisations.

---

## Video 2 — Access Control Services Overview
- Duration: 05:08
- Lesson: https://new.my.destcert.com/schedule/lesson/092700f9-b5e5-4df1-8b6c-26827fbc33f3
- Chapters: Introduction 00:00; Access Control Services 00:13; Identification 00:50; Authentication 01:17; Authorization 02:02; Accountability 02:24; User Identification Guidelines 03:08
- Transcript: 00:13–04:29; 10 blocks / 88 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The four access-control services, in order (this is the IAAA sequence, drill topic 5.2.1): (1) IDENTIFICATION — claiming an identity (username, user ID, employee ID, account number); a claim, NOT proof. (2) AUTHENTICATION — verifying the claim, via the three factors: knowledge (password/PIN), possession/ownership (token, smart card, phone), inherence/characteristic (fingerprint, retina, face, voice). (3) AUTHORIZATION — after authentication, deciding what the person may do and which resources they may use (permissions/rights under policy or role). (4) ACCOUNTABILITY — detailed logs/audit trails tracing actions back to a specific user. User-identification guidelines, explicitly flagged as exam-tested: a user ID must be UNIQUE to one person; must NOT be shared or generic (sharing destroys traceability/accountability); must NOT be descriptive of the person's role or function — a username advertising a privileged/admin role invites targeting.

---

## Video 3 — AAA
- Duration: 01:15
- Lesson: https://new.my.destcert.com/schedule/lesson/c69a4cfd-1bc0-4c48-ad08-e93c8f7b018a
- Chapters: Introduction 00:00; Identification, Authentication, Authorization, Accountability 00:19; AAA 00:41
- Transcript: 00:19–00:56; 2 blocks / 12 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A 75-second terminology recap: AAA = Authentication, Authorization, and Accounting — the last three of the four services, where "accounting" is accountability (the logging/tracing function). Identification is NOT part of AAA; AAA starts at authentication. (No AAA protocols — RADIUS/TACACS+/Diameter — are introduced in this lesson.)

---

## Video 4 — Authentication Types (Factors): Knowledge & Ownership
- Duration: 07:42
- Lesson: https://new.my.destcert.com/schedule/lesson/e364535a-8357-4e22-8cb3-e4366c6e0eb0
- Chapters: Introduction 00:00; Authentication Types (Factors) 00:14; Authentication by Knowledge 00:28; Authentication by Ownership 01:10; One-time Passwords 02:21; One-time Passwords - Asynchronous 02:35; One-time Passwords - Synchronous 04:03; Smart / Memory cards 04:53; Types of Smart Cards 06:01
- Transcript: 00:14–07:26; 19 blocks / 134 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): KNOWLEDGE factor: passwords, PINs, passphrases — good practice: change regularly, never share, never write down, enforce by policy/group policy. A PASSPHRASE is easier to remember and type yet stronger than a password because it is longer with more characters (likely exam point). OWNERSHIP factor: soft tokens (software, e.g. a phone app generating codes) vs hard tokens (physical devices, e.g. USB). Both tie to ONE-TIME PASSWORDS — used once, then change, so a seen code is only briefly valid. ASYNCHRONOUS OTP = challenge-response, NOT time-based (user supplies a challenge, system returns a code, user enters it). SYNCHRONOUS OTP = token and server share a predetermined algorithm synchronised in time; the code changes about every 30 seconds. Cards — the key exam distinction: SMART cards contain an embedded microprocessor and can PROCESS/execute functions and store substantial information; MEMORY cards only STORE information, no processing. Smart card types: CONTACT (inserted, physical contact with a reader) vs CONTACTLESS (wireless, e.g. RF).

---

## Video 5 — Password Vaults
- Duration: 03:06
- Lesson: https://new.my.destcert.com/schedule/lesson/0091ce9b-89c5-4b92-926b-b9bd47b0801b
- Chapters: Introduction 00:00; Password Vaults 00:19
- Transcript: 00:18–02:42; 4 blocks / 55 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A password vault (password manager) securely stores a user's many credentials, locally or in the cloud. One MASTER PASSWORD unlocks the vault and encrypts/decrypts it; the vault enables a different strong password per site/service and can generate them, instead of reuse or writing passwords down. The central risk: if the master password is lost/forgotten, NOBODY can recover the vault; if it is compromised, everything stored is at risk. Best practice: a strong master password, plus MFA to unlock the vault.

---

## Video 6 — Authentication Types (Factors): Characteristics
- Duration: 08:10
- Lesson: https://new.my.destcert.com/schedule/lesson/7d96c1cd-90a9-4ef8-bbbe-340141c55512
- Chapters: Introduction 00:00; Authentication by Characteristics and its Types 00:24; Biometric Device Considerations 01:15; Error Rate in Biometric Systems 03:12; Cross Over Error Rate (CER) 04:26; Types of Biometric Devices 05:05
- Transcript: 00:14–07:39; 17 blocks / 151 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The CHARACTERISTIC factor = biometrics, in two types: PHYSIOLOGICAL (what a person is made of — fingerprint, handprint, iris, retina) and BEHAVIOURAL (how a person behaves — voice, walk, typing). Four device considerations: processing speed (some scans are slower than a password check); user acceptance (uncomfortable systems, e.g. iris cups with bright flashes, get resisted); protection of biometric data — the MOST important: a person has only one set of fingerprints/iris/veins, so exposed biometric data can never be replaced like a password; and accuracy — unlike knowledge/ownership (binary, 100% decidable), biometrics are NOT binary and not 100% accurate (a dirty/wet finger fails a phone unlock). Error rates: TYPE 1 = false reject (a valid user rejected — irritating); TYPE 2 = false acceptance (an invalid user accepted — an attacker gets in; explicitly the WORSE error). The two rates are inversely related; their crossing point is the CROSSOVER ERROR RATE (CER) — the measure of a system's overall accuracy for comparing systems, flagged as a likely hotspot-style exam question. Physiological devices: fingerprint; hand geometry (hand shape — cinematic, rare in real life); vascular pattern (vein pattern, usually the back of the hand — Pearson VUE scans this at CISSP check-in so a returning candidate after a break can be confirmed as the same person, not a paid substitute); facial recognition (now common on phones); IRIS (the coloured ring); RETINA (the back of the eyeball, its vein pattern) — retina is the MOST ACCURATE biometric, flagged explicitly, but rarely used: users dislike the cup/bright light/temporary blinding, and a retinal scan can reveal conditions such as diabetes or pregnancy (privacy concern). Behavioural devices: voice, signature, keystroke, and GAIT (walking — camera-based gait systems are becoming common and quite accurate).

---

## Video 7 — Templates
- Duration: 04:47
- Lesson: https://new.my.destcert.com/schedule/lesson/ea9dc99d-d1ab-4f4b-a93f-1e262ef205ca
- Chapters: Introduction 00:00; Templates 00:20; 1:N Identification 01:52; 1:1 Authentication 03:07
- Transcript: 00:09–04:40; 13 blocks / 83 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The remaining "really important" piece of biometrics: a good system NEVER stores the raw biometric (no literal fingerprint/face/iris/vein image). It stores a TEMPLATE — a one-way derived value, essentially hash-like (the instructor cautions it is "not quite hashing"). Why it matters: a stolen password can be changed, but a stolen fingerprint cannot — a person can't grow new ones — so templates ensure that even a compromised template store does not hand the attacker the usable raw biometric. The exam-central contrast: 1:N IDENTIFICATION — the presenter is unknown (e.g. only a fingerprint at a door); the system templates the presentation and searches the WHOLE template database for a reasonably close match to identify the person. 1:1 AUTHENTICATION — identity is already claimed (username + password given, so identification and a first check already happened, the fingerprint is a second factor); the system compares the new template against ONLY that one claimed user's stored template. Biometric matching is approximate ("reasonably close"), never exact.

---

## Video 8 — Single & Multi-Factor Authentication
- Duration: 02:20
- Lesson: https://new.my.destcert.com/schedule/lesson/0568184f-524a-4116-ab19-913c75e7e7b4
- Chapters: Introduction 00:00; Single-Factor Authentication 00:30; Multi-Factor Authentication 01:13
- Transcript: 00:14–01:53; 4 blocks / 34 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Single-factor authentication = using only ONE of the three factor categories alone (knowledge alone, ownership alone, or characteristic alone) — posed as an exam-style question: logging in with only an RSA token is single-factor, because the token is just the ownership factor. True MFA requires two or more DIFFERENT factors, not merely two checks. The stressed trap: a bank adding a security QUESTION after a password and calling it MFA — password and security question are both KNOWLEDGE, so it is still single-factor. Rule: count distinct factor categories, not the number of prompts.

---

## Video 9 — Password-less Authentication
- Duration: 03:39
- Lesson: https://new.my.destcert.com/schedule/lesson/af4a6bbf-a83f-4fc4-af08-1af5449ae2da
- Chapters: Introduction 00:00; Password-less Authentication 00:20; Advantages of Password-less Authentication 01:23; Challenges of Password-less Authentication 02:44
- Transcript: 00:19–02:59; 4 blocks / 58 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Passwordless = verifying identity with NO password — the knowledge factor is dropped, so it relies on OWNERSHIP (OTPs, a YubiKey) and CHARACTERISTIC (physiological biometrics; behavioural — keystroke dynamics, gait, typing, voice, signature). Advantages: more secure; no complex passwords to remember; and it REDUCES PHISHING — the core explanation: a phished static password (fake bank email example) can simply be replayed by the attacker, but a captured OTP is useless (single-use, rotates every 30–60 seconds) and biometric data is much harder to capture/store/reuse. Challenges: forget your phone/YubiKey and you are locked out; biometric privacy/secrecy concerns are graver because exposed biometric data cannot be changed (echoing video 7); and passwordless systems tend to cost more. Overall verdict: often a good idea despite the downsides.

---

## Video 10 — Single Sign-on, Kerberos & SESAME
- Duration: 08:29
- Lesson: https://new.my.destcert.com/schedule/lesson/14f164cd-9be4-4ee3-b99c-a18815a56484
- Chapters: Introduction 00:00; Single sign-on 00:15; Single sign-on (pros and cons) 00:42; Single Sign-on Tokens & Tickets 01:20; Kerberos 02:35; Kerberos Process 03:20; Typical Kerberos Issues 05:39; SESAME 07:39
- Transcript: 00:15–08:11; 17 blocks / 144 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): SSO = log in once, access multiple systems/applications without re-entering credentials, via a ticket/token a central authentication service issues and other systems accept. Pros: convenience, fewer passwords, less password help-desk load, simpler central administration. Cons: concentration of risk — one compromised credential opens everything, and the SSO service is a single point of failure. KERBEROS: developed at MIT, named for Cerberus; symmetric/secret-key cryptography; port 88; built on a Key Distribution Center (KDC) = Authentication Server (AS) + Ticket-Granting Server (TGS). Process: the user gets a Ticket-Granting Ticket (TGT) from the AS, encrypted with the user's key; presents the TGT to the TGS for a service ticket; presents the service ticket to the service, which validates it. Tickets are time-limited (typically hours). Flagged Kerberos issues: strict TIME SYNCHRONISATION (only a few minutes' skew tolerated or tickets are rejected); the KDC is a single point of failure; Kerberos provides AUTHENTICATION ONLY — it does not decide what a user may do (no authorization); and only ONE TGT at a time. SESAME (Secure European System for Applications in a Multi-vendor Environment) — the European Kerberos-like counterpart using PKI/asymmetric cryptography: MULTIPLE TGTs, and it carries a Privilege Attribute Certificate (PAC) holding the user's permissions/access rights, so the resource can judge what the user may do. The key exam contrast: Kerberos = symmetric, one TGT, authentication only; SESAME = public-key, multiple TGTs, authentication + authorization + auditing. (Caution: the lesson's opening says Kerberos was intended for authentication, accounting and auditing — the later functional statement, authentication only, is the operative point.)

---

## Video 11 — Authenticator Assurance Levels (AAL)
- Duration: 01:47
- Lesson: https://new.my.destcert.com/schedule/lesson/af7f8eff-0f4d-4cb3-8015-e16c848f98a8
- Chapters: Introduction 00:00; AAL 00:32; AAL1 01:05; AAL2 01:19; AAL3 01:21
- Transcript: 00:15–01:28; 3 blocks / 24 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Authenticator Assurance Levels (NIST SP 800-63) scale how much confidence an organisation can have that the authenticator proves the user is who they claim. AAL1 (lowest) = single-factor (e.g. a password alone). AAL2 = two factors / MFA (e.g. password + token or authenticator app). AAL3 (highest) = MFA with a HARDWARE-BASED cryptographic authenticator. The repeated exam point: the ordering 1 < 2 < 3 and the factor/hardware requirement separating each level.

---

## Video 12 — Session Management & Identity Proofing
- Duration: 05:08
- Lesson: https://new.my.destcert.com/schedule/lesson/898a37d4-1e73-4b05-97dc-78895bd4b0d5
- Chapters: Introduction 00:00; What is a Session? 00:15; Session Management 00:31; Session Hijacking 00:36; How a session can be Hijacked? 00:56; Session Hijacking Prevention 01:22; Session Termination 02:13; Registration and Identity Proofing 03:55
- Transcript: 00:15–04:55; 11 blocks / 89 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A session begins once a user has identified, authenticated and been authorised; session management keeps that session secure. Session hijacking = an attacker taking over an already-authenticated session and inheriting the victim's rights — ranging from complex (VPN session hijacking) to trivially simple (walking up to a laptop left logged in IS session hijacking). The best/"perfect" exam answer for prevention: FORCE RE-AUTHENTICATION (screensaver login, password re-entry, terminate and re-authenticate); for high concern, near-continuous re-authentication (some VPNs already do this). Three session controls: SCHEDULE limitations (logins only inside an allowed window — e.g. 8–5 Mon–Fri, so a 2 AM Saturday attempt is blocked); LOGIN limitations (no shared accounts, one account per user, one concurrent login — a second simultaneous login signals a problem); TIMEOUTS (inactivity ends the session — e.g. a screensaver after ~5 minutes, also common in online banking). Registration and identity proofing: on day one, verify face-to-face that a new employee is who they claim BEFORE handing over badge and credentials — easiest via government-issued ID (driver's licence/passport). Direct link: a Registration Authority (RA) identity-proofs a person before a digital certificate is issued.

---

## Video 13 — Federated Identity Management (FIM) & SAML
- Duration: 08:58
- Lesson: https://new.my.destcert.com/schedule/lesson/6e0a660b-b2ec-4092-af79-7fa395cc24e0
- Chapters: Introduction 00:00; Federated Identity Management (FIM) 00:46; Federated Access Standards 03:51; SAML 04:50; Tokens/Tickets & XML-Protocol 06:58; SAML Components 07:26; Types of Identities / Accounts 07:41 (chapter label does not match the spoken content at that point, which continues the SAML components)
- Transcript: 00:13–08:29; 17 blocks / 150 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Federated identity management = trusted organisations sharing/attesting identity so a user authenticated by one organisation can access a partner's systems WITHOUT a separate account there. The home organisation keeps and verifies the credentials (credentials are never handed over) and vouches for the user; the partner relies on that attestation. It matters most as people join/move between organisations (employees, contractors, vendors, customers) — one username/password across federated platforms instead of a burdensome, risky login per system. Familiar example: signing in with an existing Google/Microsoft/Apple/Facebook account — the external identity provider authenticates and passes a token/ticket; the relying system validates the token instead of re-verifying the person. Stressed distinction: federation ≠ SSO — SSO is an access mechanism within an organisation/system; federation is the CROSS-ORGANISATION trust arrangement (SSO can be part of the federated experience, but they are distinct concepts). SAML (Security Assertion Markup Language): an XML-based open standard from OASIS for exchanging authentication and authorisation data, commonly used for SSO. Parties: the IDENTITY PROVIDER (authenticates/certifies the user) and the SERVICE PROVIDER / relying party (grants access based on the token). The token is carried in XML and must be validity-checked; invalid/expired tokens grant nothing. SAML's components: ASSERTIONS (the format of the exchanged information about the user/subject), PROTOCOL (the rules for requests/responses), BINDINGS (how SAML messages are transported between parties), PROFILES (how assertions + protocol + bindings are combined for use).

---

## Video 14 — Just-in-Time (JIT) Access
- Duration: 03:17
- Lesson: https://new.my.destcert.com/schedule/lesson/b5da9a88-a00c-4104-aa74-6ce5d8a8da6b
- Chapters: Introduction 00:00; Just-in-Time (JIT) Access 00:15; JIT Access definition 01:58; Benefits of JIT Access 02:24
- Transcript: 00:15–02:34; 6 blocks / 50 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The problem: accounts granted elevated/admin privileges for a task keep that STANDING access indefinitely — a persistent target whose full privilege can be exploited until misuse is detected. JIT access is the remedy: just enough access, for just long enough, for a specific task, only when needed. Flow: the user requests access → it is approved (manager/administrator) → granted for a bounded, task-tied period → AUTOMATICALLY revoked/disabled at expiry. It is a practical implementation of least privilege: smaller exposure window, harder privilege escalation and lateral movement, and a clearer audit record of who had elevated access, when and why. Especially useful for privileged/admin and contractor/vendor access needed only occasionally.

---

## Video 15 — Principle of Access Control
- Duration: 01:32
- Lesson: https://new.my.destcert.com/schedule/lesson/50c272ba-5e13-4d24-ab0a-0e53fee6a587
- Chapters: Introduction 00:00; Principle of Access Control 00:26; Accountability 00:42
- Transcript: 00:15–01:14; 3 blocks / 21 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A short single-point lesson: ACCOUNTABILITY is the principle of access control — its other name, and the most important thing access control does. The sequence that achieves it: uniquely IDENTIFY someone (without unique identification, nobody can be held responsible) → properly AUTHENTICATE them → properly AUTHORISE them (least privilege, need-to-know, separation of duties) → LOG AND MONITOR what they do. Only with all of those in place is accountability achieved.

---

## Video 16 — IDaaS
- Duration: 03:07
- Lesson: https://new.my.destcert.com/schedule/lesson/53bdecb1-f615-44e8-a92a-c811747c1aee
- Chapters: Introduction 00:00; Types of Identities / Accounts 00:47; IDaaS Capabilities 02:39
- Transcript: 00:20–02:53; 6 blocks / 47 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): An ACCOUNT is the credential used to authenticate (username/password, certificate, token). Account types: PHYSICAL accounts (individual accounts belonging to a person, tied to a specific system) and LOGICAL accounts (not tied to a person — the captioning of this definition is garbled/truncated, so treat the wording cautiously). IDaaS = Identity as a Service: IAM delivered from the cloud by a third-party vendor instead of built/run entirely in-house (the organisation still has work to do; the function is offloaded). Vendors named: Okta (described as the most popular), Microsoft Entra ID, Google. Capabilities: SSO; MFA (Google Authenticator as an example); provisioning incl. AUTOMATIC provisioning (a newly created user automatically receives access to various systems); user access requests; and LIFECYCLE MANAGEMENT driven by HR — joiner/mover/leaver events trigger create/modify/delete of access respectively.

---

## Video 17 — Access Control Philosophies
- Duration: 12:17
- Lesson: https://new.my.destcert.com/schedule/lesson/c610b7ea-f8ef-4c6a-8044-5795442ef022
- Chapters: Introduction 00:00; Access Control Philosophies 00:30; 1. DAC (Discretionary Access Control) 02:10; RBAC (Role-Based Access Control) 02:28; Rule-Based (Rule-Based Access Control) 03:30; Attribute Based (Attribute-Based Access Control) 03:56; XACML 07:00; Attribute Based Example 07:20; Fun Trivia about CAPTCHA 08:17; 2. MAC (Mandatory Access Control) 10:43; 3. Non-Discretionary (Non-Discretionary Access Control) 11:50
- Transcript: 00:13–12:02; 26 blocks / 215 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The three overarching philosophies — explicitly the main ones to expect on the exam (RBAC included): (1) DAC — the owner/creator of a resource decides at their discretion who may access it and can grant/change that access; flexible but comparatively LESS secure because control rests with individual owners. (2) MAC — access decided CENTRALLY by the system/authority, not the owner, using security labels/clearances (e.g. a Secret clearance reaches Secret and below, never Top Secret); suited to high-security military/government settings; more secure, less flexible. (3) NON-DISCRETIONARY — centrally set policy/authority decides rather than the owner; the umbrella family covering RBAC, RULE-BASED and ABAC. RBAC: access follows role/job function — the user gets a role, the role carries the permissions, changing role changes access; easier to manage at scale. RULE-BASED: access follows defined rules/conditions that must be met. ABAC: access follows attributes of the SUBJECT (department, job title, clearance), the RESOURCE (classification, type) and the ENVIRONMENT/CONTEXT (time, location, device), evaluated against policy — very fine-grained and flexible, but more complex. XACML is the XML-based standard language for expressing ABAC policies; its architecture: PAP (policy administration point — authors/stores policy), PDP (policy decision point — evaluates the request), PEP (policy enforcement point — enforces the decision), PIP (policy information point — supplies attribute information); a worked attribute-based example follows. Trivia: CAPTCHA = Completely Automated Public Turing test to tell Computers and Humans Apart — designed so humans pass and bots cannot (reCAPTCHA mentioned).

---

## Video 18 — Types of RBAC
- Duration: 03:21
- Lesson: https://new.my.destcert.com/schedule/lesson/fcbded4c-2d80-4fdd-b10f-5501b995b1c2
- Chapters: Introduction 00:00; Types of RBAC 00:19; Non-RBAC 00:38; Limited-RBAC 00:52; Hybrid-RBAC 01:46; Full-RBAC 02:32
- Transcript: 00:15–03:04; 8 blocks / 53 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Explicitly flagged as a topic that has shown up fairly recently on the exam — four types of RBAC by how far an organisation has deployed it: (1) NON-RBAC — no role-based access in use at all (access is probably rule-based instead). (2) LIMITED RBAC — roles exist only WITHIN specific applications (e.g. finance payroll clerk L1/L2/manager roles govern the finance app but not the same user's CRM access) — a subtle definition, stressed twice. (3) HYBRID RBAC — keeps the application-specific roles AND adds roles that span multiple applications (one role granting payroll + CRM + more). (4) FULL RBAC — RBAC deployed throughout the entire organisation in every system; a role can grant access to anything. Reality check: full RBAC is incredibly hard, near-impossible in large organisations with many legacy apps — most organisations sit between limited and hybrid.

---

## Video 19 — Roles & Groups
- Duration: 02:03
- Lesson: https://new.my.destcert.com/schedule/lesson/ce22a3ff-4ccd-4db0-8fb4-57a630e28609
- Chapters: Introduction 00:00; What are Roles? 00:28; What are Groups? 00:50; Roles vs. Groups 01:05
- Transcript: 00:18–01:30; 5 blocks / 22 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A role = a set of permissions tied to a JOB FUNCTION (e.g. payroll manager level 1 vs level 2 get different access; an employee can hold one or more roles). A group = simply a collection of USERS, given access as a collection. The stressed contrast: roles are FUNCTION-centric (built around what the job does); groups are USER-centric (built around who the people are). The instructor explicitly downplays exam weight: probably not super important for the exam, "just in case."

---

## Video 20 — Context / Attribute Based Access Controls
- Duration: 08:45
- Lesson: https://new.my.destcert.com/schedule/lesson/79666cbd-40d0-476c-985c-2b04c477b158
- Chapters: Introduction 00:00; Attribute Based Access Controls 00:15; Zero Trust 00:38; Discretionary Attribute / Context Based Access Controls 02:28; User 02:30; Environment 03:22; Resource 04:18; Action 04:55; Authorization Engine 05:14; Policy 05:40; XACML 06:06; Example of Attribute / Context Based Access Controls 06:33
- Transcript: 00:15–08:15; 18 blocks / 165 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): ABAC is also called CONTEXT-BASED access control (CBAC) — the names are interchangeable; watch for both on the exam. Framing principle: ZERO TRUST — trust nothing, verify everything; never assume trust from being inside, especially with cloud/broad access dissolving traditional defences. ABAC goes beyond MFA: MFA is excellent, but ABAC adds continuous, PER-ACTION evaluation of attributes rather than a single login check. Four attribute groups: USER (role, experience, department, country, time zone — e.g. a Mon–Fri 08:00–17:00 Pacific user logging in at 03:00 Sunday, or a Zimbabwe-based user appearing in Switzerland, or an accounting user reaching for engineering systems, all raise suspicion); ENVIRONMENT/SYSTEM (device manufacturer and OS — an issued Dell on Windows 11 is expected, a Lenovo/Mac/Windows XP/unfamiliar Linux is not — plus IP address, MAC address, installed certificates, GPS latitude/longitude); RESOURCE (what is being accessed — database vs SharePoint vs a file — and its classification, e.g. an internal public-policy wiki vs a highly sensitive database); ACTION (what the user wants to do — looking up a field value vs deleting the whole database/dropping a table are very different). Attributes feed an AUTHORIZATION ENGINE that makes a risk-based permit/deny decision per action, programmed by a POLICY document of logic statements; the language for those policies is XACML. Worked example: Google reCAPTCHA's "I'm not a robot" checkbox — the click alone proves nothing; Google weighs device, OS, time and MOUSE MOVEMENT (a robot moves straight to the centre; a human moves erratically) and either lets the user in or steps up to the 3×3 picture-grid challenge. The instructor closes by calling ABAC an important type of discretionary access control to remember for the exam. (Framing tension noted: video 17 presented non-discretionary as the umbrella over RBAC/rule-based/ABAC, while this video and video 21 frame ABAC in discretionary terms — guide wording governs.)

---

## Video 21 — Access control summary
- Duration: 02:46
- Lesson: https://new.my.destcert.com/schedule/lesson/4b443cfc-fe17-4059-97c0-1b214cee0aa7
- Chapters: Introduction 00:00; Access Control Summary 00:35; Discretionary Access Control (DAC) 00:49; Role-based Access Control (RAC) 01:06 [chapter label typo — RBAC is meant]; Rule-based Access Control 01:16; Attribute-based Access Control (ABAC) 01:32; Mandatory Access Control (MAC) 01:44
- Transcript: 00:15–02:02; 4 blocks / 44 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A recap aimed explicitly at drag-and-drop term-to-definition exam questions — one defining characteristic per philosophy: DAC = the OWNER decides who gets access (right, because owners are accountable for the system). RBAC = create roles, assign roles to users, the role defines access. RULE-BASED = a file of rules, often called an ACL (access control list) — Bob gets one directory, Alice another. ABAC (context-based) = a much more informed decision from a whole bunch of attributes. MAC = the SYSTEM decides; its key requirement is LABELLING — every employee gets a security clearance, every asset a classification, and the system decides from those two; labelling is how a classification is marked on an asset.

---

## Video 22 — Access Policy Enforcement
- Duration: 02:09
- Lesson: https://new.my.destcert.com/schedule/lesson/c018fa31-697f-47c9-a9b2-66c9cabca984
- Chapters: Introduction 00:00; Access Policy Enforcement definition 00:23; PDP & PEP 00:43; Policy Decision Point (PDP) 00:50; Policy Enforcement Point (PEP) 01:13
- Transcript: 00:19–01:50; 4 blocks / 33 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): How a decided policy becomes an enforced outcome, split into two roles that must not be confused: the POLICY DECISION POINT (PDP) decides whether a user may access a system/resource, based on the organisation's access requirements/policies and factors such as need-to-know, least privilege and security level. The POLICY ENFORCEMENT POINT (PEP) carries the decision out — allowing access on a yes, blocking it on a no. PDP decides, PEP enforces. They can be combined in one system, or run as a central decision point with distributed enforcement points.

---

## Video 23 — Provisioning Lifecycle
- Duration: 03:46
- Lesson: https://new.my.destcert.com/schedule/lesson/7a9f7919-b7f4-4cda-a257-e0a942e262cc
- Chapters: Introduction 00:00; Provisioning Lifecycle 00:16; Use Access Review 02:10; How often should access reviews be performed? 02:35; Which type of accounts should be reviewed most often? 03:22
- Transcript: 00:14–03:31; 10 blocks / 67 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The provisioning (identity) lifecycle in four parts: (1) CREATION/PROVISIONING — a joiner's account is created with access fitted to role/job responsibilities under least privilege and need-to-know (never a generic or excessive grant). (2) MAINTENANCE — as roles change (moves, new work, promotions), access is updated to stay in step with the current job rather than left as granted on day one. (3) DE-PROVISIONING/REVOCATION — access is removed when a person leaves or no longer needs it for their role. (4) ACCESS REVIEW (user access review / periodic review / recertification) — a regular check that current access is still appropriate, catching excessive, outdated or unjustified access. Review FREQUENCY is deliberately non-numeric: there is no fixed correct interval — as often as necessary, judged by the asset's value and sensitivity, the system's complexity, the risk of the access, and applicable regulations. PRIVILEGED accounts are the category to review most often.

---

## Video 24 — Service Accounts
- Duration: 02:23
- Lesson: https://new.my.destcert.com/schedule/lesson/99268fb7-ee14-4324-93b6-9ddf2a952106
- Chapters: Introduction 00:00; Service Accounts 00:19; Service Accounts Management 00:56
- Transcript: 00:19–02:05; 4 blocks / 34 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A service account is a NON-HUMAN account used by an application/system/service (not a person) to authenticate, access resources and run processes/jobs automatically in the background — the contrast with an interactive user account belonging to a person. Because it must work without anyone logging in, it is often created with broad privilege (example: a backup service needing access to a very large amount of the organisation's data/systems) — and that broad, long-lived, little-noticed privilege is the risk if it is over-privileged, forgotten, poorly tracked or compromised. Management discipline: maintain an inventory (what exists, what each is for); least privilege (only the access the service actually needs); strong randomly generated passwords, never hard-coded/embedded credentials; monitor and audit use; review regularly; disable/remove when no longer needed. The managed alternative: managed service accounts — standalone MSA vs group gMSA — where the SYSTEM automatically manages the password, including rotation, instead of a manually set static password.
- NOTE: a total-count check in this batch established Domain 5 has 25 main lesson videos, not 24 as the original exploration counted — position 25 is "5.6 Implement authentication systems" (01:21), pulled next.

---

## Video 25 — 5.6 Implement authentication systems
- Duration: 01:21
- Lesson: https://new.my.destcert.com/schedule/lesson/b5833a9a-05af-4d61-9475-f61a77190390
- Chapters: Introduction 00:00; Should security be involved if the organization is implementing any authentication system? 00:25
- Transcript: 00:15–01:06; 2 blocks / 15 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The shortest lesson in the domain — a one-point coda. Section 5.6 is one of the sections added to the CISSP exam in the 2021 update. Its entire substance is a single rhetorical question: when an organisation implements ANY authentication system — named examples: single sign-on, federated identity management, RADIUS/TACACS (the puller notes the instructor says RADIUS/TACACS are covered in Domain 4) — should the SECURITY function be involved in the implementation? The instructor's answer is an emphatic yes: security involvement is required, not optional, whenever any authentication system is implemented — presented as common sense rather than technical detail. No framework, steps, definitions, numbers or comparisons are given. CONFIRMED by this batch: video 25 is the LAST main lesson video in Domain 5 (25/25); the next item is the Domain 5 Knowledge Assessment, then the two MindMaps, flashcards and practice questions.
- NOTE: the live count established Domain 5 has 25 main lesson videos, not 24 as originally explored — the exploration count missed this final video. Total main videos for Domains 1–6 is therefore 205, not 204.

---

# Coverage appendix — Domain 5 videos vs drill-list topics

All 25 main lesson videos pulled (the domain has 25, not the 24 originally counted — the final video, "5.6 Implement authentication systems," was missed in the exploration count). All 25 transcripts were STABLE across three loads each — no alternate versions anywhere in Domain 5; only 1-second duration-label differences on a few videos. All entries are metadata + content summaries, not verbatim reproductions.

**31 of 31 Domain 5 drill topics covered:**
- 5.1.1 Access Control Principles — V1 (least privilege, separation of duties, need-to-know, flagged as exam material), V15 (accountability as the principle)
- 5.1.2 Administration Approaches — V1 (centralised vs decentralised vs hybrid)
- 5.2.1 Access Control Services — V2 (the IAAA sequence), V3 (AAA = authentication, authorization, accounting; identification is NOT part of AAA)
- 5.2.2 Identification — V2 (identification as a claim, user-ID guidelines), V7 (1:N identification vs 1:1 authentication)
- 5.2.3 Authentication by Knowledge — V4 (passwords vs passphrases), V5 (password vaults)
- 5.2.4 Authentication by Ownership — V4 (soft/hard tokens, async vs sync OTP, smart vs memory cards)
- 5.2.5 Authentication by Characteristics — V6 (biometrics, Type 1/2 errors, CER), V7 (templates)
- 5.2.6 Factors of Authentication — V8 (count factor CATEGORIES, not prompts)
- 5.2.7 Password-less Authentication — V9
- 5.2.8 Single Sign-on (Kerberos) — V10 (Kerberos + SESAME contrast)
- 5.2.9 Authenticator Assurance Levels (AAL) — V11 (NIST SP 800-63, AAL1/2/3)
- 5.2.10 Session Management — V12 (re-authentication as the best prevention answer)
- 5.2.11 Registration and Proofing of Identity — V12 (face-to-face proofing with government ID; RA proofing before certificate issuance)
- 5.2.12 Federated Identity Management (FIM) — V13 (federation ≠ SSO)
- 5.2.13 Federated Access Standards — V13 (SAML: assertions, protocol, bindings, profiles)
- 5.2.14 Just-In-Time Access — V14
- 5.2.15 Principle of Access Control — V15 (accountability, via unique ID → authentication → authorisation → logging)
- 5.3.1 Identity as a Service (IDaaS) — V16
- 5.4.1 Authorization Mechanisms — V17 (the three philosophies overview)
- 5.4.2 Discretionary Access Control (DAC) — V17, V21
- 5.4.3 Groups, Roles and RBAC — V17 (RBAC), V18 (four types of RBAC, recently on the exam), V19 (roles function-centric vs groups user-centric)
- 5.4.4 Rule-based Access Control — V17, V21 (rule file = ACL)
- 5.4.5 Attribute Based Access Control (ABAC) — V17 (incl. XACML PAP/PDP/PEP/PIP), V20 (four attribute groups, Zero Trust framing, reCAPTCHA example), V21
- 5.4.6 Mandatory Access Control (MAC) — V17, V21 (labelling requirement)
- 5.4.7 Non-Discretionary Access Control — V17 (umbrella over RBAC/rule-based/ABAC)
- 5.4.8 Access Control Summary — V21 (video-only topic in the guide; the summary video itself)
- 5.4.9 Access Policy Enforcement — V22 (PDP decides, PEP enforces)
- 5.5.1 Provisioning Lifecycle Importance — V23 (four-part lifecycle)
- 5.5.2 User Access Review — V23 (no fixed interval; privileged accounts reviewed most often)
- 5.5.3 Service Accounts — V24 (non-human accounts; MSA vs gMSA)
- 5.6.1 Implement Authentication Systems — V25 (security must be involved in implementing any authentication system)

Cross-lesson tension flagged: V17 presents non-discretionary as the umbrella over RBAC/rule-based/ABAC, while V20/V21 frame ABAC in discretionary terms — guide wording governs.
