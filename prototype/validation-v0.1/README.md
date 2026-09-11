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

## How to test

1. Parent selects grade and preferred explanation language.
2. Parent hands the device to the child.
3. Adult should avoid explaining unless the child is distressed or asks to stop.
4. Observe where the child hesitates, guesses, asks for help, or understands immediately.
5. Let the prototype complete its own teaching sequence.
6. Review the parent summary at the end.
7. Interview the parent *after* the session using `docs/06-user-research/recruitment-and-interview-kit-v1.0.md`.

## What to record

Use `research/interview-tracker-template.csv` and note:

- first answer;
- whether the child understood the wording;
- where help was needed;
- whether the representation helped;
- independent-check result;
- total session length;
- child frustration / boredom / confidence signals;
- parent interpretation of the summary;
- whether the parent would use the product in a real after-school situation.

## Important limitations

The branching logic is hand-authored and intentionally simple. A wrong answer does **not** prove a misconception. The parent summary uses language such as “signal” and “may need” rather than making educational or clinical diagnoses.

This prototype validates the *interaction model*, not the full Child Learning Model, AI architecture, curriculum coverage, or commercial product.