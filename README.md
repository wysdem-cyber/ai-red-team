# ai-red-team

Applied AI security research: adversarial testing, vulnerability documentation, and evaluation work on open-source LLMs.

## About

This repo documents hands-on red-teaming and evaluation work against open-source language models prompt injection testing, jailbreak resistance comparisons, and custom eval design. Each project follows a consistent format: methodology, reproducible test cases, results, and mitigation notes.

Background: cybersecurity student building toward AI evaluation / AI safety / red-teaming roles. Tooling used across projects includes `garak`, `promptfoo`, and the HuggingFace ecosystem.

## Projects

| Project | Focus | Status |
|---|---|---|
| [01 — Prompt Injection Audit](./01-prompt-injection-audit) | Direct & indirect injection testing against open-source instruct models | 🔧 In progress |
| [02 — Jailbreak Resistance Comparison](./02-jailbreak-comparison) | Scored comparison of jailbreak techniques across multiple models | ⏳ Planned |
| [03 — RAG Attack Report](./03-rag-attack-report) | Indirect prompt injection via poisoned documents in a RAG pipeline | ⏳ Planned |
| [04 — Custom Eval Suite](./04-custom-eval-suite) | Test suite measuring a specific failure mode (e.g. refusal consistency, PII leakage) across models | ⏳ Planned |

*(Table updates as each project ships see individual project folders for full write-ups.)*

## Structure

```
ai-red-team/
├── 01-prompt-injection-audit/
│   ├── README.md          # methodology, payloads, results, mitigations
│   ├── payloads/           
│   └── results/
├── 02-jailbreak-comparison/
├── 03-rag-attack-report/
├── 04-custom-eval-suite/
└── README.md               # this file
```

Each project folder is self-contained with its own README covering:
- **Methodology** — what was tested and why
- **Test cases** — payloads/prompts used, versioned
- **Results** — pass/fail data, tables, or scoring
- **Mitigations** — how the underlying issue could be addressed

## Tools

- `garak` — LLM vulnerability scanning
- `promptfoo` — prompt/output evaluation
- HuggingFace `transformers` — model loading and inference
- Python 3.11+

## Disclosure

Any genuine, reproducible vulnerabilities found in the course of this work are documented per responsible disclosure practices. No live production systems are targeted all testing is against openly available models and self-hosted pipelines.

## Contact

Open to AI evaluation, AI safety, and red-teaming opportunities feel free to reach out via
https://www.linkedin.com/in/emmanuella-e-a-lewis-sottie-9a6575313/.
