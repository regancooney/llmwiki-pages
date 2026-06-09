---
title: "Diffusion Language Models (dLLMs)"
created: 2026-06-09
updated: 2026-06-09
type: concept
tags: [architecture, inference, diffusion, emerging]
sources:
  - raw/papers/llmwiki-enrichment-2026.md
---

# Diffusion Language Models (dLLMs)

Diffusion Language Models represent the most significant alternative to autoregressive generation to emerge in 2025–2026. Instead of generating tokens sequentially left-to-right, dLLMs use discrete diffusion processes that iteratively refine text from noise — analogous to how image diffusion models (Stable Diffusion, DALL-E) generate pixels.

## How They Work

Traditional autoregressive models generate one token at a time, each conditioned on all previous tokens. Diffusion models start with a fully masked or noisy sequence and iteratively "unmask" or refine tokens over multiple steps, allowing parallel generation.

Key paper: *Discrete Diffusion for Text as a Competitive Alternative* (arXiv:2602.22661) demonstrated that discrete diffusion can match autoregressive quality while enabling parallel decoding.

## Key Models

- **Mercury**: One of the first commercially available dLLMs, demonstrating the approach at scale.
- **LLaDA**: An open research model exploring diffusion-based language generation.
- **Together AI Consistency DLMs**: Achieves up to 14× faster inference compared to autoregressive models of comparable quality by reducing the number of diffusion steps.

## Advantages

- **Parallel Generation**: Multiple tokens can be generated simultaneously, dramatically reducing latency.
- **Bidirectional Context**: Diffusion naturally considers both past and future context during refinement.
- **Iterative Refinement**: The model can revisit and improve earlier decisions, unlike autoregressive models.

## Current Status

Still emerging — not yet the production standard. While research progress is rapid and inference speed advantages are compelling, autoregressive models remain dominant for most deployed systems. The primary challenges include training stability at scale and matching the quality ceiling of the best autoregressive models.

## Related Pages

- [[mixture-of-experts]] — Current dominant architecture
- [[hybrid-attention-architectures]] — Complementary efficiency innovations
- [[benchmark-saturation]] — How new models are evaluated
