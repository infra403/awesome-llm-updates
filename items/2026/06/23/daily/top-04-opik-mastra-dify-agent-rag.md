---
type: IntelItem
title: "Opik / Mastra / Dify：Agent/RAG/LLMOps 工具链在同一窗口高活跃"
date: "2026-06-23"
language: zh-CN
importance: P0
tags: [agents, rag, evals, llm-infra]
source: "../../../../../archive/2026/06/23/digest/20260623-213642/daily.md"
window: daily
---

# Opik / Mastra / Dify：Agent/RAG/LLMOps 工具链在同一窗口高活跃

## 摘要

**Opik / Mastra / Dify：Agent/RAG/LLMOps 工具链在同一窗口高活跃**：核心变化是 GitHub 当前 8 小时窗口内多个 P0 工具仓库更新：`comet-ml/opik`（2026-06-23T13:35Z，19,731 stars，LLM/RAG/agent tracing、eval、monitoring）、`mastra-ai/mastra`（2026-06-23T13:35Z，25,361 stars，TypeScript AI app/agent framework，MCP/evals/workflows）、`langgenius/dify`（2026-06-23T13:32Z，146,268 stars，agentic workflow/RAG/MCP/low-code）；工程影响是 Agent workflow 进入“构建框架 + tracing/eval + 平台化编排”的组合选型阶段；建议动作：**持续观察**，今天不把“updated”当版本发布，建议只检查 release/changelog/commit diff 是否包含破坏性变更或新增评测能力；证据边界：候选确认仓库元数据、更新时间和主题标签，未确认具体 commit 内容；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/23/digest/20260623-213642/daily.md)

## 来源链接

- [GitHub: comet-ml/opik](https://github.com/comet-ml/opik)
- [GitHub: mastra-ai/mastra](https://github.com/mastra-ai/mastra)
- [GitHub: langgenius/dify](https://github.com/langgenius/dify)
