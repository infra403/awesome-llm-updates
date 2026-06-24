---
type: IntelItem
title: "开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新"
date: "2026-06-24"
language: zh-CN
importance: P0
tags: [agents, rag, evals, safety]
source: "../../../../../archive/2026/06/24/digest/20260624_213559/daily.md"
window: daily
---

# 开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新

## 摘要

**开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新**：核心变化是 GitHub 8 小时窗口内 P0 仓库包括 `comet-ml/opik`（quality_score=20，updated 2026-06-24T13:34:31Z，19,755 stars，LLM/RAG/agent tracing 与 eval）、`langgenius/dify`（quality_score=20，updated 2026-06-24T13:34:46Z，146,428 stars，agentic workflow / MCP / RAG）、`can1357/oh-my-pi`（quality_score=20，updated 2026-06-24T13:31:31Z，14,444 stars，terminal coding agent、hash-anchored edits、LSP、browser、subagents）；工程影响在于团队 workflow 的核心差异化正从“能调模型 API”转向“可观测、可评测、可编排、可安全编辑代码”；建议动作：**持续观察**，若团队正在搭 Agent 平台，今天可优先阅读 Opik 的 tracing/eval 能力和 Dify 的 MCP/workflow 更新，oh-my-pi 适合对比终端 coding agent 的编辑保障；证据边界：GitHub 候选只确认本周期 updated/stars/summary/tags，未确认具体 commit 内容、release note 或 breaking change；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、评测 / Benchmarks，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/24/digest/20260624_213559/daily.md)

## 来源链接

- [GitHub: comet-ml/opik](https://github.com/comet-ml/opik)
- [GitHub: langgenius/dify](https://github.com/langgenius/dify)
- [GitHub: can1357/oh-my-pi](https://github.com/can1357/oh-my-pi)
