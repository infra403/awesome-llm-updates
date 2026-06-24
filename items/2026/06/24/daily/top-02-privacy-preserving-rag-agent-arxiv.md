---
type: IntelItem
title: "Privacy-Preserving RAG：用多 Agent 语义重写降低敏感信息泄漏"
date: "2026-06-24"
language: zh-CN
importance: P0
tags: [agents, rag, inference, evals]
source: "../../../../../archive/2026/06/24/digest/20260624-0935/daily.md"
window: daily
---

# Privacy-Preserving RAG：用多 Agent 语义重写降低敏感信息泄漏

## 摘要

**Privacy-Preserving RAG：用多 Agent 语义重写降低敏感信息泄漏**：arXiv 新论文（published: 2026-06-23，quality_score 18，P0）提出由隐私抽取、语义分析、重构三个 Agent 协作，对检索内容做语义重写，在保留上下文语义的同时去除敏感标识；工程影响是企业 RAG/知识库问答可在检索后、生成前增加 sanitization layer，尤其适合客服、法务、医疗、内部知识库；建议动作：**今天应实验**，用一小批内部文档做 PII rewrite + answer fidelity A/B 测试；证据边界：候选确认方法框架与目标，未确认是否开源、延迟开销和跨语言效果；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、推理 / Serving，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/24/digest/20260624-0935/daily.md)

## 来源链接

- [arXiv: 2606.24623v1](https://arxiv.org/abs/2606.24623v1)
