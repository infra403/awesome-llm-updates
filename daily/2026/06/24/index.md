---
type: DailyRadar
date: "2026-06-24"
language: zh-CN
audience: "中文 LLM / Agent 工程师"
tags: [agents, evals, inference, llm-infra, model-releases, rag, safety]
source: "../../../../archive/2026/06/24/digest/20260624_213559/daily.md"
---

# 2026-06-24 LLM 工程情报 Radar

> 面向中文 LLM / Agent 工程师，优先关注模型、Agent、RAG、评测、安全、推理和基础设施的工程价值。

## 快速入口

- [项目首页](../../../../README.md)
- [每日索引](../../../README.md)
- [主题索引](../../../../topics/README.md)
- [原始归档](../../../../archive/2026/06/24/README.md)

## 今日主线

- **P1** OpenAI 与 Broadcom 发布 LLM 推理芯片 Jalapeño
  - 主题：[推理 / Serving](../../../../topics/inference/index.md#2026-06-24) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-01-broadcom-llm-jalape-news-2026.md)
  - 源内容：[OpenAI: Openai Broadcom Jalapeno Inference Chip](https://openai.com/index/openai-broadcom-jalapeno-inference-chip)
  - 摘要：OpenAI 与 Broadcom 发布 LLM 推理芯片 Jalapeño：核心变化是 OpenAI News 在 2026-06-24 发布定制 AI 推理芯片消息，候选标记为 P1、quality_score=15，reason_codes 包含 recent_window、source_s...
- **P0** Agent-native memory 从“任务成功率黑盒”转向可拆解的数据管理系统评测
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-02-agent-native-memory-arxiv-2026.md)
  - 源内容：[arXiv: 2606.24775v1](https://arxiv.org/abs/2606.24775v1)
  - 摘要：Agent-native memory 从“任务成功率黑盒”转向可拆解的数据管理系统评测：核心变化是 arXiv 2026-06-23 论文 *Are We Ready For An Agent-Native Memory System?* 被标记为 P0、quality_score=18，提出把...
- **P0** SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-03-sherloc-agent-arxiv-2026-06.md)
  - 源内容：[arXiv: 2606.24820v1](https://arxiv.org/abs/2606.24820v1)
  - 摘要：SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断：核心变化是 arXiv 2026-06-23 论文 *SHERLOC: Structured Diagnostic Localization for Code Repair Agents* 被标记为 P0、quality...
- **P0** RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-24) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-04-rag-arxiv-2026-06-23.md)
  - 源内容：[arXiv: 2606.24623v1](https://arxiv.org/abs/2606.24623v1) · [arXiv: 2606.24402v1](https://arxiv.org/abs/2606.24402v1)
  - 摘要：RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒：核心变化是两篇 arXiv 2026-06-23 P0 论文同时进入窗口：*Privacy-Preserving RAG via Multi-Agent Semantic Rewriting*（quality_score=18）关注用多 A...
- **P0** Hugging Face 本周期集中出现 Agentic / terminal / reasoning 小模型与 GGUF 量化候选
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [模型发布](../../../../topics/model-releases/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-05-agentic-terminal-reasoning-gguf-10.md)
  - 源内容：[Hugging Face: osmapi/osmQwopus3.6-27B-Fable-Agentic](https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic) · [Hugging Face: mradermacher/Fabliq-8B-Agent-Reasoning-GGUF](https://huggingface.co/mradermacher/Fabliq-8B-Agent-Reasoning-GGUF) · [Hugging Face: LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters](https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters)
  - 摘要：Hugging Face 本周期集中出现 Agentic / terminal / reasoning 小模型与 GGUF 量化候选：核心变化是模型巡检在 10 小时窗口内发现多个 P0/P1 模型：osmapi/osmQwopus3.6-27B-Fable-Agentic（P0，quality_...
- **P0** 开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-06-llm-agent-workflow-coding-p0.md)
  - 源内容：[GitHub: comet-ml/opik](https://github.com/comet-ml/opik) · [GitHub: langgenius/dify](https://github.com/langgenius/dify) · [GitHub: can1357/oh-my-pi](https://github.com/can1357/oh-my-pi)
  - 摘要：开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新：核心变化是 GitHub 8 小时窗口内 P0 仓库包括 comet-ml/opik（quality_score=20，updated 2026-06-24T13:34:31Z，...

## 按主题阅读

- [Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24)：5 条
- [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24)：4 条
- [推理 / Serving](../../../../topics/inference/index.md#2026-06-24)：3 条
- [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24)：3 条
- [模型发布](../../../../topics/model-releases/index.md#2026-06-24)：1 条
- [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24)：5 条
- [安全 / Alignment](../../../../topics/safety/index.md#2026-06-24)：1 条

## 原始归档

- [当日 archive index](../../../../archive/2026/06/24/README.md)
- [每日 digest 原文](../../../../archive/2026/06/24/digest/20260624_213559/daily.md)
