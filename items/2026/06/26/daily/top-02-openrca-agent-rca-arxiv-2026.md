---
type: IntelItem
title: "OpenRCA 2.0：从结果标签转向因果过程监督的 Agent RCA 评测"
date: "2026-06-26"
language: zh-CN
importance: P0
tags: [agents, rag, evals, llm-infra]
source: "../../../../../archive/2026/06/26/digest/20260626-0936/daily.md"
window: daily
---

# OpenRCA 2.0：从结果标签转向因果过程监督的 Agent RCA 评测

## 摘要

**OpenRCA 2.0：从结果标签转向因果过程监督的 Agent RCA 评测**：核心变化是 arXiv 2026-06-25 新增 RCA/Agent 评测论文，提出 PAVE step-wise labeling protocol，试图把根因分析从“只猜最终 root cause”推进到“标注故障传播路径”；工程影响是对 SRE/可观测性 Agent、长上下文故障诊断、多步工具调用评测更有参考价值，可用于替代只看最终答案的弱评测；建议动作：**今天应阅读**，并把其评价维度映射到团队内部 incident-agent benchmark；证据边界：候选确认摘要、日期、arXiv URL，未确认数据集可下载状态、许可证和基准结果；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/26/digest/20260626-0936/daily.md)

## 来源链接

- [arXiv: 2606.27154v1](https://arxiv.org/abs/2606.27154v1)
