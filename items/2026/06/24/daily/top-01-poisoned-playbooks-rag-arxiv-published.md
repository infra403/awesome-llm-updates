---
type: IntelItem
title: "Poisoned Playbooks：RAG 安全智能体的知识投毒风险被具体化"
date: "2026-06-24"
language: zh-CN
importance: P0
tags: [agents, rag, inference, evals]
source: "../../../../../archive/2026/06/24/digest/20260624-0935/daily.md"
window: daily
---

# Poisoned Playbooks：RAG 安全智能体的知识投毒风险被具体化

## 摘要

**Poisoned Playbooks：RAG 安全智能体的知识投毒风险被具体化**：arXiv 新论文（published: 2026-06-23，quality_score 18，P0）聚焦 AI security agents 使用 RAG 做漏洞分析/利用推理时，外部 write-up 被投毒后会如何影响行动型 agent，而不只是 QA 答案污染；工程影响是安全 Agent、漏洞 triage bot、代码审计 Agent 的检索库需要引入来源可信度、内容签名、检索结果隔离和“行动前验证”策略；建议动作：**今天应阅读**，因为它直接影响 RAG + tool-using agent 的安全边界；证据边界：候选摘要确认研究目标与风险类型，未确认实验规模、基准细节和缓解方案有效性，需要读原文；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、推理 / Serving，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/24/digest/20260624-0935/daily.md)

## 来源链接

- [arXiv: 2606.24402v1](https://arxiv.org/abs/2606.24402v1)
