# Vernacular Lesson Translator – Phase 3 PoC Demo Prototype (v01)

**Project:** AI-Powered Vernacular Pedagogy and Real-Time Translation Tool for Mother Tongue-Based Primary Education
**Project ID:** P-2025-29-CD-058-AY26-27 · **Batch:** 2025–29 · **Vertical:** CD – Cloud and DevOps
**Team:** Apex · Leader: Lokesh · Members: Kishore Kumar R, Kishore P, Kishore M, Maathavan H
**Mentor:** K N Nandhakumar
**Phase:** AY 2026–27 Phase 3 – Proof of Concept · **Version:** v01

## Status (read first)
This is an **illustrative demo prototype**. It uses a small rule-based phrase lookup, **not the AI translation model**. Its outputs are **not measured PoC evidence**.
- Tests T1 (meaning accuracy), T2 (curriculum fidelity) and T3 (time per page): **NOT TESTED**.
- Evidence IDs P3-E01 to P3-E03: **not available**.
- Component status: web page = BUILT (demo); AI translation pipeline = [BUILT / REUSED / MOCKED / PLANNED – confirm]; teacher review = demo buttons only.
- The example language is Tamil. The five sample translations are unverified by a bilingual reviewer.

## PoC question
Can an AI lesson-translation pipeline reach ≥ 85% meaning accuracy against teacher translation, within a grade-level readability limit?
(Proposed criteria: T1 ≥ 85% · T2 ≥ 95% with zero unsafe errors · T3 ≥ 50% faster than manual.)

## What the demo shows
Workflow: English lesson sentence → translate + adapt → mother-tongue text → teacher review, with manual translation as the fallback.
- Five sample Grade 1–3 sentences plus two boundary cases.
- Word-count check against a limit of 8 words (a demo stand-in for readability).
- Idioms and sentences with numbers/units are flagged for manual translation instead of being translated.
- A run log. Its "ms" column includes a fixed 1.1 s animation delay and is **not** a performance measurement.

## Files
| File | Purpose |
|---|---|
| `index.html` | Self-contained demo page (no server, no internet, no API keys) |
| `P-2025-29-CD-058-AY26-27_P3_v01_prototype_demo.mp4` | Screen recording of the demo, about 47 s, 1920×1080, 30 fps, captions only |

## How to replay
1. Download `index.html` into any folder.
2. Open it in Chrome, Edge or Firefox. A Tamil-capable font is needed; most systems have one.
3. Pick a sample sentence from the dropdown (or type one), then click **Translate**.
4. Watch the pipeline stages light up, then read the output and the word-count tag.
5. Click **Approve**, **Edit** or **Send to manual translation** (demo actions only; nothing is saved).
6. Try "It is raining cats and dogs." (idiom) and "The tree is 3.5 metres tall." (number) to see the fallback.

## Known limitations
- The lookup covers only the five sample sentences. Anything else shows "Not in lookup".
- The idiom and number detection are simple keyword/digit checks.
- It has no AI model, speech, live classroom use, user accounts or data storage.
- Not verified: accuracy, curriculum fidelity, speed, classroom use, learning impact.

## Safety and data
Non-sensitive sample text only. No child data, no personal data, no credentials.

## Next actions
| Action | Owner | Date | Evidence / output |
|---|---|---|---|
| Record a real run of the actual AI pipeline | [name] | [date] | Screen recording |
| Run T1–T3 on the 30-sentence set with the teacher reference | [name] | [date] | Results + P3-E01 to E03 |
| Bilingual reviewer checks translations | [name] | [date] | Review note |

*Team-reported technical finding, not institutional approval.*
