---
type: DailyRadar
date: "2026-06-26"
language: zh-CN
audience: "中文 LLM / Agent 工程师"
tags: [agents, evals, inference, llm-infra, model-releases, papers, rag, safety]
source: "../../../../archive/2026/06/26/digest/20260626-0936/daily.md"
---

# 2026-06-26 LLM 工程情报 Radar

> 面向中文 LLM / Agent 工程师，优先关注模型、Agent、RAG、评测、安全、推理和基础设施的工程价值。

## 快速入口

- [项目首页](../../../../README.md)
- [每日索引](../../../README.md)
- [主题索引](../../../../topics/README.md)
- [原始归档](../../../../archive/2026/06/26/README.md)

## 今日主线

- **P0** ShareLock：针对 MCP 的多工具阈值投毒攻击
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26) · [论文](../../../../topics/papers/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-01-sharelock-mcp-arxiv-2026-06.md)
  - 源内容：[arXiv: 2606.27027v1](https://arxiv.org/abs/2606.27027v1)
  - 摘要：ShareLock：针对 MCP 的多工具阈值投毒攻击：核心变化是 arXiv 2026-06-25 新增一篇 MCP 安全论文，指出随着 MCP 成为 Agent 调工具基础设施，攻击者可利用多工具、阈值式投毒绕过人工检查并在 LLM-server 交互中注入恶意提示；工程影响是所有使用 MCP...
- **P0** OpenRCA 2.0：从结果标签转向因果过程监督的 Agent RCA 评测
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-02-openrca-agent-rca-arxiv-2026.md)
  - 源内容：[arXiv: 2606.27154v1](https://arxiv.org/abs/2606.27154v1)
  - 摘要：OpenRCA 2.0：从结果标签转向因果过程监督的 Agent RCA 评测：核心变化是 arXiv 2026-06-25 新增 RCA/Agent 评测论文，提出 PAVE step-wise labeling protocol，试图把根因分析从“只猜最终 root cause”推进到“标注故...
- **P0** RAG 安全与隐私综述：把检索索引、查询日志、上下文构造纳入威胁面
  - 主题：[RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-03-rag-arxiv-2026-06-24.md)
  - 源内容：[arXiv: 2606.25533v1](https://arxiv.org/abs/2606.25533v1)
  - 摘要：RAG 安全与隐私综述：把检索索引、查询日志、上下文构造纳入威胁面：核心变化是 arXiv 2026-06-24 当前窗口候选给出 RAG 安全/隐私系统综述，强调风险不只在生成模型本身，也在检索 pipeline、索引、日志和 context construction；工程影响是企业 RAG 需...
- **P1** Hugging Face：一条命令在 HF Jobs 上运行 vLLM Server
  - 主题：[模型发布](../../../../topics/model-releases/index.md#2026-06-26) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-04-hf-jobs-vllm-server-blog.md)
  - 源内容：[Hugging Face: blog/vllm-jobs](https://huggingface.co/blog/vllm-jobs)
  - 摘要：Hugging Face：一条命令在 HF Jobs 上运行 vLLM Server：核心变化是 Hugging Face Blog 2026-06-26 新增 vLLM Jobs 教程，指向把 vLLM server 快速部署到 HF Jobs 的更低门槛路径；工程影响是对临时评测、demo、模...
- **P1** OpenAI：Agents are transforming work 研究/新闻稿
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-26) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-05-agents-are-transforming-work-news.md)
  - 源内容：[OpenAI: How Agents Are Transforming Work](https://openai.com/index/how-agents-are-transforming-work)
  - 摘要：OpenAI：Agents are transforming work 研究/新闻稿：核心变化是 OpenAI News 2026-06-25 发布关于 Agent 改变工作的研究文章，强调 Agent 正在承担更长、更复杂任务并扩展多角色生产力；工程影响是对团队 workflow 的启示大于模型...
- **P1** LLM-OS-Models/LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26) · [模型发布](../../../../topics/model-releases/index.md#2026-06-26) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26)
  - 条目：[结构化记录](../../../../items/2026/06/26/daily/top-06-llm-os-models-lfm2-8b.md)
  - 源内容：[Hugging Face: LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters](https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters)
  - 摘要：LLM-OS-Models/LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters：核心变化是 Hugging Face 2026-06-26T01:15:25Z 更新一个基于 LiquidAI/LFM2.5-8B-A1B 的 Agent/terminal-agent/...

## 按主题阅读

- [Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-26)：4 条
- [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-26)：5 条
- [推理 / Serving](../../../../topics/inference/index.md#2026-06-26)：1 条
- [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-26)：5 条
- [模型发布](../../../../topics/model-releases/index.md#2026-06-26)：2 条
- [论文](../../../../topics/papers/index.md#2026-06-26)：1 条
- [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-26)：3 条
- [安全 / Alignment](../../../../topics/safety/index.md#2026-06-26)：3 条

## 原始归档

- [当日 archive index](../../../../archive/2026/06/26/README.md)
- [每日 digest 原文](../../../../archive/2026/06/26/digest/20260626-0936/daily.md)
