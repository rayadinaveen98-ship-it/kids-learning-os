# Kids Learning OS — Prototype Flow v0.1

**Date:** 2026-09-11  
**Status:** Low-fidelity validation flow  
**Purpose:** Test the core learning loop before building a polished UI.

---

# 1. Scenario

Child: age 7, Grade 2.  
Parent says: “She keeps getting 14 - 8 wrong.”

The prototype must determine whether the child actually lacks subtraction skill or whether another prerequisite/representation issue is causing the error.

---

# 2. Parent entry

Parent opens the app and sees three simple choices:

1. **My child is stuck**
2. **Do today’s short session**
3. **See what my child is learning**

For this prototype, choose **My child is stuck**.

Parent can enter:

- topic manually;
- a simple problem;
- later: homework photo.

Example input:

> 14 - 8

The parent then hands the phone to the child.

---

# 3. Child handoff

Child screen should not say:

> Assessment

or:

> You got this wrong.

Instead:

> “Let’s figure this out together.”

The session shows one clear activity at a time.

---

# 4. Diagnostic step A — understand the operation

Prompt:

> “You have 14 mangoes and give away 8. Do you have more mangoes or fewer mangoes now?”

Purpose:

- check subtraction meaning;
- distinguish operation confusion from arithmetic difficulty.

If child answers “more,” the system should repair operation meaning before numerical strategy.

---

# 5. Diagnostic step B — number sense around ten

Prompt:

> “How many do we take away from 14 to reach 10?”

Possible evidence:

- answers 4 quickly → likely understands decomposition;
- counts laboriously → strategy not fluent;
- answers incorrectly → number-bond gap;
- cannot follow wording → language/comprehension issue.

---

# 6. Diagnostic step C — representation switch

Show 14 counters split as:

`10 + 4`

Ask:

> “If we need to take away 8, what could we remove first?”

Observe whether the child can use the visible structure.

---

# 7. Intervention path examples

## Path 1 — operation confusion

Use a physical give-away story and objects.

## Path 2 — number-bond weakness

Practice composing/decomposing 10 briefly.

## Path 3 — symbolic-only difficulty

Use counters/number line first, then return to symbols.

## Path 4 — language confusion

Rephrase in the child’s stronger language while retaining school vocabulary.

## Path 5 — one-off slip

Do not over-teach. Give one parallel check and move on.

---

# 8. Teaching interaction

Example strategy: make 10.

The child sees 14 as:

`10 + 4`

Guide:

1. take away 4 to reach 10;
2. still need to take away 4;
3. 10 - 4 = 6.

Do not immediately give the final answer. Let the child perform each step.

---

# 9. Scaffold fade

### Supported problem

13 - 7

System provides a visual split.

### Hint-only problem

15 - 8

System asks:

> “What number could you reach first?”

### Independent problem

12 - 7

No visual/hint unless requested.

The point is not repetition volume. It is evidence that support can decrease.

---

# 10. Explain-back

Ask:

> “Can you tell me how you solved it?”

The child may answer by:

- voice;
- choosing steps;
- moving counters;
- drawing.

The system should accept multiple valid representations.

This is useful evidence of understanding but should not become a language-performance trap.

---

# 11. Session stop

After one objective is reached:

> “Nice work. We’re done for today.”

No autoplay.

No:

> “Keep playing to earn 100 more coins.”

Optionally give a tiny offline mission:

> “Later, try this with 14 buttons or coins at home.”

---

# 12. Parent handback

Parent receives a short summary:

## What was happening

> Your child understands subtraction, but crossing 10 was causing confusion.

## What helped

> Breaking 14 into 10 + 4 made the idea clear.

## Evidence today

> Solved 12 - 7 independently after support was removed.

## What next

> No more work tonight. We’ll check a similar problem tomorrow to see if it stayed learned.

## Parent action

> None needed tonight.

---

# 13. Next-day retention check

The next session begins with one short unseen equivalent problem.

If successful:

Mastery state can move from:

`supported -> independent -> retained`

If unsuccessful:

Do not punish/reset. Reopen the concept with a different representation.

---

# 14. What this prototype is testing

Not visual polish.

We are testing:

- will the child tolerate a diagnostic loop before teaching?
- can the flow identify a useful cause of the error?
- does changing representation help?
- can hints be reduced?
- can the child solve a new problem independently?
- does the parent understand the final report?
- does the parent feel this saved time or gave clarity?
- does the child feel helped rather than judged?

---

# 15. Prototype variants

### Variant A — Touch first
Minimal voice, visual counters and taps.

### Variant B — Voice guided
Tutor speaks prompts and accepts short spoken answers.

### Variant C — Code-switched
Same flow with familiar-language explanation + English school terminology.

### Variant D — Physical-world
Use real coins/buttons for the teaching step.

These variants should be tested separately rather than bundled into one complicated prototype.

---

# 16. Prototype success signal

A prototype session is promising when:

1. the inferred learning gap is useful;
2. child frustration stays low;
3. support decreases during the session;
4. child succeeds independently on a changed problem;
5. parent can accurately explain what the child learned after seeing the report;
6. parent says they would use the flow in a real recent situation rather than only saying it is “nice.”
