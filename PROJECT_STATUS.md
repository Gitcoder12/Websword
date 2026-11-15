# Project Status — Websword

**Snapshot date:** 2026-11-16  
**Status type:** Initial documentation and repository-tree assessment  
**Default branch:** main  
**Review completeness:** Partial — not a code audit or release certification

## Project purpose
Minimal web page/project described as detecting whether text was written by AI or a human using writing-pattern signals.

## Current maturity (README-declared or visible scaffolding; not independently verified)
README has a one-line purpose and a live GitHub Pages URL; top-level tree shows a single index.html plus standard project files.

## Observed repository structure
.env.example, index.html, README.md and repository guidance/license files.

## Known issues and risks to investigate
AI-text detection is probabilistic and prone to false positives/false negatives; README does not document model/method, training/evaluation data, calibration or limitations. No tests or benchmark evidence visible in the root listing. Never market results as proof of authorship or academic misconduct.

## Recommended next actions
Inspect implementation and live demo; document the actual signal/algorithm and its limits; add evaluation on diverse human/LLM text with false-positive and false-negative reporting; add clear warning that outputs are not conclusive evidence; test Unicode, short texts and paraphrased content.

## Verification record
| Check | Result |
|---|---|
| Default-branch top-level tree | Inspected |
| README | Inspected |
| Deep source review | Not performed |
| Tests / build / runtime | Not run |
| Security / dependency audit | Not run |
| Live deployment / API checks | Not run |
| Independent review | Not performed |

## Change log
- 2026-11-16: Added this initial status snapshot on a review branch. No application code or existing data changed.

> Update this file only after the corresponding inspection or verification has actually been performed. Distinguish observed facts, README claims, hypotheses and unrun checks.