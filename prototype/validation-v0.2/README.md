# Kids Learning OS — Validation Prototype v0.2

**Status:** Grade-aware field-test prototype.  
**Target:** Ages 6–8 / Grades 1–2.  
**Purpose:** Test whether grade-aware starting points plus ability-aware stepping produce a more useful learning interaction than the single shared v0.1 subtraction flow.

## Why v0.2 exists

Early anonymized field observations from v0.1 showed:

- most tested children appeared to understand the provided hints;
- some children still struggled after hints;
- some children used finger counting and took additional time;
- Grade 1 and Grade 2 were receiving the same questions in v0.1.

No participant-identifying information or individual reviews are stored in the repository.

The important product correction is:

> **Grade chooses the starting point. Observed ability determines where the learning path goes next.**

## Curriculum rationale

Current India-first curriculum guidance supports different starting expectations:

- NIPUN Bharat describes Class I / age 6–7 numeracy around foundational counting and addition/subtraction in small-number daily-life situations.
- NIPUN Bharat describes Class II / age 7–8 numeracy using addition and subtraction up to two-digit numbers in daily-life situations.
- NCERT Class II learning outcomes explicitly include place value and subtraction involving two-digit numbers.

References:

- NIPUN Bharat Guidelines: https://www.education.gov.in/sites/upload_files/mhrd/files/nipun_bharat_eng1.pdf
- NCERT Class II Mathematics Learning Outcomes: https://ncert.nic.in/pdf/publication/otherpublications/tilops101.pdf
- National Curriculum Framework for Foundational Stage: https://www.ncert.nic.in/pdf/NCF_for_Foundational_Stage_20_October_2022.pdf

This prototype is not intended to reproduce a board syllabus chapter-by-chapter. It uses curriculum expectations only to choose developmentally sensible starting points.

## Grade 1 path

Starting problem: `8 − 3`

If support is needed:

1. prerequisite probe: `5 − 2`;
2. verbal/finger hint;
3. visual object/block hint;
4. concrete subtraction explanation.

Practice: `9 − 4`

Independent transfer check: `7 − 3`

The Grade 1 path deliberately accepts finger counting, object counting and slower response as valid strategies. The prototype records the strategy instead of treating speed as the goal.

## Grade 2 path

Starting problem: `34 − 8`

If support is needed:

1. prerequisite probe: `14 − 8`;
2. bridge-through-ten hint;
3. visual object hint if required;
4. rebuild the original two-digit problem using place-value reasoning.

Practice: `43 − 7`

Independent transfer check: `52 − 8`

If the Grade 2 child cannot yet solve the prerequisite, the system steps backward to concrete subtraction before returning to the grade-level problem.

## Strategy evidence

After the first problem, the child can report the strategy used:

- fingers;
- mental counting;
- breaking the number apart;
- remembered / just knew;
- drawing or imagining objects;
- not sure.

This is **self-report**, not proof of cognitive process. It is included to test whether strategy information makes the learner model and parent summary more useful.

## Time evidence

v0.2 records first-question time locally and displays it to the parent as context.

Time is explicitly **not scored**. A slower correct answer may reflect a valid developing strategy rather than weak understanding.

## Privacy

- no backend;
- no account;
- no child name;
- no camera or microphone;
- no analytics;
- no external AI calls;
- no participant-identifying data in Git.

Browser-local state only.

## What v0.2 tests

1. Does grade-aware starting difficulty feel more appropriate?
2. Does ability-aware stepping backward reduce frustration for a Grade 2 child with a prerequisite gap?
3. Are multiple hint levels more useful than a single hint?
4. Is finger counting / strategy information useful to parents and product decisions?
5. Can a child move from support to an independent transfer item?
6. Does the parent summary communicate *how* the child solved, not merely whether the child was correct?

## What v0.2 still does not prove

It does not validate:

- the full Child Learning Model;
- long-term retention;
- curriculum coverage;
- willingness to pay;
- AI tutoring quality;
- reading/language learning;
- production UX;
- medical, developmental or psychological conclusions.
