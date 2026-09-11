# India Privacy, Safety & Operating Constraints (v0.4)

**Date:** 2026-09-11  
**Scope:** India-first product constraints for a learning product serving children roughly ages 4–8.

---

## Executive conclusion

For a children’s AI learning product in India, privacy and safety cannot be bolted on after growth. They directly constrain identity, analytics, personalisation, voice/camera features, notifications, monetisation, parent consent, retention mechanics and model design.

The safest strategic position is stricter than the minimum legal baseline:

> collect less, infer less, retain less, expose less, and make parent control obvious.

---

## 1. India’s DPDP framework is directly relevant

The Digital Personal Data Protection Act, 2023 and DPDP Rules, 2025 create special obligations for children’s personal data.

Important provisions include:

- verifiable parental/guardian consent before processing a child’s personal data, subject to prescribed exemptions;
- prohibition on processing likely to cause detrimental effects on child well-being;
- prohibition on tracking or behavioural monitoring of children and targeted advertising directed at children, subject to limited statutory exemptions;
- rights around access, correction, update and erasure;
- operational rules for verifying the adult providing consent.

The final DPDP Rules were notified in November 2025 with phased implementation timelines.

### Sources

- MeitY DPDP Act 2023: https://www.meity.gov.in/static/uploads/2024/02/Digital-Personal-Data-Protection-Act-2023.pdf
- MeitY DPDP Rules 2025: https://www.meity.gov.in/documents/act-and-policies/digital-personal-data-protection-rules-2025-gDOxUjMtQWa
- PIB summary: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2190014&lang=2&reg=3
- PIB student-platform note: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2202901&lang=2&reg=48

---

## 2. Product implication: parent account first

For ages 4–8, the default identity architecture should probably be:

`Parent/guardian account -> child profile(s)`

rather than giving the child a standalone email/mobile identity.

Child profile should use minimum necessary identifiers.

Possible minimum:

- nickname/display name;
- age or birth month/year where genuinely necessary;
- school grade/stage;
- language preferences;
- learning state.

Avoid collecting unless necessary:

- exact address;
- child phone number;
- child email;
- precise GPS;
- social graph;
- advertising identifiers;
- unnecessary face images;
- continuous audio recordings.

---

## 3. Child personalisation must not become behavioural advertising

The product may need behavioural learning data to adapt instruction, but that data must be tightly purpose-bound to education and safety.

We should explicitly prohibit internally:

- ad targeting;
- sale of child profiles;
- cross-app advertising IDs;
- commercial interest profiles;
- manipulation based on emotional vulnerability;
- using learning weakness to upsell the parent.

Example of unacceptable product logic:

> “Child repeatedly struggles with reading -> show parent urgent premium upgrade.”

Better:

> “Child repeatedly struggles with decoding -> explain observation neutrally; offer the same learning support rules regardless of subscription status where safety/essential feedback is concerned.”

---

## 4. Voice is useful but sensitive

Voice can dramatically improve access for ages 4–8 because typing and reading are limited.

Potential benefits:

- oral reading assessment;
- pronunciation practice;
- story retelling;
- verbal math reasoning;
- home-language interaction;
- accessibility.

But microphone data creates privacy and household risks.

### Default design principles

- microphone activates only during a clearly visible interaction;
- no passive/background listening;
- provide an obvious microphone indicator;
- process locally/on-device where feasible for simple recognition;
- if cloud processing is required, explain it to the parent;
- do not retain raw child audio by default if derived features are sufficient;
- if raw audio is retained for a specific feature, use short retention and explicit consent;
- allow parent to disable voice entirely.

---

## 5. Camera should be optional, purpose-specific and rare

Potential educational uses:

- photograph homework;
- capture a drawing/project;
- recognise physical objects in a supervised activity;
- document completion of an off-screen mission.

Risks:

- accidental capture of family members/home;
- location clues;
- biometric implications;
- background personal information;
- child misunderstanding of when camera is active.

### Default rule

No always-on vision. Camera opens only after a deliberate parent/child action tied to a named task.

For many activities, a child’s verbal confirmation or simple tap should be enough; do not require proof-of-completion photos merely to create more data.

---

## 6. AI safety boundary

The child-facing agent should be **task-bounded**.

Allowed domains can include:

- curriculum explanation;
- age-appropriate curiosity questions;
- stories/creative learning;
- guided reasoning;
- safe everyday knowledge.

High-risk topics should invoke tightly designed responses and adult escalation.

The system should never pretend to be:

- a doctor;
- therapist;
- emergency service;
- secret confidant against caregivers;
- human friend who “needs” the child.

UNICEF’s 2025/2026 work specifically warns that conversational and companion-like AI can create distinct relational and privacy risks for children.

Sources:
- https://www.unicef.org/innocenti/reports/policy-guidance-ai-children
- https://www.unicef.org/documents/when-ai-becomes-friend-child-rights-risks

---

## 7. Parent visibility should be meaningful, not surveillance

Parent trust does not require streaming every word a child says.

A better default is meaningful summaries:

- what concept was practised;
- what the child could do independently;
- what support was needed;
- what should be revisited;
- any safety-relevant event requiring parent attention.

Avoid turning the parent dashboard into a transcript-monitoring console unless a specific child-safety reason requires review.

Privacy should protect the child too.

---

## 8. Notifications should target the parent, not manipulate the child

For ages 4–8, push-notification growth loops can easily become coercive.

Avoid child-directed notifications like:

> “Milo misses you!”
> “Your streak will die!”
> “Come back to earn a rare pet!”

Parent-facing reminders can instead be utilitarian:

> “Today’s 10-minute reading activity is ready.”

or

> “This week Aarav became independent with addition within 10.”

No guilt, loss-aversion or synthetic attachment.

---

## 9. Monetisation constraints

Recommended constitution:

- no advertising in child mode;
- no targeted ads anywhere using child data;
- no loot boxes;
- no premium currency;
- no randomised rewards tied to money;
- no child-facing purchase UI;
- no “ask your parent to buy this” messaging;
- parent-only subscription management;
- transparent renewal/cancellation;
- no fear-based upsell around learning gaps.

This is both a trust strategy and a safety strategy.

---

## 10. Analytics constraints

Traditional consumer-product analytics often optimise retention through granular behavioural tracking. For children, the safer model is purpose-limited product/learning analytics.

Useful aggregated events may include:

- session completed;
- activity type;
- concept attempted;
- hint count;
- independent success;
- crash/performance metrics.

Avoid unnecessary event streams containing:

- raw free-form child speech;
- exact typed content unrelated to learning;
- precise location;
- persistent cross-service tracking IDs.

Analytics should be designed from the learning question backward, not collected “in case useful later.”

---

## 11. Shared-phone safety

Because many Indian children use a parent’s phone, parent and child surfaces must be clearly separated.

Potential requirements:

- parent gate for purchases/settings/data controls;
- child cannot access parent account details;
- parent notifications do not appear as child rewards;
- switching out of child mode should not expose sensitive learning notes accidentally;
- offline downloaded child content should be encrypted/appropriately sandboxed where needed;
- multiple sibling profiles should not leak one child’s progress to another.

---

## 12. Data retention policy should be explicit from V1

Proposed default philosophy:

- raw media: shortest practical retention;
- derived learning signals: retained only while useful for learning continuity;
- inactive account cleanup;
- parent-accessible delete control;
- account deletion cascades to child profiles;
- documented backup deletion schedule;
- separate research opt-in if anonymised data is ever used for educational research.

Do not make “training our AI” a blanket purpose for collecting child data.

---

## 13. Model-training policy

Recommended default:

> Child conversations, voice, photos and learning records are **not used to train general-purpose foundation models** by default.

If any future product improvement relies on child data:

- use de-identified/aggregated data where possible;
- isolate purpose;
- obtain explicit appropriate consent;
- publish understandable documentation;
- conduct internal child-safety/privacy review.

This should become a brand promise if technically sustainable.

---

## 14. Safety testing requirements before public launch

Before shipping an AI child interface, red-team at minimum:

- harmful content requests;
- sexual content;
- self-harm language;
- violence;
- bullying;
- secrecy from parents;
- attempts to obtain personal information;
- requests for exact location/contact details;
- unsafe physical experiments;
- medical advice;
- emotional dependency prompts;
- jailbreaking/prompt injection;
- hallucinated school facts;
- false claims presented confidently;
- direct homework-answer extraction.

Safety testing must include Indian-language and code-switched prompts, not English only.

---

## 15. Accessibility and inclusion

India-first design should consider:

- low-end Android performance;
- intermittent connectivity;
- small phone screens;
- audio in noisy homes;
- children who are not fluent readers;
- multiple Indian scripts;
- left-handed drawing/tracing interactions;
- motor/vision/hearing accessibility;
- parent literacy variation.

A premium visual experience that requires a high-end tablet would exclude much of the market.

---

## 16. Regulatory interpretation rule

This repository records product implications, not legal advice.

Before launch, obtain professional Indian privacy/legal review covering:

- DPDP applicability and implementation date;
- parental consent flow;
- educational exemptions if any;
- processor/vendor contracts;
- international data transfer;
- data breach procedures;
- app-store children/family policies;
- voice/image biometric implications;
- future school deployments.

---

## Safety constitution — current research recommendation

1. Child mode never sells.
2. No ads.
3. No infinite feed.
4. No attachment manipulation.
5. No background microphone/camera.
6. No unrestricted open-web browsing by young children.
7. No general model training on child data by default.
8. Parent controls all data/purchase settings.
9. Data collection must have an educational/safety purpose.
10. AI should be a teacher/tool, not a replacement relationship.
11. Safety must work in Indian languages and code-switching.
12. A child should become more independent over time, not more dependent on the product.
