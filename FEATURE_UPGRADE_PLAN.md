# Websword — Feature Upgrade Plan

## Objective

A browser tool that examines writing patterns and shows heuristic signals that may be associated with AI-generated text.

## P0 — validity and honest claims

- [ ] Document the exact features and scoring logic; distinguish measured linguistic features from unsupported model-authorship claims.
- [ ] Add unit tests for empty text, unicode, short passages, long passages and adversarially edited text.

## P1 — explainable user workflow

- [ ] Expose individual feature signals and uncertainty rather than a single authoritative verdict.
- [ ] Add reproducible fixtures and compare heuristic output to a labelled, appropriately licensed dataset.

## P2 — research quality

- [ ] Evaluate calibration, subgroup error and robustness to paraphrasing and mixed human/AI text.
- [ ] Add a clear report that explains why detection is uncertain and discourages high-stakes use.

## Collaborator work packages

1. Feature extraction specification and deterministic tests.
2. Dataset curation, licences, labels and provenance.
3. Calibration and robustness evaluation.
4. Plain-language result explanation and risk/limitations review.

## Definition of done

- [ ] The app describes output as heuristic signals, not proof of authorship.
- [ ] Tests cover empty, short, long, unicode and adversarial inputs.
- [ ] Evaluation dataset and method are reproducible.
- [ ] Error rates and uncertainty are visible before publishing performance claims.
