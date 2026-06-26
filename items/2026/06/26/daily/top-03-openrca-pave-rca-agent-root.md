---
type: IntelItem
title: "OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测"
date: "2026-06-26"
language: zh-CN
importance: P0
tags: [agents, rag, evals, llm-infra]
source: "../../../../../archive/2026/06/26/digest/20260626-213634/daily.md"
window: daily
---

# OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测

## 摘要

**OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测**：核心变化是候选摘要指出现有 RCA 数据集只标 root cause，容易退化成模式匹配；新协议强调 fault propagation path 的逐步标签；工程影响是 AIOps/可观测性 Agent、日志分析 Agent 和工具调用 Agent 的评测应考察“定位路径”而非只看最终答案；建议动作：**今天应阅读**，可把因果路径标签作为内部 incident replay eval 的评分维度；证据边界：已确认 2026-06-25 arXiv 摘要与 P0 评分，未确认数据规模、标注成本和是否提供代码；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/26/digest/20260626-213634/daily.md)

## 来源链接

- [arXiv: 2606.27154v1](https://arxiv.org/abs/2606.27154v1)
