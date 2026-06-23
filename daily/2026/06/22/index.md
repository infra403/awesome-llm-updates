---
type: DailyRadar
date: "2026-06-22"
language: zh-CN
audience: "中文 LLM / Agent 工程师"
tags: [agents, evals, inference, llm-infra, model-releases, papers, rag, safety]
source: "../../../../archive/2026/06/22/digest/20260622-224238/daily.md"
---

# 2026-06-22 LLM 工程情报 Radar

> 面向中文 LLM / Agent 工程师，优先关注模型、Agent、RAG、评测、安全、推理和基础设施的工程价值。

## 快速入口

- [项目首页](../../../../README.md)
- [每日索引](../../../README.md)
- [主题索引](../../../../topics/README.md)
- [原始归档](../../../../archive/2026/06/22/README.md)

## 今日主线

- **P0** OpenAI 将“上线前部署仿真”作为评测方向推到台前
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-22) · [模型发布](../../../../topics/model-releases/index.md#2026-06-22) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-22) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-22)
  - 条目：[结构化记录](../../../../items/2026/06/22/daily/top-01-2026-06-16-deployment-simulation.md)
  - 源内容：[OpenAI: Deployment Simulation](https://openai.com/index/deployment-simulation)
  - 摘要：OpenAI 将“上线前部署仿真”作为评测方向推到台前：2026-06-16 发布的 Deployment Simulation 用真实会话数据模拟部署场景，在模型发布前预测行为与安全风险。这对工程团队的含义是：eval 不应只停留在静态题库，应加入匿名化真实流量回放、场景分层和工具调用回归。
- **P0** Agent/RAG 的上下文管理与流式工具调用开始被拆解为可工程化机制
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-22) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-22) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-22) · [论文](../../../../topics/papers/index.md#2026-06-22)
  - 条目：[结构化记录](../../../../items/2026/06/22/daily/top-02-agent-rag-2026-06-18.md)
  - 源内容：[arXiv: 2606.20047v1](https://arxiv.org/abs/2606.20047v1) · [arXiv: 2606.20113v1](https://arxiv.org/abs/2606.20113v1)
  - 摘要：Agent/RAG 的上下文管理与流式工具调用开始被拆解为可工程化机制：2026-06-18 arXiv 论文 PACMS 将 Agent 上下文选择建模为可插拔 submodular selection；Streaming RAG 论文指出只有当 tool intent 在用户输入结束前已稳定时...
- **P0** 端侧/实时 Agent Serving 需要超越 KV cache 的状态复用
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-22) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-22) · [论文](../../../../topics/papers/index.md#2026-06-22)
  - 条目：[结构化记录](../../../../items/2026/06/22/daily/top-03-agent-serving-kv-cache-2026.md)
  - 源内容：[arXiv: 2606.20537v1](https://arxiv.org/abs/2606.20537v1)
  - 摘要：端侧/实时 Agent Serving 需要超越 KV cache 的状态复用：2026-06-18 arXiv 的 Execution-State Capsules 将复用对象扩展到图绑定执行状态 checkpoint/restore，面向低延迟、小 batch、端侧物理 AI 的分支、重置、中...
- **P1** 评测从单轮题库继续走向部署仿真、多轮红队、多语言和领域专家任务
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-22) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-22) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-22) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-22)
  - 条目：[结构化记录](../../../../items/2026/06/22/daily/top-04-lifescibench-multi-lcb-livecodebench-nrt.md)
  - 源内容：[OpenAI: Introducing Life Sci Bench](https://openai.com/index/introducing-life-sci-bench) · [arXiv: 2606.20517v1](https://arxiv.org/abs/2606.20517v1) · [arXiv: 2606.20408v1](https://arxiv.org/abs/2606.20408v1)
  - 摘要：评测从单轮题库继续走向部署仿真、多轮红队、多语言和领域专家任务：LifeSciBench 面向生命科学专家任务；Multi-LCB 扩展 LiveCodeBench 到多语言；NRT-Bench 用模拟核电站控制室测试安全关键 Agent 的多轮对抗鲁棒性。

## 按主题阅读

- [Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-22)：4 条
- [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-22)：1 条
- [推理 / Serving](../../../../topics/inference/index.md#2026-06-22)：3 条
- [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-22)：1 条
- [模型发布](../../../../topics/model-releases/index.md#2026-06-22)：1 条
- [论文](../../../../topics/papers/index.md#2026-06-22)：2 条
- [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-22)：2 条
- [安全 / Alignment](../../../../topics/safety/index.md#2026-06-22)：1 条

## 原始归档

- [当日 archive index](../../../../archive/2026/06/22/README.md)
- [每日 digest 原文](../../../../archive/2026/06/22/digest/20260622-224238/daily.md)
