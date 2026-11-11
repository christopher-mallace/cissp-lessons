# CISSP Master Learning Profile

Last updated: 2026-11-11 00:45 ET
Version marker: V6-DRILL-20261111
Source: Quantum Exams, "CISSP: 10 Question Quiz" — analyzed by Darla
Exam: Mon Dec 21, 2026, 10:00 AM ET

## Overall
- Attempts: 15 (Oct 3 – Nov 5, 2026), all finished
- Questions: 150 — Correct: 78 (52.0%) — Missed: 72
- Best attempts: 8/10 (Oct 25, Oct 28). Most recent Nov 5: 2/10 and 4/10.
- Quantum does not label domains. Domains are inferred by Darla from topic/feedback, mapped to the DestCert Review Guide domains.

## Per-domain results (attempted / correct / % / missed)
- Domain 1 Security and Risk Management: 43 / 17 / 39.5% / 26 missed
- Domain 2 Asset Security: 9 / 5 / 55.6% / 4 missed
- Domain 3 Security Architecture and Engineering: 32 / 18 / 56.3% / 14 missed
- Domain 4 Communication and Network Security: 16 / 12 / 75.0% / 4 missed
- Domain 5 Identity and Access Management: 12 / 8 / 66.7% / 4 missed
- Domain 6 Security Assessment and Testing: 11 / 5 / 45.5% / 6 missed
- Domain 7 Security Operations: 13 / 8 / 61.5% / 5 missed
- Domain 8 Software Development Security: 14 / 5 / 35.7% / 9 missed

## Focus ranking — descending by misses
1. Domain 1 (26) — BCP/DRP/BIA cluster first: BIA purpose & business process owners, BCP vs DRP, MTD, recovery sites by risk, hot/warm site vs UPS, BCP testing. Due care vs due diligence (missed 3x). Risk order: NIST 800-30, qualitative matrix steps, control selection by risk capacity. Governance, RMF order, CSA STAR Level 2, separation of duties, mandatory vacation, HA/SLA first, power fault = short-term loss, CIA Integrity.
2. Domain 3 (14) — Crypto distinctions: ECC, ECDSA vs ECDH/DH, link vs end-to-end encryption, one-time pad, PKI. Side-channel vs covert channel (missed 2x). ACID, polyinstantiation, fire detection, ICS/SCADA availability, IoT segmentation, data remanence.
3. Domain 8 (9) — Lowest % correct. SDLC phases/models, STRIDE, functional vs non-functional requirements, path traversal, DOM XSS vs CSRF, AI training data protection.
4. Domain 6 (6) — Vulnerability workflow steps, continuous monitoring, audit types, virtualized-image scanning, legacy apps with no access controls.
5. Domain 7 (5) — Full backup = fastest restore, RAID is not backup, eDiscovery Review vs Analysis / Information Governance, ransomware remediation.
6. Domain 2 (4) — Owner vs Steward/Custodian/Processor, classification in Storage stage, crypto-erase disposal.
7. Domain 5 (4) — Iris / Type 3 biometrics, IAM lifecycle Provision step, authentication-device confidentiality.
8. Domain 4 (4) — Strongest domain. IPsec AH/NAT, VoIP eavesdropping, bastion host, L2TP/IPsec layer.

## Error patterns to train (Rain: classify every new miss this way)
- Knowledge gap — did not know the concept
- Interpretation — misread / confused similar terms
- Application — knew it, applied it wrong
- Managerial judgment — chose the technical answer over the risk/policy answer
- Distinction failure — could not separate two competing choices

## Source questions — Missed Questions Appendix (added 2026-11-09)
The actual questions behind every cluster in this profile are in the companion file `Missed_Questions_Appendix.md` in this repo (raw: https://raw.githubusercontent.com/christopher-mallace/cissp-lessons/main/Missed_Questions_Appendix.md). Each missed question has a stable ID (MQ-01 … MQ-72) with the attempt/question number, a summary of what was asked, what Christopher picked, the correct answer, and the feedback point.
**Rule for Rain:** fetch the appendix together with this profile. At the top of every lesson, cite the MQ IDs that spurred it. When Christopher asks which question(s) he got wrong behind a lesson or priority, answer from the appendix — do not say you cannot identify them.

## Need-to-Know Drill List (added 2026-11-11)
At Christopher's direction on 2026-11-11, Darla extracted from the DestCert Review Guides for all 8 domains everything the guides tell him he must know / memorize — every Core Concepts box and every blue side call-out, with the full answer from the guide (steps in order, models, definitions, formulas, values). That companion file is `DestCert_Need_To_Know_Drill_List.md` in this repo (raw: https://raw.githubusercontent.com/christopher-mallace/cissp-lessons/main/DestCert_Need_To_Know_Drill_List.md). Coverage: 263 topics — D1: 34, D2: 16, D3: 71, D4: 38, D5: 31, D6: 19, D7: 36, D8: 18. Topics marked video-only in that file have no Guidebook, so there is nothing to drill from the guide for them; a few items are flagged in-file where the guide extract did not give full detail — do not invent answers for those.

**Rule for Rain — drilling:** fetch the drill list together with this profile and the Missed Questions Appendix. Drill Christopher on these need-to-knows and ensure he actually understands them, not just that he has seen them:
- Ask him to produce the list / order / definitions / formula unaided first (e.g. the Common Criteria steps and EAL levels in 3.2.7, the RMF steps in 1.9.11, RPO/RTO/WRT/MTD in 7.11.4) — do not show him the answer before he attempts it.
- Then test application, not only recall: follow with a CISSP-style scenario at equal-or-harder difficulty, using the Lesson standard below (qualifiers MOST/BEST/FIRST/PRIMARY, plausible distractors, technician-vs-manager traps, process order), and grade his reasoning, not just his pick.
- An item counts as understood only when he can both reproduce it unaided and apply it correctly in a scenario. If he misses either, coach it, re-drill it in that session, and mark it still weak in your reply so Darla can record it.
- Work domain by domain, prioritising his weakest areas from the focus ranking above, and report at the end of each drill session which section IDs (e.g. 1.9.11, 3.2.7) he mastered and which are still weak. Darla remains the sole writer to this repo and will record those outcomes in the Mastery log.
- Drilling under this section is a drill track Christopher requested on 2026-11-11; it is not a new numbered lesson for Pacing Rule 6 below, but Lesson 1's pending final judgment scenario remains outstanding and should not be silently dropped — tell Christopher how you are sequencing the two if there is a conflict.

## Next three instructional priorities
1. Domain 1: BCP/BIA/DR decision order — source questions: MQ-12, MQ-27, MQ-34, MQ-35, MQ-39, MQ-41, MQ-45, MQ-46, MQ-51, MQ-59, MQ-63
2. Domain 1: Due care vs due diligence — source questions: MQ-11, MQ-24, MQ-36 (risk order: MQ-19, MQ-49)
3. Domain 3: Side-channel vs covert channel + crypto distinctions — source questions: MQ-04, MQ-18, MQ-07, MQ-20, MQ-37, MQ-50, MQ-72

## Lesson standard — DestCert answering strategy (standing requirement)
Added 2026-11-05 at Christopher's direction; accepted by Rain as a standing instructional specification. This applies to every lesson Rain creates from this file, including any scheduled-task run.

1. Coach Christopher, in every lesson, to apply DestCert's strategy for answering CISSP exam questions — and evaluate whether he used that strategy, not just whether his final answer was right.
2. Every practice question / judgment scenario must be at equal difficulty to the real CISSP exam, or harder. No easier warm-up sets.
3. Build questions the way CISSP asks them: loaded/tricky wording, qualifiers such as MOST / BEST / FIRST / PRIMARY, two or more plausible answers, a technician answer that looks right vs. the manager / risk-based answer CISSP wants, and correct process order mattering more than raw facts.
4. Christopher must show the strategy in his answers: identify the qualifier, eliminate distractors step by step, and name the traps before choosing.
5. A correct answer reached without using the strategy counts as incomplete — he redoes the reasoning. A wrong answer with sound strategy-based reasoning gets coached step by step, not just marked wrong.
6. Pacing rule: if a delivered lesson is not yet completed and recorded in the Mastery log below, do not create a new lesson — re-present / remind on the incomplete lesson only. Lessons do not pile up.

## Lessons delivered
- 2026-11-05 — Lesson 1: Domain 1, BCP/BIA/DR decision order (Rain, in the "Recommend Shared Study Method" ChatGPT chat; generated manually ahead of the first scheduled run at Christopher's request)

## Mastery log
- Lesson 1 (Domain 1: BCP/BIA/DR decision order) — DELIVERED 2026-11-05, completion PENDING: Christopher has not yet answered the final judgment scenario, so under Rule 6 the next run continues this lesson instead of starting a new one.
