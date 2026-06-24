---
type: IntelItem
title: "RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒"
date: "2026-06-24"
language: zh-CN
importance: P0
tags: [agents, rag, inference, evals]
source: "../../../../../archive/2026/06/24/digest/20260624_213559/daily.md"
window: daily
---

# RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒

## 摘要

**RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒**：核心变化是两篇 arXiv 2026-06-23 P0 论文同时进入窗口：*Privacy-Preserving RAG via Multi-Agent Semantic Rewriting*（quality_score=18）关注用多 Agent 对检索内容做隐私抽取、语义分析和重构；*Poisoned Playbooks*（quality_score=18）关注知识投毒对 AI security agents 的影响；工程影响在于企业 RAG 不仅要防 prompt 泄密，还要防知识库被污染后误导安全 Agent，检索前清洗、检索后重写、来源可信度和 playbook 变更审计需要作为一套安全链路设计；建议动作：**今天应阅读**，并把“敏感字段语义保真重写”和“知识库投毒回归测试”加入 RAG 安全 checklist；证据边界：候选摘要未确认生产延迟、召回损失、攻击集规模或防御覆盖率；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、推理 / Serving，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/24/digest/20260624_213559/daily.md)

## 来源链接

- [arXiv: 2606.24623v1](https://arxiv.org/abs/2606.24623v1)
- [arXiv: 2606.24402v1](https://arxiv.org/abs/2606.24402v1)
