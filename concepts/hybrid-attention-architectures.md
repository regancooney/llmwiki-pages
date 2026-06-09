---
title: "Hybrid Attention Architectures"
created: 2026-06-09
updated: 2026-06-09
type: concept
tags: [architecture, attention, long-context, efficiency]
sources:
  - raw/papers/llmwiki-enrichment-2026.md
---

# Hybrid Attention Architectures

The standard transformer self-attention mechanism is being systematically augmented — and in some cases replaced — by more efficient alternatives. By mid-2026, hybrid architectures combining multiple attention mechanisms have become the norm for frontier models, driven by the need to handle context windows exceeding 1 million tokens.

## Key Approaches

### DeepSeek V4 CSA/HCA
DeepSeek's Compressed Sparse Attention (CSA) and Heavily Compressed Attention (HCA) reduce the KV-cache to approximately 10% of the standard transformer at 1M token context lengths. This is achieved through aggressive compression of historical key-value pairs while maintaining fidelity on recent tokens.

### MiMo-V2.5 SWA/GA
MiMo combines Sliding Window Attention (SWA) with Global Attention (GA) at a 6:1 ratio, achieving a 7× reduction in KV-cache size. Sliding windows capture local context efficiently while global attention ensures long-range dependencies are not lost.

### Mamba-3 State-Space Models
Third-generation state-space models (SSMs) have matured into practical building blocks. Mamba-3 powers key components in Nemotron 4 and Qwen 4, offering linear-time sequence processing as an alternative to quadratic attention.

### Gated DeltaNet-2
An evolution of linear attention with decoupled erase and write operations. This allows the model to selectively forget and update information in its recurrent state, improving long-context retention.

### Nemotron 3 Production Hybrid
NVIDIA's Nemotron 3 alternates standard attention layers with Mamba-2 layers in production, combined with NVFP4 quantization. This hybrid approach balances the representational power of attention with the efficiency of SSMs.

## Why Hybrid?

The core insight driving hybrid architectures: no single attention mechanism is optimal for all sequence positions. Local context benefits from sliding windows; long-range dependencies need global attention; and linear-time alternatives like SSMs excel at very long sequences. Hybrid architectures compose these mechanisms to get the best of each.

## Related Pages

- [[deepseek-v4-pro]] — CSA/HCA pioneer
- [[mimo-v2-5-pro]] — SWA/GA implementation
- [[mixture-of-experts]] — Complementary efficiency pattern
- [[diffusion-language-models]] — Alternative generation paradigm
