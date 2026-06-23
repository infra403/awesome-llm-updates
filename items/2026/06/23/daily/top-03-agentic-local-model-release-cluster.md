---
type: IntelItem
title: "Agentic local model release cluster：Gemma/Fabliq 系列强调 tool-use、terminal、coding-agent"
date: "2026-06-23"
language: zh-CN
importance: P0
tags: [agents, model-releases, rag, inference]
source: "../../../../../archive/2026/06/23/digest/20260623-213642/daily.md"
window: daily
---

# Agentic local model release cluster：Gemma/Fabliq 系列强调 tool-use、terminal、coding-agent

## 摘要

**Agentic local model release cluster：Gemma/Fabliq 系列强调 tool-use、terminal、coding-agent**：核心变化是 Hugging Face 在当前 10 小时模型窗口出现多个 P0 模型更新，包括 `tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-*`（2026-06-23T13:10Z，image-text-to-text/text-generation 标签、Apache-2.0、coding/agentic/tool-use/reasoning/terminal）和 `LLM-OS-Models/Fabliq-8B-Agent`（2026-06-23T12:24Z，LFM/Liquid-AI MoE、terminal/toolbench SFT、coding-agent）；工程影响是本地/私有 Agent、工具调用和代码工作流的模型选型池继续扩大；建议动作：**今天应实验**，只做小规模 smoke test：函数调用/终端任务、代码修复、视觉文本输入（Gemma cluster）和延迟/显存占用；证据边界：候选确认模型卡元数据、更新时间、标签和少量下载/点赞，不确认真实 benchmark、对齐质量或安全边界；

## P级别依据

P0：命中 Agent / Coding Agent、模型发布、RAG / Knowledge，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/23/digest/20260623-213642/daily.md)

## 来源链接

- [Hugging Face: tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1](https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1)
- [Hugging Face: tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1](https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1)
- [Hugging Face: LLM-OS-Models/Fabliq-8B-Agent](https://huggingface.co/LLM-OS-Models/Fabliq-8B-Agent)
