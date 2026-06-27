---
type: DailyRadar
date: "2026-06-27"
language: zh-CN
audience: "中文 LLM / Agent 工程师"
tags: [agents, evals, inference, llm-infra, model-releases, papers, rag, safety]
source: "../../../../archive/2026/06/27/digest/20260627_093827/daily.md"
---

# 2026-06-27 LLM 工程情报 Radar

> 面向中文 LLM / Agent 工程师，优先关注模型、Agent、RAG、评测、安全、推理和基础设施的工程价值。

## 快速入口

- [项目首页](../../../../README.md)
- [每日索引](../../../README.md)
- [主题索引](../../../../topics/README.md)
- [原始归档](../../../../archive/2026/06/27/README.md)

## 今日主线

- **P0** MIRROR：面向 Agentic RAG 的跨表面红队框架
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-27) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-27) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-27) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-27)
  - 条目：[结构化记录](../../../../items/2026/06/27/daily/top-01-mirror-agentic-rag-novelty-constrained.md)
  - 源内容：[arXiv: 2606.26793v1](https://arxiv.org/abs/2606.26793v1)
  - 摘要：MIRROR：面向 Agentic RAG 的跨表面红队框架：核心变化是提出 novelty-constrained、memory-guided MCTS，用于覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level tool manipulatio...
- **P0** Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模
  - 主题：[RAG / Knowledge](../../../../topics/rag/index.md#2026-06-27) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-27) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-27) · [论文](../../../../topics/papers/index.md#2026-06-27)
  - 条目：[结构化记录](../../../../items/2026/06/27/daily/top-02-temporal-validity-in-retrieval-memory.md)
  - 源内容：[arXiv: 2606.26511v1](https://arxiv.org/abs/2606.26511v1)
  - 摘要：Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模：核心变化是把 stale-fact errors 明确为结构性检索问题：事实变更后，旧事实与新事实 embedding 相似度接近，候选摘要报告 cosine similarity 区分...
- **P0** OpenRCA 2.0：从结果标签转向因果过程监督
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-27) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-27) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-27) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-27)
  - 条目：[结构化记录](../../../../items/2026/06/27/daily/top-03-openrca-root-cause-analysis-pattern.md)
  - 源内容：[arXiv: 2606.27154v1](https://arxiv.org/abs/2606.27154v1)
  - 摘要：OpenRCA 2.0：从结果标签转向因果过程监督：核心变化是针对 root cause analysis 任务，指出只标 root cause 容易退化成 pattern matching，并引入 PAVE step-wise labeling protocol 来标注从故障到症状的传播路径；工...
- **P1** Hugging Face Jobs 一行启动 vLLM Server
  - 主题：[模型发布](../../../../topics/model-releases/index.md#2026-06-27) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-27) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-27) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-27)
  - 条目：[结构化记录](../../../../items/2026/06/27/daily/top-04-jobs-vllm-server-blog-hf.md)
  - 源内容：[Hugging Face: blog/vllm-jobs](https://huggingface.co/blog/vllm-jobs)
  - 摘要：Hugging Face Jobs 一行启动 vLLM Server：核心变化是 Hugging Face Blog 发布在 HF Jobs 中运行 vLLM server 的工程路径；工程影响是临时模型服务、benchmark、demo/评测环境可以更低摩擦地拉起 vLLM，而不必先维护长期 G...
- **P1** InternScience/Agents-A1：Apache-2.0 的 Agent 向模型候选
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-27) · [模型发布](../../../../topics/model-releases/index.md#2026-06-27) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-27) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-27)
  - 条目：[结构化记录](../../../../items/2026/06/27/daily/top-05-internscience-agents-a1-apache-agent.md)
  - 源内容：[Hugging Face: InternScience/Agents-A1](https://huggingface.co/InternScience/Agents-A1)
  - 摘要：InternScience/Agents-A1：Apache-2.0 的 Agent 向模型候选：核心变化是 Hugging Face 在 2026-06-26T22:18:39Z 更新 InternScience/Agents-A1，标签包含 qwen3_5_moe、image-text-to-...
- **P0** LLM-OS-Models/LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters：面向 terminal-agent 的 LoRA/adapter 信号
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-27) · [模型发布](../../../../topics/model-releases/index.md#2026-06-27) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-27) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-27)
  - 条目：[结构化记录](../../../../items/2026/06/27/daily/top-06-llm-os-models-lfm2-8b.md)
  - 源内容：[Hugging Face: LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters](https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters)
  - 摘要：LLM-OS-Models/LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters：面向 terminal-agent 的 LoRA/adapter 信号：核心变化是 Hugging Face 在 2026-06-27T01:16:44Z 更新基于 LiquidAI/L...

## 按主题阅读

- [Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-27)：4 条
- [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-27)：4 条
- [推理 / Serving](../../../../topics/inference/index.md#2026-06-27)：4 条
- [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-27)：2 条
- [模型发布](../../../../topics/model-releases/index.md#2026-06-27)：3 条
- [论文](../../../../topics/papers/index.md#2026-06-27)：1 条
- [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-27)：5 条
- [安全 / Alignment](../../../../topics/safety/index.md#2026-06-27)：1 条

## 原始归档

- [当日 archive index](../../../../archive/2026/06/27/README.md)
- [每日 digest 原文](../../../../archive/2026/06/27/digest/20260627_093827/daily.md)
