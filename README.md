# LLM Wiki Pages

Concept and comparison pages for the llmwiki knowledge base.

## Contents

### Concept Pages (6)
| File | Description |
|------|-------------|
| `concepts/mixture-of-experts.md` | MoE architecture, key models, efficiency tradeoffs |
| `concepts/hybrid-attention-architectures.md` | CSA/HCA, SWA/GA, Mamba-3, DeltaNet-2, Nemotron 3 |
| `concepts/diffusion-language-models.md` | dLLMs as alternative to autoregressive generation |
| `concepts/benchmark-saturation.md` | Saturation crisis, contamination, new gold standards |
| `concepts/llm-agent-frameworks.md` | LangGraph, CrewAI, AutoGen, Claude Agent SDK, Pydantic AI |
| `concepts/llm-pricing-landscape.md` | API pricing, open-source TCO, cost-performance curves |

### Comparison Pages (4)
| File | Description |
|------|-------------|
| `comparisons/proprietary-vs-open-source-2026.md` | Coding, reasoning, cost, licensing, control |
| `comparisons/frontier-benchmark-comparison-2026.md` | HLE, SWE-bench, ARC-AGI-2, GPQA Diamond, AIME, BenchLM.ai |
| `comparisons/inference-engine-comparison.md` | vLLM, SGLang, TensorRT-LLM, Ollama, llama.cpp, LM Studio |
| `comparisons/code-assistant-comparison.md` | Cursor, Windsurf, Claude Code, Codex, Aider, Copilot, Cline, Continue |

## Local Installation

Clone into your llmwiki directory:

```bash
cd /Users/regancooney/llmwiki
git clone https://github.com/regancooney/llmwiki-pages.git .
```

Or copy individual directories:

```bash
cp -r llmwiki-pages/concepts /Users/regancooney/llmwiki/
cp -r llmwiki-pages/comparisons /Users/regancooney/llmwiki/
```

## Format

All pages use:
- YAML frontmatter (title, created, updated, type, tags, sources)
- Wikilinks (`[[page-name]]`) for cross-referencing
- Markdown tables for structured data
- Source attribution linking to raw research documents
