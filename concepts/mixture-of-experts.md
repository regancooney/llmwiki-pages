---
title: "Mixture-of-Experts (MoE)"
created: 2026-06-09
updated: 2026-06-09
type: concept
tags: [architecture, moe, efficiency]
sources:
  - raw/papers/llmwiki-enrichment-2026.md
---

# Mixture-of-Experts (MoE)

Mixture-of-Experts has become the standard architecture for every frontier model in 2026. The core pattern: massive total parameter counts (400B-2T) combined with small active subsets (13B-49B parameters), achieving high capability at manageable inference cost.

## Key Models

| Model | Total Params | Active Params | Experts |
|-------|-------------|--------------|---------|
| DeepSeek-V4-Pro | 1.6T | 49B | — |
| Mistral Large 3 | 675B | 41B | — |
| MiMo-V2.5-Pro | 1.02T | 42B | — |
| Llama 4 Maverick | 400B | 17B | 128 |
| Qwen 3.5 | 397B | 17B | — |

## Efficiency Frontier

Step 3.5 Flash achieves frontier-level performance at only 11B active parameters, demonstrating the extreme efficiency gains possible with modern MoE routing strategies. This model shows that MoE can deliver competitive results at a fraction of the compute cost of dense models.

## Tradeoffs

- **Routing Overhead**: Expert selection and load balancing add complexity during both training and inference.
- **Compute Savings**: Only a small fraction of total parameters are activated per token, dramatically reducing FLOP requirements.
- **Memory Requirements**: Despite sparse activation, the full model must reside in memory (or be efficiently paged), creating deployment challenges for the largest models.
- **Training Stability**: Load imbalance across experts can lead to under-utilization and training instability.

## Industry Adoption

MoE is no longer experimental — every major frontier model released in 2026 uses it. The combination of MoE with hybrid attention architectures (see [[hybrid-attention-architectures]]) and improved inference engines (see [[llm-pricing-landscape]]) has made trillion-parameter models economically viable for API serving.

## Related Pages

- [[deepseek-v4-pro]] — DeepSeek's 1.6T MoE flagship
- [[llama-4-5]] — Meta's 400B/17B MoE model
- [[hybrid-attention-architectures]] — Complementary efficiency innovations
- [[llm-pricing-landscape]] — How MoE affects API costs
