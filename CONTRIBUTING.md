# Contributing to Websword

## Improving Detection
- Detection logic lives in the classifier section of `index.html`
- Add new heuristics as scored features (0–1 range each)
- Document what each feature detects and why

## Heuristic Categories
- Lexical: vocabulary diversity, rare word usage
- Syntactic: sentence length variance, clause depth
- Semantic: topic coherence, transition patterns
- Statistical: perplexity proxies, burstiness
