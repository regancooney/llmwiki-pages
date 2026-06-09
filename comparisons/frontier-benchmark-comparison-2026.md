---
title: "Frontier Benchmark Comparison (2026)"
created: 2026-06-09
updated: 2026-06-09
type: comparison
tags: [comparison, benchmark, frontier]
sources:
  - raw/papers/llmwiki-enrichment-2026.md
---

# Frontier Benchmark Comparison (2026)

Comprehensive leaderboard of frontier models across the major benchmarks as of June 2026.

## HLE (Humanity's Last Exam)

The hardest evaluation dataset: 2,500 expert-level questions across disciplines.

| Rank | Model | Score |
|------|-------|-------|
| 1 | Claude Mythos Preview | 64.7% |
| 2 | Claude Opus 4.8 | 57.9% |
| 3 | Gemini 3 Pro | 45.8% |
| 4 | Kimi K2 Thinking | 44.9% |
| 5 | GPT-5.5 Pro | 43.1% |

## SWE-bench Verified

Real-world software engineering tasks from open-source Python repositories.

| Rank | Model | Score |
|------|-------|-------|
| 1 | Claude Opus 4.8 | 88.6% |
| 2 | Claude Opus 4.7 | 87.6% |
| 3 | Claude Sonnet 4.6 | 82.0% |
| 4 | GLM-5.1 | 77.8% |
| 5 | Claude 4.5 Opus | 76.8% |

## ARC-AGI-2

Abstract reasoning and visual puzzle benchmark.

| Rank | Model | Score |
|------|-------|-------|
| 1 | GPT-5.5 Pro | 85.0% |

## GPQA Diamond

Graduate-level science questions (physics, chemistry, biology).

| Rank | Model | Score |
|------|-------|-------|
| 1 | GPT-5.4 Pro xhigh | 94.6% |
| 2 | Gemini 3.1 Pro | 94.1% |
| 3 | Claude Opus 4.8 | 93.6% |

## AIME 2025

Competition mathematics.

| Rank | Model | Score |
|------|-------|-------|
| 1 | Gemini 3 Pro | 100% |
| 1 | GPT 5.2 | 100% |

## BenchLM.ai Unified Rankings

Weighted average across 8 categories, covering 256+ models.

| Rank | Model | Unified Score |
|------|-------|---------------|
| 1 | Claude Mythos Preview | 99 |
| 2 | Claude Opus 4.8 | 95 |
| 3 | Gemini 3.1 Pro | 92 |
| 4 | GPT-5.5 | 91 |
| 5 | Qwen3.7 Max | 91 |

## Key Observations

- **Claude dominates coding and reasoning**: Anthropic holds the top spot on HLE, SWE-bench, and BenchLM.ai Unified.
- **GPT-5.5 Pro leads visual reasoning**: OpenAI's most expensive model excels at ARC-AGI-2.
- **Math is saturated at the top**: Both Gemini 3 Pro and GPT 5.2 achieve perfect scores on AIME 2025.
- **GPQA Diamond is nearly saturated**: Top models cluster within 1% at ~94%.

## Related Pages

- [[claude-opus-4-8]]
- [[gpt-5-5-pro]]
- [[gemini-2-5-ultra]]
- [[benchmark-saturation]]
- [[proprietary-vs-open-source-2026]]
