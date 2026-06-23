---
type: IntelItem
title: "Agent/RAG 的上下文管理与流式工具调用开始被拆解为可工程化机制"
date: "2026-06-22"
language: zh-CN
importance: P0
tags: [agents, rag, llm-infra, papers]
source: "../../../../../archive/2026/06/22/digest/20260622-224238/daily.md"
window: daily
---

# Agent/RAG 的上下文管理与流式工具调用开始被拆解为可工程化机制

## 摘要

**Agent/RAG 的上下文管理与流式工具调用开始被拆解为可工程化机制**：2026-06-18 arXiv 论文 PACMS 将 Agent 上下文选择建模为可插拔 submodular selection；Streaming RAG 论文指出只有当 tool intent 在用户输入结束前已稳定时，提前检索才有收益。

## 工程影响

检查 agent runtime、工具权限、状态管理、审计日志和失败恢复是否需要调整。

## 来源

- [每日 digest](../../../../../archive/2026/06/22/digest/20260622-224238/daily.md)

## 来源链接

- [arXiv: 2606.20047v1](https://arxiv.org/abs/2606.20047v1)
- [arXiv: 2606.20113v1](https://arxiv.org/abs/2606.20113v1)
