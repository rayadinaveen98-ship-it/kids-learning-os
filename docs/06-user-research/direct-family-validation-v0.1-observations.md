# Direct Family Validation v0.1 — First Anonymized Observations

**Date:** 2026-09-12  
**Status:** Early qualitative field observations; not a completed validation sample.  
**Privacy:** No child or parent identities, quotes, recordings, or identifying details are stored.

## What was observed

The field tester reported the following aggregate patterns after showing the validation prototype to multiple Grade 1 / Grade 2 children and parents:

1. **Most children understood the hints.**
   - This is early support for the hypothesis that the scaffolded hint flow can help children continue without immediately giving the final answer.
   - This is qualitative only; exact counts were not recorded.

2. **A smaller group still struggled after hints.**
   - This is important evidence that one hint path is not sufficient for every learner.
   - A future learning engine should be able to switch representation rather than simply repeat the same hint.
   - Candidate progression: verbal/decomposition hint -> visual/concrete representation -> smaller prerequisite probe -> worked example -> re-attempt.

3. **Some children used their fingers to count and took more time.**
   - This should not automatically be classified as failure.
   - It is evidence about current strategy, fluency, and support level.
   - Future learner state should distinguish correct-independent-with-counting from fluent recall, rather than collapsing both into a binary correct/incorrect score.
   - Speed should not be treated as the primary learning outcome in this early-stage prototype.

4. **Grade 1 and Grade 2 currently receive the same questions.**
   - Confirmed limitation of Validation Prototype v0.1.
   - The grade selector currently records context but does not branch the maths sequence.
   - This was acceptable for the first prototype because v0.1 was designed to test one diagnostic-learning loop rather than curriculum coverage.
   - It is **not acceptable as the next validation version**, because Grade 1 and Grade 2 should not be treated as equivalent difficulty bands.

## Interpretation

### Early positive signal
The basic loop — attempt -> hint/diagnostic -> explanation -> practice -> independent check — appears understandable to many children.

### Early challenge
Some children need deeper or alternative scaffolding. This supports the Learning OS thesis that adaptation should change *how* a concept is represented, not merely show another question.

### Strategy signal
Finger counting and slow-but-correct performance should be captured as learning evidence. The system should eventually model:

- answer correctness;
- time taken only as context, not judgment;
- whether fingers/objects/counting were used;
- hints requested;
- representation that unlocked understanding;
- whether a later problem can be solved with less support.

## Required change for Validation Prototype v0.2

Create grade-aware maths paths.

### Grade 1 validation path
Focus on foundational subtraction in a smaller number range with concrete support available. Preserve problems around numbers to 20 and emphasize taking-away/counting/decomposition strategies.

### Grade 2 validation path
Move into two-digit number sense and subtraction situations, while still testing prerequisite repair when the child struggles. Include place-value-aware / two-digit subtraction rather than replaying the Grade 1 sequence unchanged.

The precise item set should be calibrated against the product's target curriculum and field-tested; grade should remain contextual rather than assuming every child has grade-level mastery.

## Product implication

**Grade determines the starting probe, not the ceiling or floor.**

A Grade 2 child who struggles with a Grade 1 prerequisite should be routed backward without stigma. A Grade 1 child who demonstrates mastery should be allowed to progress.

This preserves the project's core principle: **ability > grade label.**

## Evidence quality

These observations are direct field signals provided by the project owner but are currently aggregate and unquantified. They should be treated as stronger than synthetic/desk hypotheses, but weaker than a structured sample with session-level records.

Next step: revise the prototype to v0.2 with grade-aware starting probes and multi-level scaffolding, then continue validation.