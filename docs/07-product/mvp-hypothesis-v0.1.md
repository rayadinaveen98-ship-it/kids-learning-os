# Kids Learning OS — MVP Hypothesis v0.1

**Date:** 2026-09-11  
**Status:** Candidate MVP — must be validated before full implementation

---

# 1. MVP objective

Prove one thing:

> A short software-guided learning loop can diagnose an early-math misconception, teach the missing idea in an appropriate way, reduce support, and produce later independent performance that a parent can understand.

If we cannot prove that, the broader Learning OS thesis is not ready.

---

# 2. Target

- Age: 6–8
- Grade: 1–2
- Context: India
- Buyer: parent/caregiver
- User: child
- Platform: Android-first
- Initial environment: home / after-school

---

# 3. Initial subject scope

Foundational mathematics only.

Suggested V0 concept graph:

1. quantity and number sense;
2. comparing numbers;
3. number bonds;
4. place value basics;
5. addition within 20;
6. subtraction within 20;
7. crossing 10;
8. simple word problems;
9. early grouping/repeated addition;
10. basic measurement/comparison.

The exact set should be reduced further after parent/child validation.

---

# 4. Core child flow

## Entry

Parent or child selects one of:

- “I’m stuck”;
- current math topic;
- simple homework input.

Camera OCR is optional for V0 and should not be required for the core test.

## Diagnostic micro-loop

2–5 carefully chosen prompts that separate likely causes.

The system should not announce “assessment.”

## Intervention

Use one or more of:

- objects/counters;
- number line;
- visual grouping;
- short spoken explanation;
- home-language support;
- worked example;
- child explanation;
- physical mini-task.

## Scaffold fade

Move from:

`model -> guided -> hint -> independent`

## Independent check

Use a structurally similar but not identical problem.

## Close

Finite session with a clear stop.

---

# 5. Parent flow

Parent sees three things only:

### What was happening

> “Riya can subtract using objects but gets confused when the calculation crosses 10.”

### What changed today

> “She solved two new crossing-10 problems independently after using a make-10 strategy.”

### What happens next

> “No more work tonight. We’ll re-check this tomorrow for retention.”

The dashboard should not begin as a dense analytics product.

---

# 6. Minimum Child Learning Model

For every concept:

- prerequisite state;
- current mastery state;
- last evidence date;
- support required;
- representation used;
- independent check result;
- retention check result.

Do not store speculative personality labels.

---

# 7. AI use in V0

AI should be narrow and controlled.

### Deterministic/local first

- concept graph;
- question selection;
- expected-answer checking;
- scaffold state;
- session state;
- spaced revisit scheduling;
- most parent-report templates.

### AI where useful

- classify a spoken/written explanation;
- generate a safe equivalent example;
- rephrase an explanation;
- multilingual/code-switched explanation;
- summarize evidence for parent;
- interpret a photographed homework problem in later prototype.

The model must operate behind pedagogical rules.

---

# 8. Voice hypothesis

Voice can improve accessibility for ages 6–8, but V0 should not require continuous premium real-time voice.

Candidate approach:

- tap-to-speak;
- short responses;
- local/native TTS where quality is sufficient;
- cloud speech selectively;
- text/touch fallback;
- explicit microphone indicator;
- no background listening.

---

# 9. Language hypothesis

Do not attempt all Indian languages in V0.

Prototype with:

- English school terminology;
- one or two familiar-language explanation modes during pilots.

The language pair should be selected based on accessible pilot families, not founder preference alone.

Architecture should keep:

`concept language != UI language != school terminology`

so expansion remains possible.

---

# 10. Session constraints

Target:

- 5–15 minutes;
- one clear learning objective;
- finite endpoint;
- no autoplay chain;
- no streak threat;
- no forced reward loop;
- optional short off-screen task where pedagogically useful.

---

# 11. MVP non-goals

V0 does not need:

- all school boards;
- all subjects;
- story generation;
- avatar world;
- social features;
- teacher dashboards;
- live tutors;
- leaderboard;
- open internet;
- long-form video library;
- general AI chat;
- elaborate subscription system;
- school integrations;
- perfect homework OCR.

---

# 12. Validation metrics

## Learning

- pre-intervention success;
- independent post-intervention success;
- next-day retention;
- changed-context transfer;
- support reduction.

## Parent

- minutes of intervention saved;
- understanding of child state;
- trust rating;
- perceived usefulness;
- repeat-use behavior;
- willingness to replace current workaround.

## Child

- session completion;
- frustration indicators;
- willingness to explain reasoning;
- voluntary return;
- ability to stop without manipulative reward dependence.

## System

- incorrect diagnosis rate;
- unsafe/incorrect AI output rate;
- latency;
- data consumption;
- AI cost per completed session;
- low-end Android reliability.

---

# 13. MVP success condition

The MVP is promising if repeated testing shows that:

1. it finds a useful missing prerequisite/misconception often enough to matter;
2. the child improves within the session;
3. the child can still perform later with less/no help;
4. the parent understands the result;
5. the parent saves time or gains clarity;
6. the child tolerates/enjoys the process without addictive mechanics;
7. economics remain compatible with India-scale pricing.

---

# 14. MVP failure condition

Pivot if:

- diagnosis adds complexity without improving learning;
- the child simply wants a direct answer;
- parents do not perceive enough value beyond free alternatives;
- retention does not improve;
- parent supervision remains high;
- multilingual behavior is unreliable/confusing;
- AI errors create unacceptable trust risk;
- session cost is too high.

---

# 15. Build order after validation

1. concept/prerequisite graph;
2. deterministic session engine;
3. child profile + evidence model;
4. simple touch-based diagnostic activities;
5. scaffold engine;
6. independent/retention checks;
7. parent evidence summary;
8. selective AI explanation layer;
9. voice;
10. homework image input;
11. richer physical-world activities.

Do not reverse this order and build the flashy AI/avatar layer before the learning engine.
