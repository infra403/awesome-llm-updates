---
type: IntelItem
title: "SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断"
date: "2026-06-24"
language: zh-CN
importance: P0
tags: [agents, rag, evals, llm-infra]
source: "../../../../../archive/2026/06/24/digest/20260624_213559/daily.md"
window: daily
---

# SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断

## 摘要

**SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断**：核心变化是 arXiv 2026-06-23 论文 *SHERLOC: Structured Diagnostic Localization for Code Repair Agents* 被标记为 P0、quality_score=18，指出 repo-level coding agent 会把约一半预算花在 fault localization，提出 training-free 的结构化假设探索/诊断定位框架；工程影响在于 coding agent 的成本和成功率瓶颈可能不在编辑器，而在定位阶段是否能产出可执行诊断上下文，适合改造 SWE-bench 类流水线的 pre-edit 阶段；建议动作：**今天应实验**，优先在一个内部 bugfix benchmark 上比较“文件检索 top-k”与“结构化诊断上下文”对修复成功率和 token 成本的影响；证据边界：候选确认论文方向与摘要，未确认开源实现、具体提升幅度和适配哪些模型；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/24/digest/20260624_213559/daily.md)

## 来源链接

- [arXiv: 2606.24820v1](https://arxiv.org/abs/2606.24820v1)
