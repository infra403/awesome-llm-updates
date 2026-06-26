---
type: IntelItem
title: "Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性"
date: "2026-06-26"
language: zh-CN
importance: P0
tags: [agents, rag, evals, llm-infra]
source: "../../../../../archive/2026/06/26/digest/20260626-213634/daily.md"
window: daily
---

# Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性

## 摘要

**Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性**：核心变化是论文指出传统 embedding 相似度无法可靠区分“重复事实”和“已过期/被推翻事实”，候选摘要给出 contradicted vs duplicated fact 的 AUROC 0.59（接近随机）；工程影响是长期记忆、代码知识库、API 文档 RAG 和 Agent workflow 需要把 valid\_from/valid\_to、版本和冲突消解纳入检索排序，而不是只依赖向量相似度；建议动作：**今天应阅读**，优先检查自家 RAG 是否会把旧 API、旧配置和旧决策与新事实混检；证据边界：已确认来源为 2026-06-25 arXiv 候选摘要，未确认完整实验设置和数据集细节；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/26/digest/20260626-213634/daily.md)

## 来源链接

- [arXiv: 2606.26511v1](https://arxiv.org/abs/2606.26511v1)
