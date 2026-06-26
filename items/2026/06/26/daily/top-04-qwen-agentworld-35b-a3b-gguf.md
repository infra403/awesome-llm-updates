---
type: IntelItem
title: "Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支"
date: "2026-06-26"
language: zh-CN
importance: P1
tags: [agents, model-releases, rag, inference]
source: "../../../../../archive/2026/06/26/digest/20260626-213634/daily.md"
window: daily
---

# Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支

## 摘要

**Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支**：核心变化是 HF 上新增/更新 FreedomAISVR 的 Qwen-AgentWorld-35B-A3B-NVFP4-GGUF 与 MXFP4-MOE-GGUF，标签包含 agent、world-model、vision、multimodal、GGUF、Apache-2.0，更新时间分别为 2026-06-26 13:30:14/13:30:21 UTC；工程影响是本地/边缘 Agent、多模态 Agent 原型可以评估更低精度 GGUF 路线，但需要验证实际上下文、视觉能力、工具调用与量化精度损失；建议动作：**今天应实验**，只在隔离环境跑 smoke test 和小型 agent task，不直接进入生产模型池；证据边界：已确认 HF 元数据、下载量和标签，未确认官方来源、模型卡质量、benchmark 与安全评测；

## P级别依据

P1：命中 Agent / Coding Agent、模型发布、RAG / Knowledge，包含可直接核验的源链接；适合进入阅读、实验或技术储备队列。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/26/digest/20260626-213634/daily.md)

## 来源链接

- [Hugging Face: FreedomAISVR/Qwen-AgentWorld-35B-A3B-NVFP4-GGUF](https://huggingface.co/FreedomAISVR/Qwen-AgentWorld-35B-A3B-NVFP4-GGUF)
- [Hugging Face: FreedomAISVR/Qwen-AgentWorld-35B-A3B-MXFP4-MOE-GGUF](https://huggingface.co/FreedomAISVR/Qwen-AgentWorld-35B-A3B-MXFP4-MOE-GGUF)
