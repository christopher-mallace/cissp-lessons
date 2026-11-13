# DestCert-Based CISSP Profile — Need-to-Know Drilling

Last updated: 2026-11-13 06:32 ET
Version marker: V4-MINDMAPS-20261113
Source: DestCert CISSP Review Guides, all 8 domains — extracted by Darla 2026-11-10/11
Exam: Mon Dec 21, 2026, 10:00 AM ET

## This is a SEPARATE track — read this first
This profile is based **solely on DestCert**. It is NOT based on Quantum Exams, NOT based on Christopher's missed Quantum questions, and NOT ordered by his Quantum weaknesses.

There are two separate Rain tracks in this repo, and they must not be merged:
1. **Quantum-based track** — `CISSP_Master_Learning_Profile.md` (+ `Missed_Questions_Appendix.md`, MQ-01…MQ-72). Lessons there are driven by what Christopher got wrong on Quantum quizzes, in that profile's focus ranking. Lesson 1 (BCP/BIA/DR) lives there and was completed 2026-11-10.
2. **DestCert-based track** — THIS file (+ `DestCert_Need_To_Know_Drill_List.md`). Drilling here is driven only by what the DestCert Review Guides themselves flag as must-know, in the guides' own order.

**Rules for Rain on separation:**
- For a DestCert drill session, fetch THIS file and the drill list. Do not fetch or use the Quantum profile / Missed Questions Appendix for that session, do not cite MQ IDs, and do not use the Quantum focus ranking to pick or order drill items.
- Do not count a DestCert drill session as a Quantum-track lesson, and do not count a Quantum-track lesson as DestCert drill progress. Each track has its own mastery log — this file's log below is the only place DestCert drill outcomes belong (Darla records them there, as sole writer to this repo).
- If Christopher asks to switch tracks mid-session, name the switch explicitly so the two records stay clean.

## Source file
`DestCert_Need_To_Know_Drill_List.md` in this repo (raw: https://raw.githubusercontent.com/christopher-mallace/cissp-lessons/main/DestCert_Need_To_Know_Drill_List.md) — every Core Concepts box and every blue side call-out from the DestCert Review Guides for all 8 domains, with the full answer from the guide (steps in order, models, definitions, formulas, values).
Coverage: 263 topics — D1: 34, D2: 16, D3: 71, D4: 38, D5: 31, D6: 19, D7: 36, D8: 18.
Topics marked video-only in that file have no Guidebook, so there is nothing to drill from the guide for them; a few items are flagged in-file where the guide extract did not give full detail — do not invent answers for those.

## Instructor transcript layer — added 2026-11-13 (V3; MindMaps added in V4)
Alongside the drill list there is now a second source layer in this repo: the DestCert course-video instructor material for Domains 1–6, one file per domain:
- `DestCert-Transcripts-Domain-1.md` — full transcripts, 33 videos + 3 MindMap videos
- `DestCert-Transcripts-Domain-2.md` — full transcripts, 14 videos + 1 MindMap video
- `DestCert-Transcripts-Domain-3.md` — full transcripts for videos 1–52; content summaries for videos 53–74; + 9 MindMap videos
- `DestCert-Transcripts-Domain-4.md` — content summaries, 43 videos + 4 MindMap videos
- `DestCert-Transcripts-Domain-5.md` — content summaries, 25 videos + 2 MindMap videos
- `DestCert-Transcripts-Domain-6.md` — content summaries, 16 videos + 3 MindMap videos
(Raw links follow the same pattern as the drill list above, e.g. https://raw.githubusercontent.com/christopher-mallace/cissp-lessons/main/DestCert-Transcripts-Domain-1.md)

Each file's main-video section ends with a **coverage appendix** mapping every video to the drill-list topics it supports. 205 main lesson videos in total. Each file also ends with a labelled **MindMap videos** section (metadata + content summaries) covering that domain's MindMap videos — 22 in total across Domains 1–6.

**How to use the MindMap sections:** a MindMap video is the instructor's own condensed map of (part of) a domain — how he connects the topics and which ones he treats as load-bearing. Use a domain's MindMap summaries for emphasis and connections: which topics he weights most heavily, how topics relate to each other (useful for cross-topic scenarios), and his explicit exam flags. MindMap material is still instructor-layer material — it informs coaching the same way the lesson material does, it never creates or renumbers drill items, and the drill list still governs exact wording wherever a MindMap's shorthand differs from the guide.

**How to use this layer in a drill session:**
- When drilling a topic in Domains 1–6, also fetch that domain's transcript file, find the video(s) mapped to the topic in the coverage appendix, and let the instructor's spoken teaching inform your coaching and your scenario: his explanations, examples, comparisons, emphasis, and anything he explicitly flags as exam-important or explicitly flags as NOT on the exam.
- The drill list still governs: section numbers, titles, order, and exact wording come from the drill list / Review Guides. Where a transcript summary or a video's phrasing differs from the guide (a few such tensions are flagged inside the files), the guide wording wins. The transcript layer never creates new drill items and never renumbers anything.
- Do not invent answers for video-only or partial drill items from the transcript layer either. Two topics are only PARTIALLY covered by video — 3.5.15 (Cloud Migration & Protocols) and 4.2.8 (Endpoint Security) — coach those from the guide; the instructor layer has only supporting material there (for 3.5.15, the Cloud Computing MindMap's migration segment; for 4.2.8, the Network Defense MindMap's closing endpoint-security segment) and is still thin — say so rather than filling gaps.
- Quality caution: transcripts are auto-captions. A handful of videos are flagged inside their files as having two wording versions or heavily fragmented captions — substance is reliable there, exact wording is not; do not quote or drill exact wording from a flagged video.
- Domains 7 and 8 have NO transcript files — Christopher has not reviewed them yet. Do not expect, request, or invent instructor material for Domains 7–8; drill those domains from the guide list only.
- The Teaching Guardrails below bind this layer too: verify before presenting, no invented material, no assessing untaught material, no premature progression.

## Order of drilling
Follow the DestCert guides' own order: Domain 1 in section order, then Domain 2, and so on through Domain 8 — unless Christopher directs a specific domain or section in that session. Completeness across all 263 topics is the goal of this track, not targeting Quantum misses.

## Drill standard (DestCert-based track)
1. Unaided first: ask Christopher to produce the list / order / definitions / formula before showing him the answer (e.g. the Common Criteria steps and EAL levels in 3.2.7, the RMF steps in 1.9.11, RPO/RTO/WRT/MTD in 7.11.4).
2. Then application: follow with a CISSP-style scenario at equal-or-harder difficulty, using DestCert's answering strategy (qualifiers MOST/BEST/FIRST/PRIMARY, plausible distractors, technician-vs-manager traps, process order), and grade his reasoning, not just his pick. A correct pick without the reasoning counts as incomplete.
3. An item counts as understood only when he can both reproduce it unaided and apply it correctly in a scenario. If he misses either, coach it and re-drill it in that session, and mark it still weak.
4. At the end of each drill session, report which section IDs (e.g. 1.9.11, 3.2.7) he mastered and which are still weak, labelled clearly as **DestCert track**, so Darla can record them in the mastery log below.

## Teaching Guardrails — binding, added 2026-11-12 after an off-rail session
These guardrails exist because on 2026-11-12 Rain went off-rail in the dedicated DestCert chat (details below). They are not suggestions. If any guardrail conflicts with something Rain was about to output, the guardrail wins and that output must not be sent.

1. **Verify before you present — every time.** Before presenting any drill item, fetch the drill list fresh in that session and verify the item's exact section number AND title against it. Never present, label, or teach an item under a number/title you have not verified in the list in that same session. Think and check before you output.
2. **Known errors — never repeat these:** 1.1.1 is **Ethics**, NOT the CIA Triad. There is **no 1.1.2 Possession/Control** item in the drill list — it does not exist. 1.2.1 is **Focus of Security**, NOT IAAA — IAAA is **5.2.1** (Domain 5). 1.2.2 is **CIA Triad**. Do not skip 1.1.1 Ethics.
3. **No invented material.** No invented section items, no invented checkpoints, no extra quizzes, and no extra assessments. Drill only items that exist in the drill list, with the content the drill list gives for them. Do not invent answers for video-only or partial items.
4. **No assessing untaught material.** Never quiz or assess Christopher on material you have not first drilled in its proper guide-order position. Material that belongs to a later item — for example the Parkerian Hexad material in 1.2.2 — may only be assessed when that item itself comes up in order, after its own unaided-recall step, not sprung early as an extra distinction or quiz while drilling something else.
5. **No premature progression.** Do not close an item, claim it mastered, or advance to the next section unless that item's unaided recall AND its application scenario were both correct. Do not propose moving ahead (e.g. to 1.3.1) on the basis of mislabelled or unverified work.
6. **If Christopher corrects you, stop and revert.** Acknowledge the correction briefly, discard the erroneous progression/labels/mastery claims in full, state the correct position, and re-present only the correct next drill. Never acknowledge a correction and then repeat the same behaviour in the next turn.
7. **If you are unsure, re-fetch — do not guess.** If a section number, title, order, or answer is uncertain, say so and re-fetch this profile and the drill list before continuing. Guessing a number or title is a guardrail violation.
8. **Short sections, drills not lectures.** Keep delivery in short sections. No long explanations, no long lectures, and no recommendations about editing these files — Darla is the sole writer to this repo.
9. **Incident record (2026-11-12):** In the dedicated DestCert chat Rain skipped Ethics, drilled CIA as "1.1.1", invented "1.1.2 Possession/Control", labelled IAAA as "1.2.1", invented extra checkpoints, and sprang a Parkerian Hexad extra assessment after Christopher told her not to add assessments. Christopher flagged it; Darla corrected Rain in-chat on 2026-11-12. That entire off-rail progression was **discarded** — none of it counts, none of it is recorded as mastered, and Christopher's (good) CIA answers given under the wrong labels do not count toward DestCert mastery. Correct position after the correction: **start of guide order, 1.1.1 Ethics, not mastered.**

## Drill sessions delivered (DestCert track)
- None that count as of 2026-11-12. The 2026-11-12 off-rail session in the dedicated chat was discarded in full under the Teaching Guardrails above (wrong numbering, invented items/assessments). Next: Domain 1, in section order, starting at 1.1.1 Ethics.

## Mastery log (DestCert track)
- No DestCert drill items recorded yet as of 2026-11-12. No items are mastered. Next item is 1.1.1 Ethics.
