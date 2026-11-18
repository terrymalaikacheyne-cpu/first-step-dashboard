# F.I.R.S.T. STEP — Making the pilot run itself

**For:** Terry Malaika Cheyne, Team Lead
**Date:** 17 November 2026
**Companion files:** `FIRST-STEP-Dashboard.html` · `FIRST-STEP-Master-Tracker.csv` · `FIRST-STEP-Scoring-Rubric.csv`

---

## The one-sentence diagnosis

The programme is working; the **evidence system** is not. Delivery is 3 of 7 weeks in and Month 2 is already built, but only **5 of 18 participant-week items** (28%) can be documented, and **4 of 18** (22%) rest on a real artefact. Everything below is aimed at that gap, not at more content.

What the folder audit actually found:

- Week 2 and Week 3 have **zero participant submissions**. Five Week 3 files are byte-identical to the blank template (4,604 characters, 3 placeholders) — they were saved with names, never filled in.
- Jan's Week 1 file is also a blank template, yet Week 1 is reported as complete for him. The report and the artefact disagree.
- Aki's blank Week 1 file still sits in the cohort folder, inflating the denominator.
- Week 2 has no session notes or recording at all, so attendance cannot be evidenced even in principle.
- Nothing anywhere captures a score or a rubric, so a strong reflection and a rushed one look identical in reporting.

That is a process design problem, not a commitment problem. The cohort is engaged — the Week 1 writing proves it.

---

## Six changes, in order of impact

### 1. One master tracker, one row per participant-week

**Now:** each person keeps their own Drive copy, so "submitted" is indistinguishable from "downloaded". You reconstruct completion by opening files.

**Change:** a single sheet — `FIRST-STEP-Master-Tracker.csv` is already built and prefilled with all 42 participant-week rows. Columns that matter: `Status`, `Evidence link`, `Reviewed by`, `Submitted on`, `Score (1-5)`, `Next action`, `Due`.

**Rule:** a status may only move to **Complete** when `Evidence link` has a URL and `Reviewed by` has initials. Everything else is *Not verifiable* — a legitimate, reportable state.

**Time effect:** completion reporting drops from ~45 minutes of folder archaeology to a filter on one column.

### 2. A 30-second submission form instead of "send me your log"

**Now:** you chase six people across chat, email and Drive, and still cannot tell who sent what.

**Change:** Google Form → responses into the tracker. Four fields: name, week, link, one sentence — *"what changed in your work this week?"* That last field is the only quality signal you need, and it takes ten seconds to read.

Add one automation: reminder at **session + 24h**, escalation to you at **+48h**. Either Apps Script or a Calendar reminder plus a saved Gmail draft will do. The form is the point; the automation is the multiplier.

**Time effect:** chasing becomes an exception, not a routine.

### 3. Kill the blank-template failure mode

**Now:** "make a copy" produces a file that looks like a submission.

**Change:** stop distributing editable copies. Either (a) assign via Google Classroom/Forms so the response *is* the submission, or (b) use a `Make a copy` link with the participant's name pre-filled in the filename and the header, plus a bold line at the top: *"This file is a template until your name appears in the header and every placeholder is gone."*

Also: rename to a convention that sorts — `W03_Afril_Kahulugan_Log`. At six people this is cosmetic; at twenty it is the difference between a usable archive and a folder of noise.

### 4. Make the week's notes do the chasing for you

**Now:** the Gemini notes already contain the action items (Week 3 literally records *"Jan — watch recording and complete the log"*), but they sit in a 183 KB docx nobody reopens.

**Change:** after each session, copy the **Next steps** block straight into the tracker's `Next action` / `Due` columns. Two minutes, and every commitment has an owner and a date.

### 5. Protect the one structural constraint — Krystel

This is the only risk that cannot be solved with a form. She is the sole Ode participant, the campaign is an agent down, and she is carrying coverage. No amount of process design fixes that.

**Change:** book a **recurring 45-minute protected window** with the Ode lead and treat it as a client commitment with a name against it. Record it. If the slot is lost, she watches the recording within 48 hours — but the slot is the primary plan, not the fallback.

Do not let this roll into Month 2. If it does, the pilot's first leadership outcome will be "the one person we could not release".

### 6. Stop measuring attendance; measure artefacts

Jan and Noemi are part-time buffers on another campaign. They left the Week 3 session at 00:28. They will keep doing that, and it is not a performance issue.

**Change:** every session is recording-first with a 48-hour log deadline. Live attendance is a delivery metric, not a completion metric. This removes an unfair penalty and makes the completion number honest at the same time.

---

## The weekly rhythm (15 minutes total)

| When | What | Time |
|---|---|---|
| Monday | Open the dashboard, read three numbers: documented completion, open evidence items, capstone pipeline | 5 min |
| After each session | Paste the Gemini "Next steps" into the tracker | 2 min |
| +24h | Form reminder fires automatically | 0 min |
| +48h | Only chase the exceptions the dashboard shows in red | 5 min |
| Logs are in | Score the week as a cohort, one pass | 2 min per log |
| Friday | `Copy update` on the dashboard → paste into the leadership note → edit two sentences | 3 min |

That is the whole operating model. Everything else is delivery.

---

## Scoring the assessment logs (2 minutes each)

A completion tick tells you a file exists. It does not tell you whether the learning landed. The rubric closes that gap without turning into an essay-marking exercise.

- **Five criteria, five points each, 25 total.** Four are common to every week: completion and accuracy, specificity, application, reflection depth. The fifth changes by week — DISC consistency in Week 1, a workable energy plan in Week 2, data hygiene and AI guardrails in Week 3, analysis-to-decision in Week 4, and so on.
- **The gate:** 15 / 25 or above, with no criterion below 3. Below that, return the log once with a single rewrite instruction.
- **Score the whole cohort on the same week in one sitting.** Consistency comes from comparing logs against each other; scoring one person on Monday and another on Friday produces drift.
- **Score only what is written.** The insight in your head does not count. This is also what makes the score defensible if a participant challenges it.

Where: the **Scoring** tab in the dashboard (click any cell, score all five criteria, add one line of feedback) and `FIRST-STEP-Scoring-Rubric.csv` for a printable or Google Sheets version. The rubric is deliberately identical in both, so the standard does not move depending on where it is applied.

---

## Two-week rollout

**This week (by 21 Nov)**
- [ ] Load `FIRST-STEP-Master-Tracker.csv` into Google Sheets; share as the single source of truth.
- [ ] Publish the submission form and put the link in the cohort chat, pinned.
- [ ] Reissue Week 2–4 logs as `Make a copy` links with names prefilled.
- [ ] Back-fill Weeks 2–4: every row ends the week as Complete, Partial or Missing — no greys left.
- [ ] Fix Jan's Week 1 (recover or resubmit) and archive Aki's file out of the cohort folder.

**Next week (by 28 Nov)**
- [ ] Confirm Krystel's recurring 45-minute window with the Ode lead.
- [ ] Confirm department track and shadow buddy for all six.
- [ ] Open capstone scoping in the Week 5 lifecycle session — one page each: problem, metric, baseline, target, owner.
- [ ] Add `Score (0-25)` and `Reviewed by` to every completed row from Week 4 onward.
- [x] Score Week 1 as a calibration set (done 17 Nov): five logs, 11-24 out of 25. The spread is wide enough that the anchors hold — leave them alone now.
- [x] Score Kyle's Week 2 and Week 3 logs (23 and 20): the only Weeks 2-3 submissions on file.

---

## What the dashboard is for (and not for)

- **For:** a five-minute Monday review, a defensible completion number, a one-click leadership update, and a single place where the capstone pipeline is visible.
- **Not for:** ranking agents. Completion is a programme-health metric. The moment it becomes a performance score, people will submit for the metric rather than for the learning — and the reflections are the most valuable thing you have.
- **Edit mode** writes to your browser only, so treat it as a working view. The tracker is the record. Use `Export CSV` to move edits across.

---

## The one number to watch

Not attendance. Not sessions delivered. This one:

> **Scoped capstones with a baseline metric.**

Five people can name a workflow to redesign. Zero have a baseline. When that number reaches five, the pilot has produced something leadership can measure in AHT, FCR, QA or CSAT — and the business case writes itself.
