---
type: IntelItem
title: "开源 Agent/LLM Infra 项目集中更新：workflow、memory、context budget 成为主线"
date: "2026-06-24"
language: zh-CN
importance: P0
tags: [agents, rag, llm-infra, open-source]
source: "../../../../../archive/2026/06/24/digest/20260624-0935/daily.md"
window: daily
---

# 开源 Agent/LLM Infra 项目集中更新：workflow、memory、context budget 成为主线

## 摘要

**开源 Agent/LLM Infra 项目集中更新：workflow、memory、context budget 成为主线**：GitHub 当前窗口 P0 候选包括 Dify（updated: 2026-06-24T01:21:03Z，stars 146330，quality_score 20，P0）、Openloomi（updated: 2026-06-24T01:29:03Z，stars 478，quality_score 20，P0）、SDL-MCP（updated: 2026-06-24T01:30:05Z，stars 376，quality_score 20，P0）和 Omnigent（updated: 2026-06-24T01:30:36Z，stars 4584，quality_score 19，P0）；核心变化是候选元数据集中指向 agentic workflow、memory/RAG、MCP、context budget、multi-agent orchestration；工程影响是团队构建 coding agent 或业务 agent 时，架构关注点正在从“单模型调用”转向上下文预算、工具治理、持久记忆和多 harness 编排；建议动作：**今天应实验**，优先试 SDL-MCP 的代码上下文压缩思路与 Dify/Openloomi 的 workflow/memory 能否接入现有工具链；证据边界：候选确认 repo 元数据与更新时间，未确认本次更新具体 commit 内容或 release notes；

## P级别依据

P0：命中 Agent / Coding Agent、RAG / Knowledge、LLM Infra，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/24/digest/20260624-0935/daily.md)

## 来源链接

- [GitHub: langgenius/dify](https://github.com/langgenius/dify)
- [GitHub: melandlabs/openloomi](https://github.com/melandlabs/openloomi)
- [GitHub: GlitterKill/sdl-mcp](https://github.com/GlitterKill/sdl-mcp)
- [GitHub: omnigent-ai/omnigent](https://github.com/omnigent-ai/omnigent)
