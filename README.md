# WebSword
Detects whether text was written by AI or a human, using simple writing-pattern signals.
Live: https://gitcoder12.github.io/Websword/


---

## AI-maintained project notes (secondary — 2026-11-13)

This section supplements the maintainer-authored README above. The original text has been restored verbatim from Git-history baseline `de875802850c5c01eb401d4331c1e8785a9e4c3d`; this addendum does not replace or certify the original claims.

- The current source tree, runtime data and tests are the implementation source of truth. Roadmap items, draft PRs and AI-generated descriptions are not shipped features by themselves.
- Preserve real and maintainer-provided data. Never silently substitute generated or placeholder data. Clearly label and isolate synthetic fixtures.
- Mark unverified sources, identifiers, metrics, benchmark results and external claims as unknown/unverified rather than guessing.
- Verify setup, execution, tests and public claims against the exact current commit before using this repository in a job, research or academic application.
- See [MODEL_AUDIT_ROUTER.md](MODEL_AUDIT_ROUTER.md) for independent model review instructions and the merge gate.

---

## Engineering Audit & Handover — 2026-11-17

**Reviewed commit:** `486ce28bd1579c0f5b890c798c604f47f976f802` (`main`).

### Confirmed findings
- The inspected `detectAI()` implementation calculates heuristic signals from text features such as vocabulary-length variance, sentence-length variance, transition phrases, hedging words, passive constructions, and repetition.
- The analysis flow includes a fixed delay to animate progress steps before calling the local heuristic function. No remote model inference or trained classifier was found in the inspected implementation.
- The resulting percentage/verdict is therefore a heuristic score, not a calibrated probability that text was written by AI. It can misclassify human and AI writing and should not be used for academic misconduct decisions.
- Scan history is stored in browser `localStorage`; it is local to that browser profile.

### Next actions
1. Rename/display the result as a heuristic indicator and remove probability/confidence claims unless calibrated on a representative benchmark.
2. Add a labelled evaluation corpus with false-positive/false-negative reporting across languages, domains, and edited text.
3. Add clear user-facing limitations and privacy controls for locally stored text history.

**Verification status:** static HTML/JavaScript inspection only; no detector benchmark or browser tests were run.

---

## Examples Used
- Comparing a human-written paragraph with AI-generated text
- Testing how paraphrasing changes writing-pattern signals
- Measuring false positives on edited human writing

---

## Repository navigation

[Alphabetical file index](FILE_INDEX.md)
