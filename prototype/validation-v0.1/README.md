# Kids Learning OS — Validation Prototype v0.1

**Purpose:** Test the core learning loop with parents and children before building the real product.

This is not a production app and not a diagnostic tool.

## What this prototype tests

1. Can a short interaction reveal *why* a child is stuck rather than only whether the answer is wrong?
2. Does changing the representation help?
3. Can support be reduced within one short session?
4. Can the child complete a new problem independently afterward?
5. Does the parent summary feel more useful than minutes/XP/streaks?
6. Does simple English / Telugu+English / Hindi+English code-switching feel natural enough to justify deeper language work?

## Scope

- Target: ages 6–8 / Grades 1–2
- Subject: foundational subtraction only
- Anchor problem: `14 − 8`
- Follow-up practice: `13 − 7`
- Independent check: `15 − 8`
- Interaction: touch + numeric input
- No backend
- No account
- No child name
- No microphone/camera
- No external AI/API calls
- No analytics or third-party tracking

## Privacy

The prototype runs entirely in the browser. Session state is stored only in browser `localStorage` so a family can resume on the same device. Nothing is uploaded anywhere.

## First anonymized field observations

Early direct use with children/parents produced these qualitative patterns:

- most children appeared to understand the hints;
- some children still struggled, indicating that one hint path is not enough for everyone;
- some children used their fingers to count and took more time;
- finger counting / slow correct performance should be treated as strategy and fluency evidence, not automatic failure.

Full notes are stored in `docs/06-user-research/direct-family-validation-v0.1-observations.md`.

## Known grade-path limitation

The Grade 1 and Grade 2 selectors currently lead to the **same subtraction sequence** (`14 − 8`, `13 − 7`, `15 − 8`).

This was intentional for v0.1 because the purpose was to validate the generic diagnosis → scaffold → independent-check loop rather than curriculum differentiation.

It should **not** remain this way in v0.2.

### Required v0.2 change

- Grade 1: start with smaller-range foundational subtraction and concrete support.
- Grade 2: start with two-digit/place-value-aware subtraction situations.
- Both paths must remain adaptive: route backward to prerequisites when needed and forward when mastery is demonstrated.

**Grade should select the starting probe; actual demonstrated ability should control the next step.**

## How to test

1. Parent selects grade and preferred explanation language.
2. Parent hands the device to the child.
3. Adult should avoid explaining unless the child is distressed or asks to stop.
4. Observe where the child hesitates, guesses, counts on fingers, asks for help, or understands immediately.
5. Let the prototype complete its own teaching sequence.
6. Review the parent summary at the end.
7. Interview the parent *after* the session using `docs/06-user-research/recruitment-and-interview-kit-v1.0.md`.

## What to record

Use `research/interview-tracker-template.csv` and note:

- first answer;
- whether the child understood the wording;
- where help was needed;
- strategy used (mental, finger counting, objects, counting back, decomposition, etc.);
- whether the representation helped;
- independent-check result;
- total session length;
- child frustration / boredom / confidence signals;
- parent interpretation of the summary;
- whether the parent would use the product in a real after-school situation.

## Important limitations

The branching logic is hand-authored and intentionally simple. A wrong answer does **not** prove a misconception. The parent summary uses language such as “signal” and “may need” rather than making educational or clinical diagnoses.

This prototype validates the *interaction model*, not the full Child Learning Model, AI architecture, curriculum coverage, or commercial product.