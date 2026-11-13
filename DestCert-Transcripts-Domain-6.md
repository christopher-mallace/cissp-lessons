# DestCert CISSP MasterClass — Domain 6 Lesson Notes (Security Assessment and Testing)

Pulled 2026-11-13 from https://new.my.destcert.com/schedule (CISSP MasterClass), main lesson videos only — MindMaps excluded. 16 main videos expected. Each entry: lesson metadata (duration, URL, chapters, transcript timestamp range, block/phrase-line counts, reload-stability result) plus a content summary in our own words, NOT a verbatim reproduction of the transcript.

## Video 1 — Introduction to Security Assessment and Testing
- Duration: 10:25
- Lesson: https://new.my.destcert.com/schedule/lesson/64b05e22-f29f-4524-ada6-e596f535e6d5
- Chapters: Introduction 00:00; Purpose of Security Assessment and Testing? 02:53; Validation 03:39; Verification 05:24; Effort to invest in testing? 07:38; Testing Strategies 07:58; Role of Security Professional 09:24
- Transcript: 00:14–09:24; 25 blocks / 199 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Domain 6 is the ASSURANCE pillar — every control has a functional side and an assurance side, and assessment/testing supplies the assurance. A complexity slide (lines of code: ~50k average iPhone app, 6.5M Boeing avionics, 50M Windows, 2B Google services) is explicitly NOT for the exam; line count is a rough, imperfect complexity measure. Testing must test SECURITY functionality — the instructor objects to "non-functional testing" as a label because security must actually work and the label risks it being dropped when projects run late. Testing spans the whole life cycle, conception through end of life (secure destruction/move of data). VALIDATION (at the very start) = are you building the RIGHT product — fully capturing business requirements first (miss one and you discover card data in production and have to bolt on PCI). VERIFICATION (after building) = are you building the product RIGHT — it works as designed and its security controls work. Verification's three Cs: COMPLETENESS, CORRECTNESS, CONSISTENCY (and the same Cs apply to test cases). Certainty is never 100%; the aim is a level of confidence driven by stakeholder requirements and the system's VALUE — which also drives how much testing effort to invest. Three testing STRATEGIES by who tests: INTERNAL (own auditors, own systems); EXTERNAL (own auditors assessing a provider, or an outside auditor assessing the organisation); THIRD-PARTY (consumer + provider + external auditor — e.g. Azure hires a trusted audit firm and gives all customers the one report). The security professional does NOT conduct the testing: stakeholders/owners/management provide the assurance; security monitors, advises and reviews results from a security perspective.

---

## Video 2 — Location of Assessment
- Duration: 02:36
- Lesson: https://new.my.destcert.com/schedule/lesson/6f87ac44-fca3-4054-b198-46cab02a3166
- Chapters: Introduction 00:00; Location 00:18; On-premise 00:30; Cloud 00:44; Hybrid 00:57
- Transcript: 00:01–02:30; 6 blocks / 40 phrase lines (stable across three loads; no alternate version). NOTE: the panel's final block (02:30) contains only the word "you" — the closing ~6 seconds appear truncated in the panel as shown.
- Content summary (not a verbatim reproduction): WHERE a system lives changes how you assess/test it (approach, scheduling, coordination). ON-PREMISE: own data centres — physical security well understood, infrastructure known, systems often custom-built and more complex; assembling systems and getting permission comparatively straightforward. CLOUD: runs on a provider's infrastructure (Azure example; a single Azure data centre has 250,000+ servers, built from shipped-in container units); commonly SHARED (multi-tenant) infrastructure with a single-tenant option at extra cost; the provider controls facility physical security. HYBRID: on-premise + cloud combined (example: ~80% moved to cloud, the most sensitive/top-secret material kept on-premise) — cover both sides and liaise with the provider for the cloud side.

---

## Video 3 — Software Testing Stages
- Duration: 05:13
- Lesson: https://new.my.destcert.com/schedule/lesson/8aaa36ec-96ea-46b0-b9b8-535eab38475a
- Chapters: Introduction 00:00; Software Testing 00:13; Examples of Testing Performed 00:26; When should security become involved in testing? 01:58; Software Testing Stages 02:26; Interface Testing 04:48
- Transcript: 00:13–05:01; 10 blocks / 101 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Security's involvement across the life cycle (the diagram used is explicitly NOT to be memorised — a visual aid only): PLANNING — requirements incl. all security requirements captured and validated; DESIGN — heavy involvement designing the controls (CIA etc.); DEVELOPMENT — checks controls are being built in (vulnerability assessments; unit, integration, system testing); DEPLOYMENT (QA/test → production) — vulnerability assessments and log analysis; OPERATION — continued testing, validation, vulnerability assessment, log analysis; plus DECOMMISSIONING (not on the diagram) — secure data destruction. Explicit exam takeaway: asked WHEN security should become involved, answer the EARLIEST possible stage — security from the start and throughout ("baking security in"). Testing stages in build-up order: UNIT testing (a single unit in isolation — e.g. the keyboard-input team testing its own unit of Windows); INTERFACE testing (units connect via standardised interfaces — Lego analogy: a block bought today still fits 1950s blocks because the interface is precisely defined); INTEGRATION testing (groups of units together); SYSTEM testing (the whole integrated system as one).

---

## Video 4 — Software Testing Techniques
- Duration: 09:33
- Lesson: https://new.my.destcert.com/schedule/lesson/d2ddc9af-275d-45f3-ae06-eba786a31440
- Chapters: Introduction 00:00; Testing Techniques 00:20; Manual & Automated Testing 00:31; Runtime Testing (Static, Dynamic & Fuzz) 00:54; Access to Code (Black box & White Box Testing) 02:48; Test Types (Positive, Negative & Misuse) 03:28; Equivalence Partitioning & Boundary Value Analysis 04:35; Testing Examples 07:25; Test Coverage Analysis 08:40
- Transcript: 00:13–09:11; 26 blocks / 170 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Techniques organised along how testing is performed, when code is examined, and what access the tester has. MANUAL testing = a person working through the system (slow, repetitive); AUTOMATED = scripts/scanners running checks repeatedly — complementary, not replacements (people still write the scripts by hand). STATIC testing examines source code WITHOUT running it; DYNAMIC testing runs and exercises the system (manual or automated). FUZZING is dynamic: malformed/unexpected/mutated input to expose buffer overflows, crashes, hangs. BLACK-BOX = no source access, behaviour inferred from inputs/outputs, as an outside user/attacker would; WHITE-BOX = source access, code inspected directly — the distinction is explicitly stressed. Test types: POSITIVE (system used as intended, valid input); NEGATIVE = MISUSE testing (deliberately unintended use or invalid input — should fail safely). EQUIVALENCE PARTITIONING groups inputs into classes treated the same way, so one representative per class cuts test count; BOUNDARY VALUE ANALYSIS tests the class edges (just inside, on, just outside), where errors cluster. Worked examples: age 18–65 (test 17/18/65/66); password length 8–16 (partitions below 8 / 8–16 / above 16; boundaries 7/8 and 16/17). TEST COVERAGE ANALYSIS measures how much of the code testing has actually exercised — no threshold percentage is given.

---

## Video 5 — Types of fuzzing
- Duration: 02:21
- Lesson: https://new.my.destcert.com/schedule/lesson/00305cab-ce9e-40bd-8c95-a500f6e8297f
- Chapters: Introduction 00:00; Fuzzing 00:20; Mutation vs. Generation 00:34; Mutation Fuzzer 01:10; Generation Fuzzer 01:23
- Transcript: 00:14–01:42; 4 blocks / 40 phrase lines (stable across three loads; no alternate version). NOTE: the last transcript timestamp (01:42) sits ~39 seconds before the video's end.
- Content summary (not a verbatim reproduction): The one central distinction — MUTATION vs GENERATION fuzzing. A mutation fuzzer starts from a valid SEED input (a real file/genuine input) and randomly alters it, running each mutated version and watching for crashes — easy to set up (no input model needed), but most outputs are invalid and rejected early. A generation fuzzer builds inputs FROM SCRATCH from a model/specification of the expected format or protocol, so its inputs pass initial validation and reach deeper code paths — but it needs that format knowledge and more up-front work, and is often custom-built for one application. The exam point: whether the input is mutated from a seed or generated from a specification.

---

## Video 6 — Interactive Application Security Testing (IAST)
- Duration: 01:40
- Lesson: https://new.my.destcert.com/schedule/lesson/39d03f74-1dcd-45e2-a431-08e0e875d9b8
- Chapters: Introduction 00:00; Testing techniques 00:22; Static Application Security Testing (SAST) 00:49; Dynamic Application Security Testing (DAST) 01:01; Interactive Application Security Testing (IAST) 01:07
- Transcript: 00:18–01:06; 5 blocks / 21 phrase lines (stable across three loads; no alternate version). NOTE: the last transcript timestamp (01:06) sits ~34 seconds before the video's end.
- Content summary (not a verbatim reproduction): SAST examines source code while the application is NOT running ("static" = not running; the object is the source code itself). DAST tests the RUNNING application from the outside. IAST is the combination — testing a system while it runs WHILE still having access to the source code — giving DAST's runtime behaviour plus SAST's code-level visibility (Venn-diagram framing).

---

## Video 7 — Decision table & state-based analysis
- Duration: 03:30
- Lesson: https://new.my.destcert.com/schedule/lesson/4910390e-a5c8-4a5e-bd8a-4aaef6941256
- Chapters: Introduction 00:00; Decision table 00:27; State-based 01:54
- Transcript: 00:15–03:01; 7 blocks / 60 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Two further testing approaches. A DECISION TABLE is a systematic grid for testing COMBINATIONS of inputs/conditions against expected outputs — conditions across the top, possible values branching down, outcomes at the bottom — so every combination becomes a distinct case and none gets missed (worked example: a website registration form printing customer cards, with member/not-member type conditions; the captioning of the example's exact fields is garbled). STATE-BASED ANALYSIS models the system as STATES and the TRANSITIONS between them (ideally as a diagram): an action/event moves the system from one state to another, and testers verify each transition behaves as intended.

---

## Video 8 — Vulnerability Assessment & Penetration Testing
- Duration: 09:25
- Lesson: https://new.my.destcert.com/schedule/lesson/c311eaa9-dd58-4756-a4a2-e0b22633e75d
- Chapters: Introduction 00:00; Purpose of Vulnerability Assessment 00:16; Vulnerability Assessment vs Penetration Testing 01:00; Typical Testing Process 04:54
- Transcript: 00:15–08:38; 19 blocks / 168 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Assess yourself before real attackers do — find weaknesses, understand what they affect and how severe they are, and produce a report so management can prioritise fixes. The central contrast: a VULNERABILITY ASSESSMENT is the broader activity — an automated scan across the environment that identifies and lists vulnerabilities with severity WITHOUT exploiting them (example: scanning a SUSE Linux machine, checking its Oracle version/patch state, reporting unpatched findings). A PENETRATION TEST is narrower and focused — actively trying to EXPLOIT a vulnerability to prove it is really exploitable (e.g. testing the edge of a website whose underlying weakness may affect ~2,000 pages). Assessment finds and grades; pen testing validates by exploitation. Named scanners: Nessus, Qualys, OpenVAS. Typical process: agree SCOPE and RULES OF ENGAGEMENT (incl. the IP range in scope) → run the scan → review the report and verify findings (check FALSE POSITIVES) → identify CVE IDs and severity for confirmed issues → pen-test the exploitable-looking ones → document everything for management so remediation is prioritised by severity.

---

## Video 9 — Red, Blue and Purple Teams
- Duration: 03:18
- Lesson: https://new.my.destcert.com/schedule/lesson/91bdd12d-35a9-4448-b05f-b953fa729ac2
- Chapters: Introduction 00:00; Red team 00:29; Blue team 01:08; Purple team 02:07
- Transcript: 00:19–02:00; 6 blocks / 55 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Colour names describe ROLES in vulnerability management/pen testing. RED team = the simulated attacker: offensive security — ethical hacking, penetration testing, simulated spear-phishing and internal phishing campaigns, tracking the latest threats and how they could be applied. BLUE team = the defender: security operations — monitoring systems and log files, watching monitoring systems/alerts (SIEM), handling incidents. Origin trivia (hedged by the instructor as his recollection): US military war games — blue = the US "good guys," red = the opposing threat — carried into security. PURPLE is somewhat misnamed: not usually a separate team at all, but red and blue working TOGETHER collaboratively — sharing threat intelligence and findings so blue can mitigate what red found; the purpose is joint learning and information sharing, not competition to the point the teams stop talking.

---

## Video 10 — Vulnerability Testing Techniques, Banner Grabbing, Fingerprinting, & Interpreting Results
- Duration: 11:45
- Lesson: https://new.my.destcert.com/schedule/lesson/66e280cd-8f8d-4c53-bd5c-bfdc4a3cea7c
- Chapters: Introduction 00:00; Vulnerability & Pen Testing Techniques 00:45; Automated vulnerability scanners 03:08; Additional Testing Techniques 04:50; Banner Grabbing & Fingerprinting 06:45; Interpreting & Understanding Results 08:27; False Positives & False Negatives 10:51
- Transcript: 00:16–11:30; 23 blocks / 232 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Testing framed by perspective × knowledge. INTERNAL test simulates an insider; EXTERNAL simulates an outsider. Knowledge: ZERO = black-box, PARTIAL = grey-box, FULL = white-box (internal + full knowledge = malicious insider; external + black-box = random internet attacker). BLIND testing = the assessor gets no information (no IPs, no credentials); DOUBLE-BLIND = the SOC is also not told, so the exercise tests detection/response — approved by SENIOR MANAGEMENT, not the assessment team. Automated scanners (Nessus, Qualys): an UNCREDENTIALED scan sees only the outsider/no-login view — a good simulation of it, but many false positives; a CREDENTIALED scan logs in, checks patching/configuration against a baseline, cuts false positives and gives better compliance evidence — but handing scanner credentials to a tool is itself a risk. WAR DIALING dials number ranges hunting a modem/fax that answers (still valid: POTS is very reliable, works in power cuts, and forgotten modem backdoors from decades ago may sit unmonitored on critical systems). WAR DRIVING hunts wireless access points, ideally unencrypted or WEP. The EXACT VERSION matters (flagged important): different versions are vulnerable to different things. BANNER GRABBING exploits verbose errors (a 404 revealing the exact Apache Tomcat version) — systems must not advertise that detail. FINGERPRINTING is subtler: packet construction differs slightly between OSes/applications despite OSI standardisation, so the exact version can be inferred. Interpreting results: CVE gives one common identifier so vendors/tools don't use different names for the same flaw; CVSS scores 0–10 (0 ≈ don't care, 10 ≈ run screaming) — reports should list CVE + CVSS per finding so the highest scores are fixed first. FALSE POSITIVES (tool reports a vuln that isn't there; common in uncredentialed scans) vs FALSE NEGATIVES (tool says fine when a vuln exists) — false negatives are FAR worse (false sense of security); tune to cut false positives without creating false negatives.

---

## Video 11 — SCAP, Breach Attack Simulation & Compliance Checks
- Duration: 07:04
- Lesson: https://new.my.destcert.com/schedule/lesson/691b6e11-b7b6-4f34-9e0e-5d0082ddc3eb
- Chapters: Introduction 00:00; Security Content Automation Protocol (SCAP) 00:42; Breach Attack Simulation 02:03; Security Content Automation Protocol (SCAP) vs. Breach Attack Simulation 03:39; Compliance Checks 04:10
- Transcript: 00:19–06:44; 13 blocks / 130 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): SCAP (Security Content Automation Protocol) = the NIST standard for automating patch/configuration checking in a machine-readable, standardised way. Components named: XCCDF (checklist format), OVAL (vulnerability assessment language), CPE (platform enumeration), CCE (configuration enumeration), CVE, CVSS, and the Asset Reporting Format. Tools such as Qualys implement SCAP; scanning can be ad hoc or continuous. BREACH ATTACK SIMULATION (BAS) is the active counterpart: safely simulates REAL attacks in production, runs frequently/continuously, tries actual attack paths, tests what can really be exploited and whether detection works — in effect continuous red teaming, "pen testing as a subscription," vs SCAP's periodic posture/baseline report. The SCAP-vs-BAS distinction is the lesson's core: automated configuration/posture checking vs active simulated attacks + detection testing. COMPLIANCE CHECKS test the environment against a framework/standard/regulation (example: PCI DSS v4 requiring encryption of payment data — missing encryption = fail). Remediation windows given by severity: critical 7–14 days, high 30 days, medium 90 days, low 120 days (a trailing captioned phrase about longer windows is inconsistent — do not rely on it). SCOPE — what is actually being scanned — is stressed as the most important part of a scan.

---

## Video 12 — Log Review & Analysis
- Duration: 07:19
- Lesson: https://new.my.destcert.com/schedule/lesson/218948fa-6fd1-468d-9f66-de55a51f19a9
- Chapters: Introduction 00:00; Log Reviews / Analysis Overview (relevant, review, errors) 00:51; Looking for? 02:03; Logging & Monitoring Processes 02:21; Log Data Generation 02:54; Limiting Log Sizes 03:13; Better Method for Detecting Breach 04:59; Log Event Time 05:35
- Transcript: 00:13–07:02; 15 blocks / 130 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Log review is in the testing domain because reviewing/monitoring logs tests whether production systems work properly (SIEM detail is deferred to Domain 7). Principles: log only what is RELEVANT — determine relevance from risk management (what are the key risks to the asset, and how would you detect one occurring?) — then review PROACTIVELY (person or system), not only after a breach; a system is essential because large environments produce millions of events per second. Look for: ERRORS (esp. unexpected), MODIFICATIONS (esp. unauthorised), and BREACHES. Endpoint devices (firewalls) generate enormous data with very limited onboard storage, so log size must be limited — the two methods to know: CIRCULAR OVERWRITE (write to a set maximum size, then circle back and overwrite from the top; the file never exceeds the max) vs CLIPPING LEVELS (a threshold: below it, log nothing; above it, log — e.g. ignore <3 failed logins in 30 seconds as mistyping, but log 50 in 30 seconds as a probable brute-force attempt). Exam-style answer given: for DETECTING A BREACH, clipping levels are better — circular overwrite destroys the very data needed to investigate, while clipping limits volume without ever overwriting. LOG EVENT TIME: timestamps must be consistent (same date/clock formats) and ALL systems must share the same time — even a few seconds' skew makes tracing an attacker's path across systems very hard; the fix is NTP (Network Time Protocol) syncing clocks, ultimately to atomic-clock sources.

---

## Video 13 — Operational & Regression Testing
- Duration: 03:47
- Lesson: https://new.my.destcert.com/schedule/lesson/80ea18f1-6d57-4bcd-afb7-ac9385cb181c
- Chapters: Introduction 00:00; Operational Testing 00:17; Real User Monitoring 00:27; Synthetic Transactions 00:51; Regression Testing 02:46; Reporting Testing Results 03:09
- Transcript: 00:15–03:36; 6 blocks / 63 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): REAL USER MONITORING (RUM) = watching log files to see what real users actually do with a system (e.g. which error messages surface, like a 404). SYNTHETIC TRANSACTIONS = transactions created artificially by small scripts/bots performing a function (banking example: separate bots to log in, check a balance, transfer funds) — also used for load/performance testing (e.g. 10,000 synthetic transactions at once, Black Friday style). Exam point flagged: the MOST ACCURATE environment for synthetic transactions is PRODUCTION, because it truly shows how the system reacts under huge load — with the heavy caveat to be extremely careful and test in development/other environments first. REGRESSION TESTING = after a change, verifying not only that the new functionality works but that ALL EXISTING functionality still works — a change broke nothing. Test REPORTING: results must be unambiguous (a clear pass or fail, never a vague "maybe"), with the right detail/metrics for the right audience.

---

## Video 14 — Metrics: KPIs & KRIs
- Duration: 05:05
- Lesson: https://new.my.destcert.com/schedule/lesson/c862115e-0db9-4ca3-b60f-766127de524d
- Chapters: Introduction 00:00; SMART Metrics 00:54; Key Performance & Risk Indicators 01:50; Limitation of Measurement 03:01; How do you decide what metrics to focus on? 03:11; Example areas for metrics 03:52
- Transcript: 00:14–04:49; 10 blocks / 90 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Assessment/testing collects information to give stakeholders assurance — and technical information must be TRANSLATED into language the audience understands; metrics must always be based on the organisation's GOALS AND OBJECTIVES. SMART (Specific, Measurable, Actionable, Relevant, Timely) is a way to think about metrics — explicitly NOT to be memorised for the exam. Useless-metric example: telling a CEO "seven billion hits against our firewall" answers "how secure are we?" with nothing — translate into risk/exposure terms. The two terms to know: KPI (Key Performance Indicator) is BACKWARD-looking (did we achieve the goals we set — do what we said, spend as planned?); KRI (Key Risk Indicator) is FORWARD-looking (risks you worry might occur, measured to see whether they are happening). KGIs (Key Goal Indicators) sit above them, of most interest to the CEO/board. You cannot measure everything; choose by VALUE — involve the goal-level stakeholders, measure what they care about (top-down beats the old bottom-up struggle). Different stakeholders want different things: never quote backup-verification counts to a CEO, but the backup owner wants exactly that.

---

## Video 15 — Test output
- Duration: 04:44
- Lesson: https://new.my.destcert.com/schedule/lesson/96de3ac9-5cc5-4d98-ac17-81bb71f18b8d
- Chapters: Introduction 00:00; Error Handling 00:29; Remediation 01:14; Ethical Disclosure 02:15
- Transcript: 00:15–04:26; 8 blocks / 85 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): (a) AUTOMATED ERROR HANDLING: with many scripts running (example: 100), one script's failure must not stop the rest — a failing script should FAIL GRACEFULLY, the error captured and investigated, the remaining tests continuing; automated testing runs 24×7 and must keep going through errors. (b) REMEDIATION accountability: when testing finds an issue, the SYSTEM OWNER is accountable for getting it fixed — security's role is to advise (report findings, advise how to remediate); the owner usually also pays, and remediation costs money and time. (c) ETHICAL DISCLOSURE — explicitly flagged as NOT on the exam (interesting, keep an eye on it, but don't expect questions): an undefined, "Wild West" area — who must a finder report to, how quickly; researchers torn between reporting to the owner and selling the bug (organisations, nations, companies pay a lot); BUG BOUNTY programmes (Apple/Microsoft/Google; Apple pays up to $1M for certain vulnerabilities) exist to pull reporting toward the company; the minefield case: a researcher reports properly, the company dismisses it, public disclosure would leave users vulnerable.

---

## Video 16 — Third-Party Audit Reports
- Duration: 09:05
- Lesson: https://new.my.destcert.com/schedule/lesson/6829a33e-a057-492e-8df3-7c2b1ce484a3
- Chapters: Introduction 00:00; Different Audit Approaches 00:42; ISAE 3402 / SSAE18 Third-Party Audit reports 03:39; Audit Roles & Responsibilities 07:07
- Transcript: 00:14–08:46; 16 blocks / 164 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Audit approaches: INTERNAL (own auditors, own systems); EXTERNAL (own auditors sent out to audit a provider, e.g. auditing AWS); THIRD-PARTY — the scaling answer: a provider with millions of customers can't host everyone's auditors (even 0.25% would overrun it), so it hires an INDEPENDENT auditor whose report goes to all customers; the name = the three parties (customer, provider, independent auditor), and a provider's own claim about its security should never be taken at face value. Reports are under SSAE 18 (AICPA, US; ISAE 3402 is the international counterpart named in the chapter title). SOC 1 = financial-reporting focus — security professionals "don't really care" about it. SOC 2 = the five TRUST PRINCIPLES (security, availability, confidentiality, processing integrity, privacy) — exactly what security cares about. SOC 3 = a sanitised, summarised SOC 2 for public release — basically a marketing tool, not enough detail for assurance. TYPE 1 = DESIGN at a POINT IN TIME (a paper exercise — policies/procedures as they stand on the day; shows nothing about operating effectiveness; "not that helpful"). TYPE 2 = design PLUS OPERATING EFFECTIVENESS over a PERIOD (typically a year) — e.g. change management: check the design, then sample the whole year's population of changes and test each for initiation, impact assessment, approvals, testing, back-out plans, regression testing and documentation. Conclusion: what security professionals want is a SOC 2 TYPE 2. Audit roles (flagged as very important to remember): SENIOR MANAGEMENT — tone from the top, support and funding; AUDIT COMMITTEE — stakeholders providing input, keeping the function aimed at the right things/regulations; SECURITY OFFICER — advises on what the audit should cover and how to read results; COMPLIANCE MANAGER — makes sure the compliance function is created, staffed and running; INTERNAL AUDITORS — own auditors on own processes; EXTERNAL AUDITORS — brought in from outside for an independent, unbiased view. CONFIRMED by this batch: video 16 is the LAST main lesson video in Domain 6 (16 total); next items are flashcards, the 50-question assessment, results, then the three MindMaps.

---

# Coverage appendix — Domain 6 videos vs drill-list topics

All 16 main lesson videos pulled and confirmed (16/16; video 16 is the last, followed by flashcards, the assessment, results, then the three MindMaps). All 16 transcripts were STABLE across three loads each — no alternate versions anywhere in Domain 6; only 1-second duration-label differences on a few videos and a truncated closing block in V2's panel. All entries are metadata + content summaries, not verbatim reproductions.

**19 of 19 Domain 6 drill topics covered:**
- 6.1.1 Intro to Testing — V1 (assurance pillar; security functionality, not "non-functional")
- 6.1.2 Validation & Verification — V1 (right product vs product right; three Cs)
- 6.1.3 Effort to Invest in Testing — V1 (driven by system value)
- 6.1.4 Location of Assessment — V2 (on-premise / cloud / hybrid)
- 6.2.1 Testing Overview — V3 (stages: unit, interface, integration, system; security from the earliest stage), V4
- 6.2.2 Testing Techniques — V4 (manual/automated, static/dynamic, black/white box, positive/negative/misuse, equivalence partitioning, boundary values, coverage), V5 (mutation vs generation fuzzing), V6 (SAST/DAST/IAST), V7 (decision tables, state-based analysis)
- 6.2.3 Vulnerability Assessment & Penetration Testing — V8 (assessment finds/grades; pen test exploits; typical process)
- 6.2.4 Red, Blue and Purple Teams — V9 (purple = collaboration, not a separate team)
- 6.2.5 Vulnerability & Pen Testing Techniques — V10 (internal/external × black/grey/white box, blind vs double-blind, credentialed vs uncredentialed scans, war dialing/driving, banner grabbing, fingerprinting, CVE/CVSS, false negatives far worse)
- 6.2.6 SCAP & Breach Attack Simulation — V11 (SCAP components; BAS = continuous active simulation; compliance checks; remediation windows)
- 6.2.7 Log Review & Analysis — V12 (relevance from risk; errors/modifications/breaches; NTP time sync)
- 6.2.8 Limiting Log Sizes — V12 (video-only topic in the guide; circular overwrite vs clipping levels — clipping better for breach detection)
- 6.2.9 Operational testing — Synthetic transactions & RUM — V13 (production = most accurate environment for synthetic transactions)
- 6.2.10 Regression Testing — V13
- 6.3.1 Key Risk & Performance Indicators — V14 (KPI backward-looking, KRI forward-looking; SMART not to be memorised)
- 6.4.1 Test Output Importance — V15 (graceful failure; system owner accountable for remediation; ethical disclosure flagged NOT on the exam), V13 (unambiguous pass/fail reporting)
- 6.5.1 Audit Approaches — V16 (internal / external / third-party), V1 (testing strategies)
- 6.5.2 SOC Reports — V16 (SOC 1/2/3; Type 1 vs Type 2; SOC 2 Type 2 is the one to want)
- 6.5.3 Audit Roles & Responsibilities — V16 (senior management, audit committee, security officer, compliance manager, internal/external auditors)

---

# MindMap videos — added 2026-11-13

The domain's MindMap videos: the instructor's condensed maps — connections and emphasis. Metadata + content summaries, not verbatim reproductions. All stable across three loads; all have full transcripts. Domain 6 has exactly 3 MindMaps (the "MindMaps:" prefix is the schedule's section label, not part of the titles).

## MindMap 1 — Security Assessment and Testing
- Duration: 11:46
- Lesson: https://new.my.destcert.com/schedule/lesson/1f707eb0-bbb5-4a96-8a32-8519be3a1eb3
- Chapters: 55 (Security Assessment and Testing; Validation; Verification; Rigour; Testing a System — Unit/Interface/Integration/System; Testing Techniques; Methods & Tools — Manual/Automated/Runtime/Static/Dynamic/Fuzz (Mutation/Generation); Access to Code — White/Black; Positive; Negative; Misuse; Decision table analysis; State-based analysis; Efficiency; Boundary Value Analysis; Equivalence Partitioning; Operational; Real User Monitoring; Synthetic Performance Monitoring; Regression Testing; Testers/Assessors — Internal/External/Third-Party; SOC 1; SOC 2; Type 1; Type 2; SOC 3; Roles — Executive Management/Audit Committee/Security Officer/Compliance Manager/Internal Auditors/External Auditors; Metrics; Focus; KPIs; KRIs)
- Transcript: 00:00–11:33; 28 blocks / 205 phrase lines (stable)
- Content summary: The domain framed as making sure security requirements and controls are defined, tested and actually working — with security involved from the VERY START of a system's life (explicit exam point: get involved as early as possible — "if 'the dawn of time' is an option, choose it"). VALIDATION (agreeing business requirements with stakeholders before building) vs VERIFICATION (testing during the build that controls were designed in properly). Testing RIGOUR scales with the system's value and the confidence needed. Test layers build up: UNIT → INTERFACE → INTEGRATION → SYSTEM. Techniques are a mix-and-match toolkit: manual vs automated; STATIC (code not running) vs DYNAMIC (running system); WHITE-box (source access) vs BLACK-box (internals hidden); FUZZ testing (chaotic unexpected input) — MUTATION fuzzing is blind (no understanding of input structure), GENERATION fuzzing builds new chaotic input from a basic understanding of the expected structure. POSITIVE testing (does what it should) vs NEGATIVE (handles expected errors gracefully) vs MISUSE (deliberate attacker-style abuse). Decision-table analysis (input combinations → expected behaviour), state-based analysis (stateful interfaces/protocols), BOUNDARY VALUE ANALYSIS (test at the edges where behaviour changes) and EQUIVALENCE PARTITIONING (group inputs that should behave the same, test each group). Operational: REAL USER monitoring vs SYNTHETIC monitoring (scripted transactions/bots); REGRESSION testing after changes. SOC reports: SOC 1 = financial reporting (less interesting to security); SOC 2 = the five trust principles (security, availability, confidentiality, processing integrity, privacy); TYPE 1 = design at a point in time vs TYPE 2 = design + operating effectiveness over a period (~a year, sampled) — SOC 2 TYPE 2 is the combination to want; SOC 3 = a sanitised public summary of SOC 2. Roles: executive management (tone/funding), audit committee (oversight), security officer (risk advice), compliance manager (programme), internal auditors (assurance), external auditors (independent view). Metrics tied to business objectives: KPIs = backward-looking performance vs targets; KRIs = forward-looking exposure to operational risk.

## MindMap 2 — Identifying Vulnerabilities
- Duration: 07:44
- Lesson: https://new.my.destcert.com/schedule/lesson/cdb415d1-3b7c-4967-baf8-b21f841d747e
- Chapters: 29 (Identifying Vulnerabilities; Vulnerability Assessment; Penetration Testing; Process; Reconnaissance; Enumeration; Vulnerability Analysis; Execution; Document Findings; Testing Techniques; Perspective — Internal/External; Approach — Blind/Double-blind; Knowledge — Zero (black)/Partial (gray)/Full (white); Types of Scans; Credentialed/Authenticated; Uncredentialed/Unauthenticated; Banner grabbing & Fingerprinting; Interpreting results; CVE; CVSS; SCAP; False positive vs False negative)
- Transcript: 00:00–07:34; 16 blocks / 142 phrase lines (stable)
- Content summary: Every system has vulnerabilities. VULNERABILITY ASSESSMENT vs PENETRATION TEST: both start by identifying, classifying and prioritising weaknesses — the assessment then goes straight to REPORTING, while the pen test goes on to EXPLOIT a weakness to prove it real (removing false positives). Assessment = faster, more automated, more false positives; pen test = slower, more manual, clearer picture, greater disruption risk. The five-step process: RECONNAISSANCE (passive, public sources — job postings, LinkedIn, DNS; undetectable) → ENUMERATION (active, detectable; walking address ranges/ports for live systems and services) → VULNERABILITY ANALYSIS (exact versions, exploitable weaknesses) → EXECUTION (pen test only — attempting the break-in) → DOCUMENT FINDINGS (impact + prioritisation, tailored to the audience). PERSPECTIVE: internal (insider's seat) vs external (outside the firewall). APPROACH: BLIND (tester given very little) vs DOUBLE-BLIND (the SOC/defenders aren't told either — detection and response get tested too). KNOWLEDGE is a separate axis: ZERO/black (no inside information, public material + deduction — same as blind), PARTIAL/gray (some knowledge, e.g. an ordinary/elevated account + basic architecture — more efficient), FULL/white, a.k.a. open/clear-box (full access incl. source code, credentials, architecture docs — "listen really carefully" emphasis). Scans: CREDENTIALED/authenticated (scanner logs in — exact configuration, fewer false positives, compliance baselines) vs UNCREDENTIALED (simulates an external attacker). Exact versions matter: BANNER GRABBING provokes an error that reveals a version (systems should be configured not to leak it) vs FINGERPRINTING (subtler — infers versions from packet structure). Results are interpreted via CVE (unique public ID per vulnerability), CVSS (0–10 severity score) and SCAP (interoperable specs automating vulnerability management and compliance checking). FALSE POSITIVE (chasing a weakness that isn't there — wasted time) vs FALSE NEGATIVE (a real weakness the tools miss — FAR WORSE, the organisation stays blind to it).

## MindMap 3 — Log Review & Analysis (LAST Domain 6 MindMap — 3 total)
- Duration: 06:01
- Lesson: https://new.my.destcert.com/schedule/lesson/879ce989-8a8e-406b-937d-de79d49e31ac
- Chapters: 20 (Log Review & Analysis; Monitor for; Errors; Modification; Breaches; SIEM; Generation; Limiting log file size; Circular Overwrite; Clipping Levels; Time Stamps; Consistent; NTP; Transmission; Collection/Aggregation; Normalization; Analysis; Retention; Disposal; Continuous Monitoring)
- Transcript: 00:00–05:50; 13 blocks / 113 phrase lines (stable)
- Content summary: Logging/monitoring as a central part of assessment. Log sources are everywhere (network devices, IDS/IPS, servers, endpoints, OSs, applications, anti-malware), so log SELECTIVELY (an avalanche otherwise) and review as close to REAL TIME as possible — not discovering a breach months later. Monitor for three things: ERRORS/anomalies (e.g. a flood of 404s), unauthorised MODIFICATIONS (attackers often patch the hole they used after installing a backdoor — unexplained patching can itself signal a breach), and BREACHES (crypto-mining, exfiltration, ransomware). That volume needs automation: SIEM. Log-file size on storage-poor devices is limited two ways: CIRCULAR OVERWRITE (cap the size, then wrap and overwrite from the top) vs CLIPPING LEVELS (a threshold — log nothing below it, start above it; e.g. ignore 1–2 failed logins as typos, care about 10 in quick succession; suggested threshold: 3 failed logins within 60 seconds). TIMESTAMPS must be in a consistent format and all clocks SYNCHRONISED via NTP, or cross-system correlation and attacker tracing break down. The SIEM PIPELINE in order: TRANSMISSION (each event sent in real time) → COLLECTION/AGGREGATION (one central system) → NORMALIZATION (disparate data cleaned into comparable formats) → ANALYSIS (correlation, statistical models, rules). SIEMs also handle RETENTION (long-term storage for longitudinal analysis and contractual/regulatory requirements) and secure DISPOSAL when retention ends. Closes with CONTINUOUS MONITORING (CSM): identify all systems, identify each one's risks, apply appropriate controls, and continuously monitor those controls' effectiveness.
