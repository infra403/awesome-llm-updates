---
type: IntelItem
title: "RAG retrieval-state lock-in：一致答案不等于可信答案"
date: "2026-06-23"
language: zh-CN
importance: P0
tags: [rag, evals, llm-infra, papers]
source: "../../../../../archive/2026/06/23/digest/20260623-213642/daily.md"
window: daily
---

# RAG retrieval-state lock-in：一致答案不等于可信答案

## 摘要

**RAG retrieval-state lock-in：一致答案不等于可信答案**：核心变化是 arXiv 2026-06-22 新增论文指出 black-box uncertainty/多采样一致性在 RAG 中会被“同一个错误检索状态”锁定，空检索或错误邻域都可能产生稳定但错误的高一致回答；工程影响在于 RAG 评测与线上置信度策略，不能只看 answer agreement，需要记录检索状态、邻域多样性和 fallback 行为；建议动作：**今天应阅读**，把现有 RAG eval 中的 confidence 指标与 retrieval trace 绑定复查；证据边界：候选确认论文摘要与问题定义，尚未确认具体数据集、算法实现和开源代码；

## P级别依据

P0：命中 RAG / Knowledge、评测 / Benchmarks、LLM Infra，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/23/digest/20260623-213642/daily.md)

## 来源链接

- [arXiv: 2606.22728v1](https://arxiv.org/abs/2606.22728v1)
