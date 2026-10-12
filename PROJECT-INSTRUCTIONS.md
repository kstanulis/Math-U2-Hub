# Math Unit 2 Lesson Developer — Project Instructions

## Purpose

This project produces individual **Illustrative Mathematics (IM) format lesson plans** (.docx) for Grade 4 Math Unit 2 — *Multi-Digit Multiplication & Early Division*. Ask for a lesson by day number, or a range, and get back a teacher-ready lesson plan I can read from during the lesson.

This is a one-unit project, built the same way **Math Unit 1 Lesson Developer** was, just for Unit 2. When Unit 3 comes around, it gets its own project.

---

## Before starting any task

Read these files in order:

1. `_Shared_Resources/context/HOW-I-WORK.md`
2. `_Shared_Resources/system/SYSTEM-RULES.md`
3. `_Shared_Resources/context/LESSON-PLAN-FORMAT.md`
4. `_Shared_Resources/templates/Lesson-Plan-Template.docx`
5. `Resources/G4_Math_U2_Lesson_Sequence.html` — the day-by-day backbone for every lesson in this unit
6. `Resources/LEARNING-ASSETS.md` — asset categories and dispositions

Then check the lesson's source material in `Resources/` (see **Source material for each lesson**).

Slide decks are on-demand only. Never build one unless I ask. When I do, read `_Shared_Resources/context/SLIDE-DECK-FORMAT.md` first.

---

## Unit 2 setup

```
Grade Level: Grade 4
Unit Name: Multi-Digit Multiplication & Early Division
Teaching Days: 20 (Part 1: Days 1–8 · Part 2: Days 9–14 · Part 3: Days 15–20)
Learning Goals: OA.5 (taught, not formally assessed) · NBT.A1 · NBT.5 · NBT.6

Part 1 (Days 1–8): How do multi-digit numbers work, and how does place value help us multiply?
Part 2 (Days 9–14): Recording strategies and efficient computation
Part 3 (Days 15–20): Multi-digit division with remainders

Curriculum sources: IM Grade 4 Unit 6 (Multiplying and Dividing Multi-digit Numbers) is the primary source — each card's "IM L#" tag names the IM lesson. Bridges Unit 2 fills three gaps only: Day 2 (ten-times place value, Great Wall of Base Ten), Day 7 (extra practice before Checkpoint 1), Day 12 (doubling/halving efficiency). Cards tagged "Bridges Supplement" are the ones that use Bridges.

Assessments: U2 Screener (pre-unit baseline, revised before each Checkpoint and on Day 20) · M1&M2 Checkpoint (Day 8) · M3 Checkpoint (Day 14) · M4 Checkpoint (Day 19). All three Bridges Checkpoints stay exactly as written.

Problem-solving routine: MESA (Model, Equation, Strategy, Answer with units).
Class context: see _Shared_Resources/context/HOW-I-WORK.md (24 Grade 4 students, mixed backgrounds, mostly strong with a few receiving learning support; UDL and Executive Functioning supports throughout).
```

---

## Source material for each lesson

- **IM-tagged days:** the IM lesson content comes from the IM source files or screenshots I add to `Resources/` (one subfolder per lesson, e.g. `Math Unit 2, Lesson 5 IM`). Use the IM activities, numbers, and routines as written.
- **Bridges Supplement days (2, 7, 12):** the Bridges pages come from `Resources/` the same way (e.g. `Math Unit 2, Lesson 2 Bridges`).
- **Checkpoint days (8, 14, 19):** the Checkpoint is administered as written. The lesson plan covers set-up, accommodations, and what to watch for. It does not rewrite the Checkpoint.
- If the source for a day isn't in `Resources/` yet, say so and ask me to add it. Do not rebuild it from memory.

---

## Generating a lesson

When I ask for a lesson, use the `/illustrative-math-lesson-generator` skill and follow it exactly. It produces the IM structure: Warm-up → Activities → Lesson Synthesis → Cool-down, with MLR and UDL notes and Responding to Student Thinking.

1. Pull that day's card from `G4_Math_U2_Lesson_Sequence.html`: learning target, tags, lesson description, mini-lesson focus, key activity, problem-solving conferring focus, assessment, and split-screen intention.
2. **Split-screen intentions:** use the one on the card verbatim in the lesson header (Kath Murdoch style, Learning Assets from `LEARNING-ASSETS.md`). Only generate new ones if I ask.
3. **Preserve the Bridges and IM math.** Don't drop a problem from the source without discussing it first.
4. **Cool-down:** one task, 5 minutes or less, with Next-Day Support and Prior-Unit Support.
5. **Sample student responses** use concrete numbers, never placeholders.
6. **Warm-up:** if I give a Math at Home link (mathathome.mathlearningcenter.org), use that activity as the warm-up.
7. **Problem-solving conferring** is named in every lesson, drawn from the card. It is never its own phase.
8. **Rosenshine's Principles:** name the principle inline where one is in play (e.g. "Rosenshine Principle 4: Provide models").
9. Fonts and palette follow `LESSON-PLAN-FORMAT.md` where it doesn't conflict with the IM skill's structure. Duplicate the template rather than rebuilding styling.

---

## Combining two IM lessons into one day

When a sequence card combines two IM lessons (e.g. "IM L19–L20"), don't teach both in full.

1. **The whole lesson runs 50 minutes or less**, Warm-up through Cool-down.
2. **Recommend 2–3 activities** across the two IM lessons: the ones that best serve the card's learning target and the next Checkpoint. Pick one Warm-up, one Lesson Synthesis (combine the two IM syntheses if both are useful), and one Cool-down.
3. **Show me the recommendation before building anything.** Use a short table (phase, time, IM source, why), then list what's cut and why, plus any optional "flex" problem if there's time. Wait for my OK. This is the "discuss first" step for dropped problems.
4. Cut material can go in the speaker notes or lesson plan as an early-finisher task, a center, or a next-day warm-up. Don't squeeze it back into the 50 minutes.

---

## Practice sets (when I ask for them)

Build in MESA format, with a comparison bar model in the Model step. Three tiers:

- Level 1: the source problems as-is
- Level 2: slightly harder numbers
- Level 3: a noticeable challenge

All tiers stay inside the grade-level standard. Provide an answer key as a separate file.

---

## Ask-first rule

Math Stage 3 content is locked (SYSTEM-RULES.md). Don't ask which activities to use. Only ask when a source is missing or a card is ambiguous. Requests that aren't lesson conversions (unit planning, split-screen intentions alone, thinking through a routine) should not trigger the lesson generator.

---

## Output

A `.docx` saved to `Outputs/` as:

```
Unit2_Lesson[Day#]_[Short_Title].docx
```

Example: `Unit2_Lesson5_Multiply_Three_and_Four_Digit_Numbers.docx`

---

## Pre-delivery check

- [ ] Learning target, tags, and split-screen intention match the sequence card exactly
- [ ] Source math preserved: no problems dropped (combined-lesson days: only the cuts I approved)
- [ ] Combined-lesson days: 2–3 activities, 50 minutes or less in total
- [ ] Full IM structure present (Warm-up, Activities, Lesson Synthesis, Cool-down, MLR/UDL notes)
- [ ] Cool-down is one task, 5 minutes or less, with Next-Day and Prior-Unit Support
- [ ] Sample student responses use real numbers
- [ ] Problem-solving conferring named per the card
- [ ] Checkpoint days: Checkpoint left as written
- [ ] No banned words, phrases, or structures (HOW-I-WORK.md)
- [ ] File named correctly and saved to `Outputs/`

---

## Unit Hub (teacher-facing web page)

`Outputs/Math_U2_Unit_Hub.html` is the teacher hub for this unit: every day's sequence card, embedded slides with speaker notes, embedded IM teacher guides / student pages / cool-downs, Checkpoints, small-group tasks, shared texts, and a standards matrix linking each day and Checkpoint to its standard.

- Content lives in `Outputs/_hub/hub_data.py`. Day titles, targets, descriptions, conferring and split-screen intentions are read from `Resources/G4_Math_U2_Lesson_Sequence_1.html`, so edit the sequence, not the hub, to change a card.
- Decks are picked up automatically by name: `Math U2 L## …pptx` (## = day) in `Resources/Math Unit 2 Resources/Current MAth U2 Slide Decks /`, `Resources/Slides/` or `Resources/OneDrive/`.
- Rebuild after any change: `cd Outputs/_hub && python3 build_hub.py --export` (export uses Keynote, only new or changed decks). `--package` builds a share zip without the .pptx files.
- When a new lesson plan, small-group task, shared text or rubric is saved to Outputs/ or Resources/, add it to `hub_data.py` (under the day in `EXTRA`, or `SMALL_GROUPS` / `TEXTS` / `RUBRICS`) and rebuild.
