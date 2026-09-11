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
**Status:** Locked for current phase

**Decision**  
Do not prematurely lock feature lists, UI, MVP scope, curriculum structure, or technical architecture. First establish the problem space, user needs, learning principles, competitive landscape, India-specific constraints, and age-group differences.

**Rationale**  
The market already contains abundant educational content and many strong learning products. Building another generic bundle would likely create weak differentiation.

---

## D-003 — India is the initial launch context

**Date:** 2026-09-11  
**Status:** Working strategic constraint

**Decision**  
Research and first product assumptions should be India-first while avoiding architecture that unnecessarily prevents later international expansion.

**Implications to investigate**

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
**Status:** Working philosophy; expected to become constitutional principle

**Decision**  
Do not optimize children toward maximum screen time, infinite sessions, addictive loops, or compulsive streak preservation. Engagement should serve learning.

---

## D-005 — AI must not default to answering

**Date:** 2026-09-11  
**Status:** Working philosophy

**Decision**  
AI behavior should depend on pedagogical context. A learning system may guide, hint, ask questions, verify, demonstrate, provide a direct answer, or refuse to solve the cognitive task on behalf of the learner depending on the learning objective.

---

## D-006 — Grade is context, not the learning model

**Date:** 2026-09-11  
**Status:** Working philosophy

**Decision**  
Do not assume all knowledge and skills correspond neatly to school grade. Future personalization should be concept- and mastery-aware.

---

## D-007 — Child-facing monetization must be non-manipulative

**Date:** 2026-09-11  
**Status:** Working philosophy

**Decision**  
Do not place children into the sales funnel. Avoid child-facing price prompts, emotional pressure to ask parents to unlock content, targeted advertising, and monetization mechanics that exploit frustration or attachment.

---

## D-008 — Child safety and privacy are architecture-level requirements

**Date:** 2026-09-11  
**Status:** Working philosophy

**Decision**  
Privacy, parental control, data minimization, age-appropriate AI behavior, profile separation, transparency, and child safety must be considered from the foundation rather than bolted on later.

---

## D-009 — The system should increase independence

**Date:** 2026-09-11  
**Status:** Working philosophy

**Decision**  
The best outcome is not dependency on an AI tutor. The system should help the learner progressively need less support as mastery improves.

**Candidate north-star:** Independent Mastery.

---

## Open decisions

The following remain deliberately unresolved:

- first target age range;
- exact problem wedge;
- whether the product is best framed as tutor, learning OS, learning intelligence layer, or another category;
- MVP subjects;
- curriculum relationship;
- parent experience;
- teacher/school role;
- gamification philosophy beyond the anti-addiction principles;
- AI architecture;
- offline strategy;
- monetization model;
- technology stack.
