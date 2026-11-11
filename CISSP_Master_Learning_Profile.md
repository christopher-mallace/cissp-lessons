# CISSP Master Learning Profile

Last updated: 2026-11-11 01:05 ET
Version marker: V8-SEPARATE-20261111
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

## Separation note — DestCert-based track is a DIFFERENT file (corrected 2026-11-11)
This profile is the **Quantum-based** track only: its lessons are driven by Christopher's missed Quantum questions and the focus ranking above.
DestCert-based drilling is a **separate track** with its own profile: `DestCert_Based_Profile.md` in this repo (raw: https://raw.githubusercontent.com/christopher-mallace/cissp-lessons/main/DestCert_Based_Profile.md), based solely on the DestCert Review Guides (`DestCert_Need_To_Know_Drill_List.md`, 263 topics) in the guides' own order.
**Rule for Rain:** do not merge the two tracks. Do not use this profile, its focus ranking, or the Missed Questions Appendix to pick or order DestCert drill items, and do not record DestCert drill outcomes in this file's Mastery log — they belong in `DestCert_Based_Profile.md`. For a Quantum-track lesson, fetch this profile + the appendix; for a DestCert drill session, fetch the DestCert profile + the drill list.

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
- Lesson 1 (Domain 1: BCP/BIA/DR decision order) — COMPLETED 2026-11-10 (recorded by Darla 2026-11-11 after a read-only verification of Rain's chat, reconciling Rain's Nov 11 report). Christopher worked the lesson in sections: Section 1 check answered Nov 6; Diagnostic Question 1 (shared authentication service, three RTOs) answered C on Nov 9 with reasoning evaluated as demonstrated; Section 2 (Recovery Objectives) Mastered Nov 9; Section 3 (Recovery Sites) Mastered Nov 9; Section 4 (BCP Testing) Mastered Nov 10. Final CISSP Assessment Nov 10 evening (acquisition scenario, FIRST action): Christopher answered C (engage business process owners to reassess business impacts, dependencies, and recovery requirements) and gave reasoning for C over D, which Rain evaluated as correct. Rain's assessment: all six competencies Demonstrated — business criticality vs technical dependencies; MTD, RTO and RPO; recovery-site selection; continuity testing; business-first decision sequencing; DestCert reasoning — "Lesson 1 is complete from my instructional assessment." Note: the original Nov 5 Part 8 scenario was superseded by the section-by-section delivery at Christopher's request; it is not the final assessment. Under Rule 6, scheduled lessons may now advance past Lesson 1.
