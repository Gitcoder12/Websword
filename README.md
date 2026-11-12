# WebSword

**A browser-based text-style analyser that estimates AI-like writing signals.**

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://gitcoder12.github.io/Websword/)
[![License](https://img.shields.io/badge/license-see%20LICENSE-lightgrey)](LICENSE)

WebSword is a lightweight, single-page experiment for examining text patterns that may be associated with machine-generated or human-written content.

## Features

- Paste text into a browser interface for analysis.
- Inspect heuristic writing-pattern signals.
- View an estimated result without installing a backend service.
- Run as a static page.

## Quick Start

Open `index.html` in a modern browser, or serve the repository locally:

```bash
git clone https://github.com/Gitcoder12/Websword.git
cd Websword
python -m http.server 8000
```

Open `http://localhost:8000`.

## Tech Stack

HTML · CSS · JavaScript

## Scope and Limitations

WebSword's output is a heuristic estimate, not a reliable authorship determination. AI detectors can produce false positives and false negatives, especially for short, edited, translated, or non-native writing. Do not use this tool as the sole basis for academic, employment, disciplinary, or other high-impact decisions.

## License

See [LICENSE](LICENSE).
