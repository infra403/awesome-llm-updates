---
type: IntelItem
title: "MIRROR：面向 Agentic RAG 的跨表面红队框架"
date: "2026-06-27"
language: zh-CN
importance: P0
tags: [agents, rag, evals, safety]
source: "../../../../../archive/2026/06/27/digest/20260627_093827/daily.md"
window: daily
---

# MIRROR：面向 Agentic RAG 的跨表面红队框架

## 摘要

**MIRROR：面向 Agentic RAG 的跨表面红队框架**：核心变化是提出 novelty-constrained、memory-guided MCTS，用于覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level tool manipulation，并指出既有红队模板在文本投毒基准上有 73–84% exact duplication；工程影响是 RAG/多模态 Agent 的安全评测不能只测 prompt injection，需要把检索内容、图片输入、工具编排层一起纳入攻击面；建议动作：**今天应阅读**，优先评估是否能补到内部 RAG/Agent 回归测试；证据边界：候选确认了论文摘要、发布时间 2026-06-25、arXiv 来源和攻击面描述，未确认代码/数据是否可用、指标是否可复现；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/27/digest/20260627_093827/daily.md)

## 来源链接

- [arXiv: 2606.26793v1](https://arxiv.org/abs/2606.26793v1)
