---
type: DailyRadar
date: "2026-06-26"
language: zh-CN
audience: "中文 LLM / Agent 工程师"
tags: [agents, evals, inference, llm-infra, model-releases, rag, safety]
source: "../../../../archive/2026/06/26/digest/20260626-213634/daily.md"
---

# 2026-06-26 LLM 工程情报 Radar

> 面向中文 LLM / Agent 工程师，优先关注模型、Agent、RAG、评测、安全、推理和基础设施的工程价值。

## 快速入口

- [项目首页](../../../../README.md)
- [每日索引](../../../README.md)
- [主题索引](../../../../topics/README.md)
- [原始归档](../../../../archive/2026/06/26/README.md)

## 今日主线

- **P0** Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-01-temporal-validity-in-retrieval-memory.md)
  - 源内容：[arXiv: 2606.26511v1](https://arxiv.org/abs/2606.26511v1)
  - 摘要：Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性：核心变化是论文指出传统 embedding 相似度无法可靠区分“重复事实”和“已过期/被推翻事实”，候选摘要给出 contradicted vs duplicated fact 的 AURO...
- **P0** MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-02-mirror-agentic-rag-novelty-constrained.md)
  - 源内容：[arXiv: 2606.26793v1](https://arxiv.org/abs/2606.26793v1)
  - 摘要：MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架：核心变化是用 novelty-constrained memory-guided MCTS 生成更少重复的攻击样本，覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level to...
- **P0** OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-03-openrca-pave-rca-agent-root.md)
  - 源内容：[arXiv: 2606.27154v1](https://arxiv.org/abs/2606.27154v1)
  - 摘要：OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测：核心变化是候选摘要指出现有 RCA 数据集只标 root cause，容易退化成模式匹配；新协议强调 fault propagation path 的逐步标签；工程影响是 AIOps/可观测性 Agent...
- **P1** Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [模型发布](../../../../topics/model-releases/index.md#2026-06-26) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-04-qwen-agentworld-35b-a3b-gguf.md)
  - 源内容：[Hugging Face: FreedomAISVR/Qwen-AgentWorld-35B-A3B-NVFP4-GGUF](https://huggingface.co/FreedomAISVR/Qwen-AgentWorld-35B-A3B-NVFP4-GGUF) · [Hugging Face: FreedomAISVR/Qwen-AgentWorld-35B-A3B-MXFP4-MOE-GGUF](https://huggingface.co/FreedomAISVR/Qwen-AgentWorld-35B-A3B-MXFP4-MOE-GGUF)
  - 摘要：Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支：核心变化是 HF 上新增/更新 FreedomAISVR 的 Qwen-AgentWorld-35B-A3B-NVFP4-GGUF 与 MXFP4-MOE-GGUF，标签包含 agent、...
- **P1** GitHub Agent/RAG 工程栈集中活跃：Dify、RAGFlow、Neo.mjs、OpenLoomi
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-05-agent-rag-dify-ragflow-neo.md)
  - 源内容：[GitHub: langgenius/dify](https://github.com/langgenius/dify) · [GitHub: infiniflow/ragflow](https://github.com/infiniflow/ragflow) · [GitHub: neomjs/neo](https://github.com/neomjs/neo) · 其余 1 个见结构化记录
  - 摘要：GitHub Agent/RAG 工程栈集中活跃：Dify、RAGFlow、Neo.mjs、OpenLoomi：核心变化是 2026-06-26 20:51-21:34 北京时间窗口内，多条高星/明确工程元数据项目更新，覆盖 production-ready agentic workflow、Ag...
- **P1** HF Jobs 一行命令运行 vLLM Server
  - 主题：[模型发布](../../../../topics/model-releases/index.md#2026-06-26) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-06-hf-jobs-vllm-server-blog.md)
  - 源内容：[Hugging Face: blog/vllm-jobs](https://huggingface.co/blog/vllm-jobs)
  - 摘要：HF Jobs 一行命令运行 vLLM Server：核心变化是 Hugging Face Blog 发布 “Run a vLLM Server on HF Jobs in One Command”，把 vLLM server 与 HF Jobs 的启动流程包装为更短路径；工程影响是临时 benc...

## 按主题阅读

- [Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26)：5 条
- [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26)：4 条
- [推理 / Serving](../../../../topics/inference/index.md#2026-06-26)：2 条
- [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)：4 条
- [模型发布](../../../../topics/model-releases/index.md#2026-06-26)：2 条
- [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26)：5 条
- [安全 / Alignment](../../../../topics/safety/index.md#2026-06-26)：2 条

## 原始归档

- [当日 archive index](../../../../archive/2026/06/26/README.md)
- [每日 digest 原文](../../../../archive/2026/06/26/digest/20260626-213634/daily.md)
