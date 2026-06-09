---
title: "LLM Pricing Landscape"
created: 2026-06-09
updated: 2026-06-09
type: concept
tags: [pricing, comparison, open-source, proprietary]
sources:
  - raw/papers/llmwiki-enrichment-2026.md
---

# LLM Pricing Landscape

API pricing for LLMs as of June 2026 shows a dramatic bifurcation: premium proprietary models command high per-token prices, while open-source models offer order-of-magnitude cost advantages, particularly for high-volume coding tasks.

## Proprietary API Pricing

| Model | Input ($/1M tokens) | Output ($/1M tokens) | Notes |
|-------|--------------------|--------------------|-------|
| Claude Opus 4.8 | $5.00 | $25.00 | Best coding/reasoning |
| GPT-5.5 | $5.00 | $30.00 | General purpose |
| GPT-5.5 Pro | $30.00 | $180.00 | Most expensive tier |
| GPT-5.2 | $1.50 | $14.00 | Cost-efficient proprietary |
| Claude Sonnet 4.6 | $3.00 | $15.00 | Sweet spot |
| Gemini 3.1 Pro | ~$2.00 | ~$12.00 | Competitive pricing |

## Open-Source TCO (Total Cost of Ownership)

Open-source models have no per-token cost when self-hosted, but incur infrastructure costs. The key comparison metric is cost-per-instance on coding benchmarks:

| Model | SWE-bench Score | Cost/Instance | License |
|-------|----------------|---------------|---------|
| MiniMax M2.5 | 75.8% | $0.07 | Proprietary (self-host) |
| Claude Opus 4.8 (API) | 88.6% | ~$0.75 | Proprietary API |
| DeepSeek-V4-Pro | ~Frontier | Self-host costs | MIT |

## Key Insight

**Cost-performance curves favor open-source for coding at scale.** MiniMax M2.5 achieves 75.8% on SWE-bench at $0.07/instance — roughly 10× cheaper than proprietary alternatives. For organizations running thousands of coding tasks daily, self-hosting open-source models can reduce costs by 10-50× compared to API calls.

## Related Pages

- [[proprietary-vs-open-source-2026]] — Full comparison
- [[minimax-m2-5]] — Cost leader
- [[deepseek-v4-pro]] — MIT-licensed frontier model
- [[vllm]] — Inference engine for self-hosting
