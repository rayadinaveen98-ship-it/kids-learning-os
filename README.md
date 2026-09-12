# Kids Learning OS

**Status:** Product Definition v1.0 + Validation Prototype v0.2 complete; direct family validation is in progress.

Kids Learning OS is an India-first research and product-development project exploring a child learning system that prioritizes understanding, independent mastery, curiosity, safety, multilingual teaching, and real-world learning over content volume or screen-time engagement.

This repository is the permanent source of truth for research, product philosophy, decisions, hypotheses, sources, prototypes, architecture, and future implementation.

## Current phase

**Product Definition + Direct Validation**

The broad desk-research phase is complete. The current leading launch hypothesis is:

> **A trusted after-school learning bridge for ages 6–8 / Grades 1–2 that finds why a child is stuck, repairs the missing foundation, fades support, and shows the parent when the child can do it independently.**

Foundational mathematics remains the first validation domain because prerequisite relationships are explicit and independent transfer can be measured without requiring constant generative AI.

This remains a hypothesis until direct validation is sufficiently complete.

## Live Validation Prototype v0.2

Canonical public URL:

https://kids-learning-os-validation.vercel.app

Source and field protocol:

`prototype/validation-v0.2/`

### What changed from v0.1

Early anonymized field observations showed:

- most children appeared to understand the provided hints;
- some children still struggled;
- some children used finger counting and took additional time;
- Grade 1 and Grade 2 were receiving the same question path.

Validation v0.2 corrects those issues.

### Grade-aware starting paths

**Grade 1**

- start: `8 − 3`
- diagnostic if needed: `5 − 2`
- practice: `9 − 4`
- independent transfer: `7 − 3`

**Grade 2**

- start: `34 − 8`
- diagnostic if needed: `14 − 8`
- practice: `43 − 7`
- independent transfer: `52 − 8`

The governing principle is:

> **Grade chooses the starting point. Demonstrated ability determines where the child goes next.**

A Grade 2 child can step backward to a concrete prerequisite. A stronger child can remain on the grade-level path.

### Strategy evidence

v0.2 records the child-reported approach to the first problem:

- fingers;
- mental counting;
- breaking the number apart;
- remembered / just knew;
- drawing or imagined objects;
- not sure.

Finger counting and slower responses are treated as useful strategy/fluency evidence, not automatic failure. Time is shown to the parent only as context and is not scored.

### Scaffolding

v0.2 introduces two hint levels rather than one:

1. lighter conceptual/verbal prompt;
2. stronger visual or worked-step support.

This lets field testing observe how much support was actually required.

### Privacy

The prototype contains:

- no backend database;
- no account;
- no child name;
- no camera or microphone;
- no analytics SDK;
- no external AI calls;
- no ads or child-facing monetization.

It is a validation instrument, not a production assessment or diagnostic tool.

## Direct validation evidence

First anonymized field patterns are recorded in:

`docs/06-user-research/direct-family-validation-v0.1-observations.md`

Validation tracking continues in GitHub Issue #2.

No individual child/parent reviews or identifying data are required in this public repository. Aggregate patterns are enough to guide product decisions.

## Core project principles

1. Learning > engagement.
2. Understanding > content consumption.
3. Ability > grade label.
4. AI should assist thinking, not replace it.
5. Mistakes are diagnostic signals.
6. School performance and genuine understanding both matter.
7. Personalization should change teaching, not merely question difficulty.
8. Parents deserve understandable evidence of learning.
9. Curiosity belongs inside education.
10. Screen-based learning should sometimes lead away from the screen.
11. Language should adapt naturally to the child.
12. Children must never become advertising inventory.
13. Parent trust beats growth hacks.
14. The system should make the learner increasingly independent of the system.
15. Child mode never sells.
16. Shared-device/offline India realities are architecture constraints, not edge cases.

## Foundation completed

- [x] Broad India education and EdTech landscape research
- [x] Parent/student/teacher problem map
- [x] Ages 4–8 Foundational Stage research
- [x] India family-life / homework / tuition / device research
- [x] Learning-science synthesis
- [x] Competitor teardown
- [x] Child-AI safety and India privacy constraints
- [x] Android/shared-device/offline operating constraints
- [x] AI technical/economic viability analysis
- [x] Opportunity map and launch-wedge ranking
- [x] Product Foundation v1.0 readiness
- [x] Product Definition v1.0 hypothesis
- [x] Direct-validation plan and interview kit
- [x] Validation Prototype v0.1
- [x] First anonymized field observations
- [x] Validation Prototype v0.2
- [x] Public v0.2 deployment

## Current critical path

### Direct Validation v0.2

- [ ] Run v0.2 on at least three real mobile browser/device combinations
- [ ] Continue parent/caregiver interviews
- [ ] Continue parent-consented child sessions
- [ ] Compare Grade 1 vs Grade 2 starting difficulty
- [ ] Observe strategy use: fingers / counting / decomposition / objects
- [ ] Measure which hint level is required
- [ ] Observe Grade 2 prerequisite step-back behavior
- [ ] Track independent transfer outcome
- [ ] Test English-only vs code-switched explanations
- [ ] Test homework-rescue vs daily-coach entry points
- [ ] Test parent mastery report vs score/XP reporting
- [ ] Validate willingness to pay after real use
- [ ] Write Validation v0.2 findings
- [ ] Decide proceed / modify wedge / stop
- [ ] Lock Product Thesis v1.0
- [ ] Lock MVP scope and measurable learning thresholds

## After validation

- [ ] Define technical architecture
- [ ] Create production design system
- [ ] Implement narrow Android MVP
- [ ] Produce installable APK milestones
- [ ] Pilot with real families
- [ ] Measure independent mastery and retention
- [ ] Expand only after the core loop proves value

## Future expansion research — not a blocker

- [ ] Ages 9–12 deep research
- [ ] Ages 13–16 deep research
- [ ] Teacher/school B2B research
- [ ] International curriculum expansion research

## Key documents

- `docs/07-product/product-definition-v1.0.md`
- `docs/06-user-research/validation-plan-v1.0.md`
- `docs/06-user-research/direct-family-validation-v0.1-observations.md`
- `prototype/validation-v0.2/README.md`
- `prototype/validation-v0.2/DEPLOYMENT.md`
- `docs/07-product/mvp-hypothesis-v0.1.md`
- `docs/07-product/product-foundation-v1.0-readiness.md`
- `docs/07-product/opportunity-map-v0.7.md`
- `docs/07-product/technical-economic-viability-v0.7.md`
- `docs/05-competitors/deep-teardown-v0.3.md`
- `docs/03-learning-science/learning-science-ai-pedagogy-v0.4.md`
- `docs/04-india/india-privacy-safety-operating-constraints-v0.4.md`
- `research/source-log.md`

## Evidence rule

Forums, Reddit, app reviews, and anecdotes are treated as signals rather than population-level evidence. Direct family feedback is stored as anonymized patterns unless participants explicitly authorize otherwise.

## Current product thesis

> **When a child is stuck, Kids Learning OS should identify the missing step, teach it in a way the child understands, reduce help as competence grows, re-check independent performance, and show the parent meaningful evidence without turning the child into a captive screen user.**
