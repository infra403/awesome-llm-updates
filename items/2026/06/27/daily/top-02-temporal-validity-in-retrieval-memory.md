---
type: IntelItem
title: "Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模"
date: "2026-06-27"
language: zh-CN
importance: P0
tags: [rag, evals, llm-infra, papers]
source: "../../../../../archive/2026/06/27/digest/20260627_093827/daily.md"
window: daily
---

# Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模

## 摘要

**Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模**：核心变化是把 stale-fact errors 明确为结构性检索问题：事实变更后，旧事实与新事实 embedding 相似度接近，候选摘要报告 cosine similarity 区分矛盾事实和重复事实 AUROC 仅 0.59；工程影响是知识库、代码助手、API 文档问答需要引入时间有效性/版本有效性，而不是只依赖向量相似度；建议动作：**今天应阅读**，并把“过期事实召回”加入 RAG eval；证据边界：候选确认了摘要中的 AUROC 与问题设定，未确认完整数据集、消融和实现细节；

## P级别依据

P0：命中 RAG / Knowledge、评测 / Benchmarks、LLM Infra，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/27/digest/20260627_093827/daily.md)

## 来源链接

- [arXiv: 2606.26511v1](https://arxiv.org/abs/2606.26511v1)
