# Validation Prototype v0.2 — Deployment

**Status:** Live for field validation  
**Date:** 2026-09-12  
**Host:** Vercel Hobby

## Canonical public URL

https://kids-learning-os-validation.vercel.app

## Vercel metadata

- Project: `kids-learning-os-validation`
- Project ID: `prj_1HaQn69au93obeFA3oDCyJ714box`
- Deployment ID: `dpl_CPEMywuHER9bTjF75b4n8dCFfE1M`
- Deployment target: `production`
- Deployment state at verification: `READY`
- Canonical alias: `kids-learning-os-validation.vercel.app`
- Secondary alias: `kids-learning-os-validation-navin7.vercel.app`

## Verification performed

The production deployment was queried through the connected Vercel account and returned `READY` with no alias error.

The canonical URL was fetched successfully and returned HTTP `200 OK` with HTML identifying itself as `Validation v0.2`.

Static inspection of the live code confirmed the grade-aware branch:

- Grade 1 initial question: `8 − 3`
- Grade 2 initial question: `34 − 8`

The live code also contains separate Grade 1 and Grade 2 diagnostic, practice and independent-transfer questions, plus strategy capture and two hint levels.

This confirms deployment and grade branching in the served code. It does **not** replace manual end-to-end interaction testing on real devices.

## Privacy characteristics

The hosted validation page contains:

- no account system;
- no child name field;
- no analytics SDK;
- no backend database;
- no microphone or camera access;
- no external AI calls;
- no advertisements;
- no child-facing monetization.

Session values exist only in page runtime for the hosted field-test build.

## v0.1 relationship

`prototype/validation-v0.1/` remains preserved as the historical first validation instrument.

The canonical Vercel URL now points to **v0.2** and should be used for new field sessions.

## Field-test rule

Use the page only as a product-learning instrument. It is not an educational assessment, clinical diagnostic, or validated learning intervention.
