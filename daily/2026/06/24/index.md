---
type: DailyRadar
date: "2026-06-24"
language: zh-CN
audience: "中文 LLM / Agent 工程师"
tags: [agents, evals, inference, llm-infra, model-releases, open-source, rag, safety]
source: "../../../../archive/2026/06/24/digest/20260624-0935/daily.md"
---

# 2026-06-24 LLM 工程情报 Radar

> 面向中文 LLM / Agent 工程师，优先关注模型、Agent、RAG、评测、安全、推理和基础设施的工程价值。

## 快速入口

- [项目首页](../../../../README.md)
- [每日索引](../../../README.md)
- [主题索引](../../../../topics/README.md)
- [原始归档](../../../../archive/2026/06/24/README.md)

## 今日主线

- **P0** Poisoned Playbooks：RAG 安全智能体的知识投毒风险被具体化
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-24) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-01-poisoned-playbooks-rag-arxiv-published.md)
  - 源内容：[arXiv: 2606.24402v1](https://arxiv.org/abs/2606.24402v1)
  - 摘要：Poisoned Playbooks：RAG 安全智能体的知识投毒风险被具体化：arXiv 新论文（published: 2026-06-23，quality_score 18，P0）聚焦 AI security agents 使用 RAG 做漏洞分析/利用推理时，外部 write-up 被投毒后...
- **P0** Privacy-Preserving RAG：用多 Agent 语义重写降低敏感信息泄漏
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-24) · [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-02-privacy-preserving-rag-agent-arxiv.md)
  - 源内容：[arXiv: 2606.24623v1](https://arxiv.org/abs/2606.24623v1)
  - 摘要：Privacy-Preserving RAG：用多 Agent 语义重写降低敏感信息泄漏：arXiv 新论文（published: 2026-06-23，quality_score 18，P0）提出由隐私抽取、语义分析、重构三个 Agent 协作，对检索内容做语义重写，在保留上下文语义的同时去除敏...
- **P0** OpenAI 参与 advanced AI shared standards：评测与安全标准化信号增强
  - 主题：[评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-24) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-03-advanced-ai-shared-standards-news.md)
  - 源内容：[OpenAI: Helping Build Shared Standards For Advanced AI](https://openai.com/index/helping-build-shared-standards-for-advanced-ai)
  - 摘要：OpenAI 参与 advanced AI shared standards：评测与安全标准化信号增强：OpenAI News（published: 2026-06-23，quality_score 16，P0）称其支持 Appia Foundation 相关的先进 AI 共享标准、评测框架、安全...
- **P0** 开源 Agent/LLM Infra 项目集中更新：workflow、memory、context budget 成为主线
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24) · [开源项目](../../../../topics/open-source/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-04-agent-llm-infra-workflow-memory.md)
  - 源内容：[GitHub: langgenius/dify](https://github.com/langgenius/dify) · [GitHub: melandlabs/openloomi](https://github.com/melandlabs/openloomi) · [GitHub: GlitterKill/sdl-mcp](https://github.com/GlitterKill/sdl-mcp) · 其余 1 个见结构化记录
  - 摘要：开源 Agent/LLM Infra 项目集中更新：workflow、memory、context budget 成为主线：GitHub 当前窗口 P0 候选包括 Dify（updated: 2026-06-24T01:21:03Z，stars 146330，quality_score 20，P0...
- **P1** Hugging Face CUGA examples：轻量 harness 的 agentic app 样例增加
  - 主题：[Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24) · [模型发布](../../../../topics/model-releases/index.md#2026-06-24) · [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-05-cuga-examples-harness-agentic-app.md)
  - 源内容：[Hugging Face: blog/ibm-research](https://huggingface.co/blog/ibm-research/cuga-apps)
  - 摘要：Hugging Face CUGA examples：轻量 harness 的 agentic app 样例增加：Hugging Face Blog（published: 2026-06-23，quality_score 15，P1）介绍 IBM Research 的 CUGA，两打 workin...
- **P1** Transformers.js + proposed Cross-Origin Storage API：浏览器端模型缓存/共享存储值得关注
  - 主题：[模型发布](../../../../topics/model-releases/index.md#2026-06-24) · [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24) · [推理 / Serving](../../../../topics/inference/index.md#2026-06-24) · [安全 / Alignment](../../../../topics/safety/index.md#2026-06-24)
  - 条目：[结构化记录](../../../../items/2026/06/24/daily/top-06-transformers-js-proposed-cross-origin.md)
  - 源内容：[Hugging Face: blog/cross-origin-storage](https://huggingface.co/blog/cross-origin-storage)
  - 摘要：Transformers.js + proposed Cross-Origin Storage API：浏览器端模型缓存/共享存储值得关注：Hugging Face Blog（published: 2026-06-23，quality_score 15，P1）讨论在 Transformers.js...

## 按主题阅读

- [Agent / Coding Agent](../../../../topics/agents/index.md#2026-06-24)：4 条
- [评测 / Benchmarks](../../../../topics/evals/index.md#2026-06-24)：3 条
- [推理 / Serving](../../../../topics/inference/index.md#2026-06-24)：3 条
- [LLM Infra](../../../../topics/llm-infra/index.md#2026-06-24)：3 条
- [模型发布](../../../../topics/model-releases/index.md#2026-06-24)：2 条
- [开源项目](../../../../topics/open-source/index.md#2026-06-24)：1 条
- [RAG / Knowledge](../../../../topics/rag/index.md#2026-06-24)：4 条
- [安全 / Alignment](../../../../topics/safety/index.md#2026-06-24)：2 条

## 原始归档

- [当日 archive index](../../../../archive/2026/06/24/README.md)
- [每日 digest 原文](../../../../archive/2026/06/24/digest/20260624-0935/daily.md)
