---
type: TopicIndex
topic: evals
title: "评测 / Benchmarks"
language: zh-CN
---

# 评测 / Benchmarks

评测集、benchmark、回归测试、私有 eval 和工程质量门禁。

## 最近 7 天趋势

- 最近 7 天自动归档 18 条，其中 P0/P1 18 条；优先打开带源链接的结构化记录二次核验。

## 今日新增信号

- **P0** [MIRROR：面向 Agentic RAG 的跨表面红队框架](../../items/2026/06/27/daily/top-01-mirror-agentic-rag-novelty-constrained.md)：MIRROR：面向 Agentic RAG 的跨表面红队框架：核心变化是提出 novelty-constrained、memory-guided MCTS，用于覆盖文本投毒、图像注入、direct-query attack 和 orche...
- **P0** [Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模](../../items/2026/06/27/daily/top-02-temporal-validity-in-retrieval-memory.md)：Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模：核心变化是把 stale-fact errors 明确为结构性检索问题：事实变更后，旧事实与新事实 embedding 相似度...
- **P0** [OpenRCA 2.0：从结果标签转向因果过程监督](../../items/2026/06/27/daily/top-03-openrca-root-cause-analysis-pattern.md)：OpenRCA 2.0：从结果标签转向因果过程监督：核心变化是针对 root cause analysis 任务，指出只标 root cause 容易退化成 pattern matching，并引入 PAVE step-wise labe...
- **P1** [Hugging Face Jobs 一行启动 vLLM Server](../../items/2026/06/27/daily/top-04-jobs-vllm-server-blog-hf.md)：Hugging Face Jobs 一行启动 vLLM Server：核心变化是 Hugging Face Blog 发布在 HF Jobs 中运行 vLLM server 的工程路径；工程影响是临时模型服务、benchmark、demo...

## 值得实验

- **P0** [MIRROR：面向 Agentic RAG 的跨表面红队框架](../../items/2026/06/27/daily/top-01-mirror-agentic-rag-novelty-constrained.md)
- **P0** [Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模](../../items/2026/06/27/daily/top-02-temporal-validity-in-retrieval-memory.md)
- **P0** [OpenRCA 2.0：从结果标签转向因果过程监督](../../items/2026/06/27/daily/top-03-openrca-root-cause-analysis-pattern.md)
- **P1** [Hugging Face Jobs 一行启动 vLLM Server](../../items/2026/06/27/daily/top-04-jobs-vllm-server-blog-hf.md)
- **P0** [Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性](../../items/2026/06/26/daily/top-01-temporal-validity-in-retrieval-memory.md)
- **P0** [MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架](../../items/2026/06/26/daily/top-02-mirror-agentic-rag-novelty-constrained.md)
- **P0** [OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测](../../items/2026/06/26/daily/top-03-openrca-pave-rca-agent-root.md)
- **P1** [HF Jobs 一行命令运行 vLLM Server](../../items/2026/06/26/daily/top-06-hf-jobs-vllm-server-blog.md)

## 持续观察

- 暂无 P2 观察条目。

## 历史条目

## 2026-06-27

- **P0** [MIRROR：面向 Agentic RAG 的跨表面红队框架](../../items/2026/06/27/daily/top-01-mirror-agentic-rag-novelty-constrained.md)：MIRROR：面向 Agentic RAG 的跨表面红队框架：核心变化是提出 novelty-constrained、memory-guided MCTS，用于覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level tool m...
- **P0** [Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模](../../items/2026/06/27/daily/top-02-temporal-validity-in-retrieval-memory.md)：Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模：核心变化是把 stale-fact errors 明确为结构性检索问题：事实变更后，旧事实与新事实 embedding 相似度接近，候选摘要报告 cosine sim...
- **P0** [OpenRCA 2.0：从结果标签转向因果过程监督](../../items/2026/06/27/daily/top-03-openrca-root-cause-analysis-pattern.md)：OpenRCA 2.0：从结果标签转向因果过程监督：核心变化是针对 root cause analysis 任务，指出只标 root cause 容易退化成 pattern matching，并引入 PAVE step-wise labeling protocol 来标注从故障...
- **P1** [Hugging Face Jobs 一行启动 vLLM Server](../../items/2026/06/27/daily/top-04-jobs-vllm-server-blog-hf.md)：Hugging Face Jobs 一行启动 vLLM Server：核心变化是 Hugging Face Blog 发布在 HF Jobs 中运行 vLLM server 的工程路径；工程影响是临时模型服务、benchmark、demo/评测环境可以更低摩擦地拉起 vLLM，...

## 2026-06-26

- **P0** [Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性](../../items/2026/06/26/daily/top-01-temporal-validity-in-retrieval-memory.md)：Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性：核心变化是论文指出传统 embedding 相似度无法可靠区分“重复事实”和“已过期/被推翻事实”，候选摘要给出 contradicted vs duplicated f...
- **P0** [MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架](../../items/2026/06/26/daily/top-02-mirror-agentic-rag-novelty-constrained.md)：MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架：核心变化是用 novelty-constrained memory-guided MCTS 生成更少重复的攻击样本，覆盖文本投毒、图像注入、direct-query attack 和 orchestrato...
- **P0** [OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测](../../items/2026/06/26/daily/top-03-openrca-pave-rca-agent-root.md)：OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测：核心变化是候选摘要指出现有 RCA 数据集只标 root cause，容易退化成模式匹配；新协议强调 fault propagation path 的逐步标签；工程影响是 AIOps/...
- **P1** [HF Jobs 一行命令运行 vLLM Server](../../items/2026/06/26/daily/top-06-hf-jobs-vllm-server-blog.md)：HF Jobs 一行命令运行 vLLM Server：核心变化是 Hugging Face Blog 发布 “Run a vLLM Server on HF Jobs in One Command”，把 vLLM server 与 HF Jobs 的启动流程包装为更短路径；工程...

## 2026-06-24

- **P0** [Agent-native memory 从“任务成功率黑盒”转向可拆解的数据管理系统评测](../../items/2026/06/24/daily/top-02-agent-native-memory-arxiv-2026.md)：Agent-native memory 从“任务成功率黑盒”转向可拆解的数据管理系统评测：核心变化是 arXiv 2026-06-23 论文 *Are We Ready For An Agent-Native Memory System?* 被标记为 P0、quality_sc...
- **P0** [SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断](../../items/2026/06/24/daily/top-03-sherloc-agent-arxiv-2026-06.md)：SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断：核心变化是 arXiv 2026-06-23 论文 *SHERLOC: Structured Diagnostic Localization for Code Repair Agents* 被标记为...
- **P0** [RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒](../../items/2026/06/24/daily/top-04-rag-arxiv-2026-06-23.md)：RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒：核心变化是两篇 arXiv 2026-06-23 P0 论文同时进入窗口：*Privacy-Preserving RAG via Multi-Agent Semantic Rewriting*（quality_score...
- **P0** [开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新](../../items/2026/06/24/daily/top-06-llm-agent-workflow-coding-p0.md)：开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新：核心变化是 GitHub 8 小时窗口内 P0 仓库包括 comet-ml/opik（quality_score=20，updated 2026-06-24T...

## 2026-06-23

- **P0** [Concordia：面向长运行 LLM Agent/Serving 的 GPU 常驻状态容错 checkpointing](../../items/2026/06/23/daily/top-01-concordia-llm-agent-serving-gpu.md)：Concordia：面向长运行 LLM Agent/Serving 的 GPU 常驻状态容错 checkpointing：核心变化是 arXiv 2026-06-22 新增论文提出 JIT-compiled persistent-kernel checkpointing，目标覆...
- **P0** [RAG retrieval-state lock-in：一致答案不等于可信答案](../../items/2026/06/23/daily/top-02-rag-retrieval-state-lock-in.md)：RAG retrieval-state lock-in：一致答案不等于可信答案：核心变化是 arXiv 2026-06-22 新增论文指出 black-box uncertainty/多采样一致性在 RAG 中会被“同一个错误检索状态”锁定，空检索或错误邻域都可能产生稳定但错误...
- **P0** [Opik / Mastra / Dify：Agent/RAG/LLMOps 工具链在同一窗口高活跃](../../items/2026/06/23/daily/top-04-opik-mastra-dify-agent-rag.md)：Opik / Mastra / Dify：Agent/RAG/LLMOps 工具链在同一窗口高活跃：核心变化是 GitHub 当前 8 小时窗口内多个 P0 工具仓库更新：comet-ml/opik（2026-06-23T13:35Z，19,731 stars，LLM/RAG/...
- **P1** [Litmus：用代码驱动、零标签 metric specification 评估 AI 系统](../../items/2026/06/23/daily/top-05-litmus-metric-specification-ai-arxiv.md)：Litmus：用代码驱动、零标签 metric specification 评估 AI 系统：核心变化是 arXiv 2026-06-22 新增论文提出 zero-label、code-driven metric specification，用于评估 AI/Agent 系统；工...
- **P1** [CUGA working examples：轻量 harness 上的 agentic app 样例集](../../items/2026/06/23/daily/top-06-cuga-working-examples-harness-agentic.md)：CUGA working examples：轻量 harness 上的 agentic app 样例集：核心变化是 Hugging Face Blog 2026-06-23 发布 IBM Research 文章，称基于 CUGA 提供 two dozen working exa...

## 2026-06-22

- **P1** [评测从单轮题库继续走向部署仿真、多轮红队、多语言和领域专家任务](../../items/2026/06/22/daily/top-04-lifescibench-multi-lcb-livecodebench-nrt.md)：评测从单轮题库继续走向部署仿真、多轮红队、多语言和领域专家任务：LifeSciBench 面向生命科学专家任务；Multi-LCB 扩展 LiveCodeBench 到多语言；NRT-Bench 用模拟核电站控制室测试安全关键 Agent 的多轮对抗鲁棒性。


## 导航

- [主题首页](../README.md)
- [项目首页](../../README.md)
