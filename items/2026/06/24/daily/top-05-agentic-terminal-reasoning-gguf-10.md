---
type: IntelItem
title: "Hugging Face 本周期集中出现 Agentic / terminal / reasoning 小模型与 GGUF 量化候选"
date: "2026-06-24"
language: zh-CN
importance: P0
tags: [agents, model-releases, rag, inference]
source: "../../../../../archive/2026/06/24/digest/20260624_213559/daily.md"
window: daily
---

# Hugging Face 本周期集中出现 Agentic / terminal / reasoning 小模型与 GGUF 量化候选

## 摘要

**Hugging Face 本周期集中出现 Agentic / terminal / reasoning 小模型与 GGUF 量化候选**：核心变化是模型巡检在 10 小时窗口内发现多个 P0/P1 模型：`osmapi/osmQwopus3.6-27B-Fable-Agentic`（P0，quality_score=19，2026-06-24T11:26:57Z，Apache-2.0，tool/function-calling/reasoning 标签）、`mradermacher/Fabliq-8B-Agent-Reasoning-GGUF`（P0，quality_score=19，2026-06-24T12:48:30Z，GGUF/agentic/tool-use/terminal 标签）、`LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters`（P0，quality_score=18，2026-06-24T13:11:55Z，terminal-agent/RLVR/GRPO/LoRA 标签）；工程影响在于本地/边缘 Agent 原型可用的模型形态继续向 3B/8B/27B、GGUF、LoRA adapter、tool-use 标签聚集，但下载量和 likes 很低，不能直接视为成熟基座；建议动作：**持续观察**，对 8B GGUF 可做 smoke test（工具调用格式、终端任务、上下文遵循），对 27B/adapter 先等 model card、eval 和社区反馈；证据边界：候选确认时间、标签、license、likes/downloads，未确认真实工具调用准确率、benchmark、训练数据或安全评估；

## P级别依据

P0：命中 Agent / Coding Agent、模型发布、RAG / Knowledge，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/24/digest/20260624_213559/daily.md)

## 来源链接

- [Hugging Face: osmapi/osmQwopus3.6-27B-Fable-Agentic](https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic)
- [Hugging Face: mradermacher/Fabliq-8B-Agent-Reasoning-GGUF](https://huggingface.co/mradermacher/Fabliq-8B-Agent-Reasoning-GGUF)
- [Hugging Face: LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters](https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters)
