---
title: "Proprietary vs Open-Source LLMs (2026)"
created: 2026-06-09
updated: 2026-06-09
type: comparison
tags: [comparison, open-source, proprietary, pricing]
sources:
  - raw/papers/llmwiki-enrichment-2026.md
---

# Proprietary vs Open-Source LLMs (2026)

Head-to-head comparison of proprietary and open-source LLMs across key dimensions as of June 2026.

## Coding

| Model | SWE-bench Verified | Type |
|-------|-------------------|------|
| Claude Opus 4.8 | 88.6% | Proprietary |
| DeepSeek-V4-Pro | ~Frontier (~Frontier) | Open-Source (MIT) |
| Claude Sonnet 4.6 | 82.0% | Proprietary |
| GLM-5.1 | 77.8% | Open-Source |
| MiniMax M2.5 | 75.8% | Open-Source |

**Verdict**: The coding gap has effectively closed. Open-source models are within striking distance of proprietary leaders, and at dramatically lower cost.

## Reasoning

| Model | HLE Score | Type |
|-------|----------|------|
| Claude Opus 4.8 | 57.9% | Proprietary |
| Kimi K2 Thinking | 44.9% | Open-Source |
| GPT-5.5 Pro | 43.1% | Proprietary |

**Verdict**: Proprietary models maintain a significant lead on the hardest reasoning benchmarks (HLE). The best open-source model trails by ~13 percentage points.

## Cost

| Model | SWE-bench | Cost/Instance | Type |
|-------|----------|---------------|------|
| MiniMax M2.5 | 75.8% | $0.07 | Open-Source |
| Claude Opus 4.8 | 88.6% | ~$0.75 | Proprietary |

**Verdict**: Open-source wins dramatically on cost. 10× cheaper per coding instance, with the gap widening at scale.

## Licensing

- **Open-Source (MIT/Apache 2.0)**: Full control, self-hosting, modification, commercial use. Examples: DeepSeek-V4-Pro (MIT), Llama 4 (Llama Community License).
- **Proprietary API**: Usage-bound, subject to rate limits, terms of service, and provider availability risk.

## Control

- **Self-Hostable**: Full data sovereignty, no external dependencies, fixed infrastructure costs.
- **API-Dependent**: Vendor lock-in, latency variability, privacy concerns for sensitive data.

## Key Trend

The gap is closing fastest in **coding** (within 5-10%), and slowest in **frontier reasoning** (13%+ gap). For coding-heavy workloads at scale, open-source is already the economically rational choice.

## Related Pages

- [[claude-opus-4-8]]
- [[deepseek-v4-pro]]
- [[minimax-m2-5]]
- [[llm-pricing-landscape]]
- [[frontier-benchmark-comparison-2026]]
