---
type: IntelItem
title: "OpenRCA 2.0：从结果标签转向因果过程监督"
date: "2026-06-27"
language: zh-CN
importance: P0
tags: [agents, rag, inference, evals]
source: "../../../../../archive/2026/06/27/digest/20260627_093827/daily.md"
window: daily
---

# OpenRCA 2.0：从结果标签转向因果过程监督

## 摘要

**OpenRCA 2.0：从结果标签转向因果过程监督**：核心变化是针对 root cause analysis 任务，指出只标 root cause 容易退化成 pattern matching，并引入 PAVE step-wise labeling protocol 来标注从故障到症状的传播路径；工程影响是评测 LLM Agent 的长上下文、多步推理、工具使用时，应看过程监督和因果链路，而不仅是最终答案；建议动作：**今天应阅读**，可作为 SRE/DevOps Agent eval 的候选基准；证据边界：候选确认论文题目、摘要、发布时间 2026-06-25，未确认 benchmark 规模、开源许可和线上可下载资产；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、推理 / Serving，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/27/digest/20260627_093827/daily.md)

## 来源链接

- [arXiv: 2606.27154v1](https://arxiv.org/abs/2606.27154v1)
