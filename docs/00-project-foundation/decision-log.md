# Decision Log

This file records meaningful product and research decisions so the project does not drift as conversations, contributors, and implementation phases change.

Each entry should include: date, decision, status, rationale, evidence, and conditions that could cause reconsideration.

---

## D-001 — Git repository is the permanent source of truth

**Date:** 2026-09-11  
**Status:** Locked

**Decision**  
`rayadinaveen98-ship-it/kids-learning-os` is the permanent source of truth for project research, product philosophy, decisions, specifications, architecture, and future implementation.

**Rationale**  
The project is expected to span many research and build sessions. Git preserves continuity, provenance, version history, and recovery across chat limits or tooling changes.

---

## D-002 — Do not design the product before completing foundational research

**Date:** 2026-09-11  
**Status:** Completed for broad desk-research phase

**Decision**  
Do not prematurely lock feature lists, UI, MVP scope, curriculum structure, or technical architecture before establishing the problem space, user needs, learning principles, competitive landscape, India-specific constraints, and age-group differences.

**Current state**  
The first broad desk-research cycle is now complete enough to move into direct parent validation and product definition. Research continues as supporting work rather than as a blocker.

---

## D-003 — India is the initial launch context

**Date:** 2026-09-11  
**Status:** Working strategic constraint

**Decision**  
Research and first product assumptions should be India-first while avoiding architecture that unnecessarily prevents later international expansion.

**Implications**

- CBSE, ICSE, and State Boards;
- multilingual and code-switched teaching;
- shared family devices;
- tuition/coaching culture;
- school-exam performance expectations;
- affordability;
- connectivity/offline needs;
- child-data regulation in India;
- regional socioeconomic differences.

---

## D-004 — Learning is more important than engagement

**Date:** 2026-09-11  
**Status:** Locked philosophy

**Decision**  
Do not optimize children toward maximum screen time, infinite sessions, addictive loops, or compulsive streak preservation. Engagement should serve learning.

---

## D-005 — AI must not default to answering

**Date:** 2026-09-11  
**Status:** Locked philosophy

**Decision**  
AI behavior should depend on pedagogical context. A learning system may guide, hint, ask questions, verify, demonstrate, provide a direct answer, or refuse to solve the cognitive task on behalf of the learner depending on the learning objective.

---

## D-006 — Grade is context, not the learning model

**Date:** 2026-09-11  
**Status:** Locked philosophy

**Decision**  
Do not assume all knowledge and skills correspond neatly to school grade. Future personalization should be concept-, prerequisite-, support- and mastery-aware.

---

## D-007 — Child-facing monetization must be non-manipulative

**Date:** 2026-09-11  
**Status:** Locked philosophy

**Decision**  
Do not place children into the sales funnel. Avoid child-facing price prompts, emotional pressure to ask parents to unlock content, targeted advertising, loot-box/premium-currency mechanics, and monetization that exploits frustration or attachment.

---

## D-008 — Child safety and privacy are architecture-level requirements

**Date:** 2026-09-11  
**Status:** Locked philosophy

**Decision**  
Privacy, parental control, data minimization, age-appropriate AI behavior, profile separation, transparency, and child safety must be considered from the foundation rather than bolted on later.

---

## D-009 — The system should increase independence

**Date:** 2026-09-11  
**Status:** Locked philosophy

**Decision**  
The best outcome is not dependency on an AI tutor. The system should help the learner progressively need less support as mastery improves.

**Candidate north-star:** Independent Mastery.

---

## D-010 — Reject “all-in-one content app” as the core product thesis

**Date:** 2026-09-11  
**Status:** Locked research conclusion

**Decision**  
Do not define differentiation as having all subjects, large content volume, videos, worksheets, quizzes, regional-language content, curriculum alignment, games or a generic AI chatbot in one application.

**Rationale**  
Competitor research shows every one of these capabilities already exists in strong products. They may be useful components, but they are not a sufficient strategic moat.

---

## D-011 — Persistent Child Learning Model is the leading moat hypothesis

**Date:** 2026-09-11  
**Status:** Research thesis; requires validation

**Decision**  
The strongest current strategic hypothesis is a longitudinal learner model that tracks concept prerequisites, assisted vs independent mastery, explanation/retention/transfer evidence, support history, school context and language context.

**Explicit boundary**  
The model must not infer clinical diagnoses, IQ, personality types or mental-health conditions.

---

## D-012 — Ages 6–8 is the leading first commercial wedge hypothesis

**Date:** 2026-09-11  
**Status:** Research recommendation, not locked MVP

**Decision**  
Before interviews, ages 6–8 / Grades 1–2 rank highest as the first commercial wedge because school/homework friction is recurring, foundational gaps are observable, tuition begins to appear, parent value is measurable, and guided tutoring is developmentally more appropriate than for preschoolers.

**Reconsider if**  
Direct parent research shows a stronger pain/value proposition in ages 4–5 or another segment.

---

## D-013 — Ages 4–5 and 6–8 should not share one undifferentiated child UX

**Date:** 2026-09-11  
**Status:** Strong research conclusion

**Decision**  
Ages 4–5 should be more play-, story-, movement-, parent- and off-screen-oriented. Ages 6–8 can introduce more explicit tutoring, reading, arithmetic, school bridging and independent work. They may share an underlying learning engine but should not be treated as the same child-facing product.

---

## D-014 — India architecture must assume shared Android devices and imperfect connectivity

**Date:** 2026-09-11  
**Status:** Strong research constraint

**Decision**  
Future implementation should assume a parent-owned/shared Android phone, interruptions, multiple child profiles, variable connectivity and the need for offline/downloading/resume support. A personal-tablet/always-online assumption is unacceptable for the India-first product.

---

## D-015 — AI architecture should be hybrid, not always-on cloud intelligence

**Date:** 2026-09-11  
**Status:** Strong research recommendation

**Decision**  
Use deterministic/local logic and on-device capabilities for routine interactions where feasible; use cloud AI selectively for high-value reasoning, tutoring, language adaptation, vision and synthesis. Do not make every child minute an expensive realtime AI session.

**Rationale**  
This improves economics, privacy, latency, offline capability and reliability.

---

## D-016 — Child mode never sells and should have natural stopping points

**Date:** 2026-09-11  
**Status:** Locked philosophy

**Decision**  
Child mode should contain no ads, purchase prompts, premium teasers, streak-loss threats, infinite feeds or synthetic-attachment notifications. Sessions should be finite and able to end positively.

---

## D-017 — Desk research is no longer the critical path

**Date:** 2026-09-11  
**Status:** Locked process decision

**Decision**  
Do not continue broad, unfocused market research before testing the product thesis. The next evidence should come from direct parent interviews, child/parent prototype testing and measurable learning experiments.

**Future expansion research**  
Ages 9–12 and 13–16 remain important long-term research areas, but they are not prerequisites for validating the first 4–8/6–8 wedge.

---

## D-018 — After-school learning bridge is the leading launch proposition

**Date:** 2026-09-11  
**Status:** Product hypothesis — must be validated

**Decision**  
The leading proposition to test is not a generic tutor or content library. It is an after-school learning bridge for ages 6–8 that starts when a child is stuck, identifies the likely missing prerequisite or misconception, teaches through an appropriate representation/language, fades support, re-checks independent performance and gives the parent plain-language evidence.

**Alternatives retained for testing**  
A daily foundation coach and a parent learning radar remain credible alternative propositions. They should be tested rather than discarded prematurely.

---

## D-019 — Foundational mathematics is the recommended first validation domain

**Date:** 2026-09-11  
**Status:** MVP hypothesis — not a permanent company scope

**Decision**  
Use foundational mathematics as the first narrow domain for validating the Learning OS because prerequisite relationships are relatively explicit, independent mastery can be measured, multiple representations can be tested, and the core loop can operate economically without continuous generative AI.

**Boundary**  
Kids Learning OS is not defined as a mathematics company. Reading/language is the next major domain if the learning engine validates.

---

## D-020 — MVP exists to prove the learning loop, not feature breadth

**Date:** 2026-09-11  
**Status:** Locked product-development rule for the validation phase

**Decision**  
The first functional MVP must prove:

`Diagnose -> Teach -> Practice -> Fade Help -> Independent Check -> Revisit Later -> Parent Evidence`

Do not add broad subjects, avatar worlds, social systems, large content libraries, school administration, live classes or open-ended AI chat before this loop shows measurable value.

---

## Open decisions

The following remain deliberately unresolved until direct validation/prototyping:

- final first target parent segment/geography;
- whether homework rescue or daily foundation coaching drives stronger retention;
- exact first math concept graph;
- first school board/curriculum mapping;
- first language pair(s) for pilot;
- camera/homework OCR scope in V0;
- voice depth and speech stack;
- exact session length;
- visual/game layer;
- parent-report depth;
- teacher/school role in V1 vs later;
- exact gamification model;
- exact AI providers/models;
- precise offline implementation;
- pricing/monetization tiers;
- technology stack;
- product name/brand;
- quantitative launch thresholds after prototype evidence.
