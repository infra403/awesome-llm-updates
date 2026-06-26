---
type: IntelItem
title: "ShareLock：针对 MCP 的多工具阈值投毒攻击"
date: "2026-06-26"
language: zh-CN
importance: P0
tags: [agents, safety, llm-infra, papers]
source: "../../../../../archive/2026/06/26/digest/20260626-0936/daily.md"
window: daily
---

# ShareLock：针对 MCP 的多工具阈值投毒攻击

## 摘要

**ShareLock：针对 MCP 的多工具阈值投毒攻击**：核心变化是 arXiv 2026-06-25 新增一篇 MCP 安全论文，指出随着 MCP 成为 Agent 调工具基础设施，攻击者可利用多工具、阈值式投毒绕过人工检查并在 LLM-server 交互中注入恶意提示；工程影响是所有使用 MCP server、工具 marketplace、远程工具注册表的 Agent 架构都需要重新评估工具描述、权限边界和审计策略；建议动作：**今天应阅读**，因为这是当前 Agent 工具链安全的高优先级风险；证据边界：候选确认了论文题名、日期、摘要和 URL，未确认攻击复现代码或影响范围，需阅读原文验证威胁模型；

## P级别依据

P0：命中 Agent / Coding Agent、安全 / Alignment、LLM Infra，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/26/digest/20260626-0936/daily.md)

## 来源链接

- [arXiv: 2606.27027v1](https://arxiv.org/abs/2606.27027v1)
