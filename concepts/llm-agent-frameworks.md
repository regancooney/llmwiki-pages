---
title: "LLM Agent Frameworks"
created: 2026-06-09
updated: 2026-06-09
type: concept
tags: [agent, framework, orchestration]
sources:
  - raw/papers/llm-tools-overview.md
  - raw/papers/llmwiki-enrichment-2026.md
---

# LLM Agent Frameworks

The agent framework landscape in 2026 has matured significantly, with a clear shift from simple prompt chains to stateful orchestration with human-in-the-loop capabilities. 57% of organizations now report having AI agents in production.

## Major Frameworks

### LangGraph
- **Type**: Graph-based state machine
- **Status**: #1 production-ranked agent framework
- **Stars**: 80K+ on GitHub
- **Key Feature**: Explicit state graph with checkpointing, branching, and human-in-the-loop
- **Best For**: Complex multi-step workflows with conditional logic

### CrewAI
- **Type**: Role-based multi-agent
- **Stars**: 44K+
- **Downloads**: 5.2M/month
- **Key Feature**: Define agent roles, goals, and collaborative workflows
- **Best For**: Multi-agent simulations and role-based task decomposition

### AutoGen / AG2
- **Type**: Multi-agent conversation framework (Microsoft)
- **Status**: Ecosystem split — AG2 (community fork) vs AutoGen v0.4+ (Microsoft)
- **Key Feature**: Conversational agents that can delegate, critique, and iterate
- **Best For**: Research and experimentation with agent communication patterns

### Claude Agent SDK
- **Type**: Anthropic-native agent framework
- **Key Feature**: Powers Claude Code, MCP-native tool integration
- **Best For**: Tight integration with Claude models and Anthropic ecosystem

### Pydantic AI
- **Type**: Type-safe, FastAPI-inspired agent framework
- **Key Feature**: Strong typing, validation, and structured output guarantees
- **Best For**: Production systems requiring reliability and type safety

## Key Trends

1. **Shift from Chains to Graphs**: LangChain's linear chains are being replaced by graph-based state machines that can branch, loop, and recover from errors.
2. **Human-in-the-Loop**: Production agents increasingly include approval gates and human oversight checkpoints.
3. **MCP Integration**: Model Context Protocol (MCP) is becoming the standard for tool integration across frameworks.
4. **Production Focus**: The conversation has moved from "can we build agents?" to "how do we run them reliably at scale?"

## Related Pages

- [[langchain]] — Foundational chain framework
- [[crewai]] — Multi-agent orchestration
- [[claude-code]] — Claude Agent SDK in action
- [[kimi-k2-6]] — Agent-capable open-source model
