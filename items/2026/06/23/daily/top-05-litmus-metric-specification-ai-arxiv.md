---
type: IntelItem
title: "Litmus：用代码驱动、零标签 metric specification 评估 AI 系统"
date: "2026-06-23"
language: zh-CN
importance: P1
tags: [agents, inference, evals, llm-infra]
source: "../../../../../archive/2026/06/23/digest/20260623-213642/daily.md"
window: daily
---

# Litmus：用代码驱动、零标签 metric specification 评估 AI 系统

## 摘要

**Litmus：用代码驱动、零标签 metric specification 评估 AI 系统**：核心变化是 arXiv 2026-06-22 新增论文提出 zero-label、code-driven metric specification，用于评估 AI/Agent 系统；工程影响在评测平台和 CI gate：把评测标准从自然语言 rubrics 转成可执行 metric 可能降低人工标注依赖，并更适合部署前回归测试；建议动作：**今天应阅读**，重点判断 metric DSL/代码规范是否能接入现有 eval harness、Opik/LangSmith/自研 CI；证据边界：候选确认标题、摘要方向、日期和 URL，未确认方法细节、开源实现或误判成本；

## P级别依据

P1：命中 Agent / Coding Agent、推理 / Serving、评测 / Benchmarks，包含可直接核验的源链接；适合进入阅读、实验或技术储备队列。

## 工程影响

把相关 benchmark 当作参考信号，优先沉淀内部私有回归集和真实任务评测。

## 来源

- [每日 digest](../../../../../archive/2026/06/23/digest/20260623-213642/daily.md)

## 来源链接

- [arXiv: 2606.23403v1](https://arxiv.org/abs/2606.23403v1)
