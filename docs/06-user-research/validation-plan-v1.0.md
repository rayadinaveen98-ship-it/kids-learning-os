# Kids Learning OS — Direct User Validation Plan v1.0

**Date:** 2026-09-11  
**Status:** Ready to execute  
**Goal:** Validate whether the proposed ages 6–8 after-school learning bridge solves a real recurring problem strongly enough to justify building the MVP.

---

# 1. Validation principles

We are no longer trying to prove that education is a large market.

We are trying to falsify specific product hypotheses.

Rules:

1. Ask about real recent behavior, not opinions about hypothetical apps.
2. Do not pitch the product before understanding the current workaround.
3. Do not interpret politeness as demand.
4. Prefer examples from yesterday/this week over general claims.
5. Observe child behavior where possible instead of relying only on parent recollection.
6. Separate willingness to try from willingness to pay.
7. Keep child testing safe, short, parent-present and non-diagnostic.
8. Record contradictory findings.

---

# 2. Primary hypotheses to test

## H1 — Homework/learning friction is frequent enough

Parents of Grades 1–2 regularly encounter situations where the child is stuck and the parent must intervene, search online, ask someone, or use tuition.

## H2 — Parents often cannot identify the real missing concept

The visible homework question is frequently not the actual learning gap.

## H3 — Parents value diagnosis + intervention more than a content library

A parent prefers:

> “Here is what your child is missing and here is a 10-minute intervention”

rather than:

> “Choose from thousands of lessons.”

## H4 — Guided help is preferred over answer-giving

Parents want the child to understand rather than merely finish homework, at least in the target segment.

## H5 — Plain-language progress evidence matters

Parents value evidence such as:

> “Can now subtract across 10 independently”

more than XP, streaks or time spent.

## H6 — Multilingual explanation creates meaningful value

Some English-medium families want conceptual explanation in a familiar/home language while preserving school terminology.

## H7 — A 10–15 minute focused session is acceptable

Families can realistically fit short learning sessions into the after-school routine.

## H8 — Parents trust a bounded AI learning tool more than an open chatbot

Clear safety rules and parent visibility increase willingness to let the child use the product.

## H9 — Foundational mathematics is a strong first wedge

Parents perceive enough value in help with early maths concepts to drive repeated use.

## H10 — The product can save parent time

A successful session can reduce the amount of direct parent teaching/supervision required.

---

# 3. Interview segments

Minimum useful first round: **20–30 parent interviews** across deliberately varied contexts.

Suggested mix:

### School type
- CBSE private;
- State Board private;
- government/aided where accessible;
- ICSE if available.

### Geography
- metro / Tier 1;
- Tier 2;
- Tier 3 / smaller town.

### Language
- English-medium + home language different;
- regional-medium;
- bilingual households.

### Learning support
- no tuition;
- occasional tuition;
- regular tuition.

### Parent working context
- both parents working;
- one primary caregiver at home;
- grandparent-supported household.

The goal is not statistical representativeness. It is to discover whether the problem is robust across relevant contexts and which segment feels it most sharply.

---

# 4. Parent interview guide

## Context

1. Tell me about your child’s school day on a normal weekday.
2. What happens between getting home and bedtime?
3. Who usually handles homework or school practice?
4. Does the child use a phone/tablet/TV for learning? Whose device?

## Recent friction

5. Think about the last time your child got stuck on homework. What happened from the beginning?
6. What exactly were they stuck on?
7. What did you try first?
8. Did you know why they were getting it wrong?
9. Did you search YouTube/Google/WhatsApp, ask a teacher, use an app, or call a tutor?
10. Roughly how long did the whole situation take?
11. How did the child react emotionally?
12. How did you react?

## Current alternatives

13. Do you use tuition/coaching? Why or why not?
14. What learning apps or YouTube channels do you currently use?
15. Which one do you trust most? Why?
16. What frustrates you about them?
17. Have you paid for any app or learning service? What made it worth paying for?

## Understanding progress

18. How do you currently know whether your child truly understands something?
19. Does the school give you enough information?
20. What would you most like to know that you cannot easily know today?

## Language

21. What language does your child speak most comfortably at home?
22. What is the school medium?
23. When a difficult concept is explained, which language works best?
24. Do you ever switch languages while explaining homework?

## AI/safety

25. Has your child used ChatGPT/Gemini/other AI tools?
26. Would you let your child talk to an AI tutor? What would worry you?
27. How would you feel about microphone use during a lesson?
28. Camera use for a homework photo?
29. What controls would you expect as a parent?

## Value test — only after discovery questions

30. Suppose a tool could identify the missing prerequisite, teach it in 10 minutes, and tell you whether your child can now do it independently. What would be useful about that?
31. What sounds unrealistic or worrying?
32. When would you use it instead of YouTube or tuition?
33. What would make you stop using it?

Do not ask “Would you buy this?” as the primary evidence of demand.

---

# 5. Child observation sessions

Target: small parent-consented sessions with ages 6–8.

Session length: roughly 10–15 minutes.

Never frame as an intelligence test.

Observe:

- whether instructions are understandable;
- response to mistakes;
- whether voice or touch feels easier;
- tolerance for short diagnostic questions;
- reaction to different representations;
- willingness to explain thinking;
- whether the child can solve a parallel problem after help;
- whether hints can be reduced;
- frustration/boredom signals;
- ability to stop when session ends.

The purpose is UX/learning-flow validation, not developmental diagnosis.

---

# 6. Prototype experiments

## Experiment A — Diagnosis vs direct explanation

Show two flows for the same wrong answer:

A. immediate explanation;
B. 2–3 diagnostic prompts before explanation.

Measure:

- child frustration;
- parent perceived intelligence/value;
- whether diagnosis leads to a better intervention.

## Experiment B — English-only vs code-switched explanation

For bilingual families, compare:

- English-only conceptual explanation;
- familiar-language explanation retaining English school terminology.

Measure comprehension and parent/child preference.

## Experiment C — Parent report

Compare:

A. scores/XP/minutes;
B. plain-language mastery evidence.

Ask which one helps the parent decide what to do next.

## Experiment D — Homework rescue vs daily coach

Present both entry points:

- “Help with what we’re stuck on now”;
- “Give us today’s 10-minute learning session.”

Observe which has stronger immediate demand and repeat-use intent.

## Experiment E — Digital vs physical activity

After a concept, test whether a small off-screen activity improves engagement/transfer without creating parent burden.

---

# 7. Evidence thresholds before MVP lock

These are directional decision gates, not statistical proof.

Proceed strongly if most of the following appear:

- repeated recent examples of homework/learning friction across segments;
- parents describe meaningful time/emotional burden;
- current workarounds are fragmented or expensive;
- diagnosis is perceived as useful rather than threatening;
- children can tolerate and benefit from short diagnostic teaching loops;
- independent re-check demonstrates learning in prototype sessions;
- at least one parent segment shows clear repeat-use behavior;
- multilingual explanation provides real value in a meaningful subset;
- parent trust improves with bounded AI/safety controls;
- a credible willingness-to-pay signal appears after real use.

---

# 8. Kill / pivot criteria

We should materially change the thesis if:

- parents rarely experience the problem;
- YouTube/teachers/tuition already solve it satisfactorily for the target segment;
- parents mainly want answer completion rather than understanding;
- diagnosis feels too slow or annoying for children;
- parents do not trust AI-based intervention even with controls;
- measurable independent mastery does not improve;
- the product does not save parent time;
- session economics require unsustainably expensive cloud AI;
- the child experience needs so much parent involvement that the value proposition collapses.

A failed hypothesis is useful evidence, not a project failure.

---

# 9. Data to record from every interview

- child age/grade;
- school board/type;
- home language;
- school medium;
- device access;
- tuition status;
- last homework-friction event;
- time spent resolving it;
- current workaround;
- parent’s main concern;
- trust concerns;
- current paid learning services;
- strongest quote/behavioral evidence;
- hypothesis supported/refuted;
- follow-up prototype candidate.

Do not store unnecessary identifying information.

---

# 10. Validation sequence

### Round 1 — Problem discovery
20–30 parent conversations.

### Round 2 — Concept test
Clickable/voice-assisted low-fidelity prototype with ~8–12 families.

### Round 3 — Wizard-of-Oz learning sessions
Human/AI-assisted prototype that simulates diagnosis and tutoring before engineering the full system.

### Round 4 — Narrow functional MVP
Real child model for a limited math concept graph.

### Round 5 — Learning/retention validation
Check independent performance after delay and across changed problem forms.

Only after this should the broader platform roadmap become implementation scope.
