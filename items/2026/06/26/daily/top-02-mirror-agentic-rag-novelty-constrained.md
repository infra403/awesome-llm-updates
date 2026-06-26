---
type: IntelItem
title: "MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架"
date: "2026-06-26"
language: zh-CN
importance: P0
tags: [agents, rag, evals, safety]
source: "../../../../../archive/2026/06/26/digest/20260626-213634/daily.md"
window: daily
---

# MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架

## 摘要

**MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架**：核心变化是用 novelty-constrained memory-guided MCTS 生成更少重复的攻击样本，覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level tool manipulation；工程影响是多模态 Agentic RAG 的安全评测不能只做 prompt injection，应把检索层、工具编排层、图文输入层纳入统一红队；建议动作：**今天应阅读**，安全/评测负责人应抽取其攻击面分类转成内部 eval checklist；证据边界：已确认候选摘要声称现有文本投毒 benchmark 有 73-84% exact duplication，未确认 MIRROR 的开源状态与复现实验成本；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/26/digest/20260626-213634/daily.md)

## 来源链接

- [arXiv: 2606.26793v1](https://arxiv.org/abs/2606.26793v1)
