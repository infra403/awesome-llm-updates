# Awesome LLM Updates

面向中文 LLM / Agent 工程师的每日情报雷达。

每天自动追踪大模型、Agent、RAG、模型发布、论文、工程项目和技术博客，
把高噪音信息流压缩成可读、可追溯、方便检索的工程情报。

> Watch：用 GitHub 通知订阅每日 LLM 工程变化。
>
> Star：收藏一个持续更新的中文 LLM 工程情报库。

## 今日 Radar

最新日期：[**2026-06-23 LLM 工程情报 Radar**](daily/2026/06/23/index.md)

- **P0** [Agent runtime 正在产品化为“模型 + 执行环境 + 状态 + 权限边界”](items/2026/06/23/daily/top-01-agent-runtime.md)：Agent runtime 正在产品化为“模型 + 执行环境 + 状态 + 权限边界”：OpenAI 介绍 Responses API + shell tool + hosted containers（2026-03-11），Amazon Bedrock Stateful Runtime（2026-02-27）与 O...
- **P0** [Agent 安全成为今天最强主题](items/2026/06/23/daily/top-02-agent.md)：Agent 安全成为今天最强主题：OpenAI prompt injection 防护（2026-03-11）、instruction hierarchy/IH-Challenge（2026-03-10）、Codex Security research preview（2026-03-06）和 coding agen...
- **P0** [小模型/量化模型继续服务 coding、reasoning 与子代理负载](items/2026/06/23/daily/top-03-coding-reasoning.md)：小模型/量化模型继续服务 coding、reasoning 与子代理负载：Hugging Face 今日高优先级候选包括 reecdev/VibeThinker-3B-LQ8-GGUF（2026-06-23T00:03:13Z，MIT，P0）与 PGCodeLLM/AgenticRL-blackbox-260401_...
- **P1** [Coding/multi-agent 工具链升温](items/2026/06/23/daily/top-04-coding-multi-agent.md)：Coding/multi-agent 工具链升温：GitHub P0 项目集中在本地并行 agent、meta-harness、终端 agent、AI gateway 与 agent-native UI：superset-sh/superset、omnigent-ai/omnigent、gptme/gptme、env...
- **P1** [论文侧主线是垂直 agent 与可回滚/可学习的 agent 控制](items/2026/06/23/daily/top-05-agent-agent.md)：论文侧主线是垂直 agent 与可回滚/可学习的 agent 控制：GA-Rollback（2025-03-04）关注逐步检查与回滚，IDEA（2024-08-19）关注交互式规则学习，ClinicalAgent（2024-04-23）与药物发现 agent（2025-06-26）体现垂直工具链集成。来源：https...
- **P1** [评测信号](items/2026/06/23/daily/top-06-item-06.md)：评测信号：公开 coding benchmark 寿命缩短，安全闭环 benchmark 增多：OpenAI 表示不再评估 SWE-bench Verified 并建议转向 SWE-bench Pro（2026-02-23）；EVMbench（2026-02-18）强调发现、修复、利用/验证的闭环能力。来源：http...

## 为什么 Watch

- 每天自动更新，不需要手动刷 X、Hacker News、GitHub、Hugging Face、论文站和厂商博客。
- 面向工程落地筛选，不是泛 AI 新闻聚合；优先保留对架构、选型、评测、安全和部署有影响的信息。
- 每条重要信息都链接到日期归档和来源上下文，方便二次核验。
- 适合持续追踪 Agent runtime、coding agent、RAG、evals、安全、推理部署、多模态和 LLM infra。

## 为什么 Star

- 这是一个持续更新的中文 LLM 工程情报库，不是一次性 awesome-list。
- 同时保留每日阅读入口、主题索引、OKF-like 条目和原始 Hermes 归档。
- 后续可以直接基于 Git 历史做趋势回看、周报生成、主题复盘和团队知识库同步。

## 主题索引

- [Agent / Coding Agent](topics/agents/index.md)：Agent runtime、工具调用、MCP、多 Agent 协作、coding agent 与权限边界。
- [模型发布](topics/model-releases/index.md)：新模型、开源权重、量化版本、微调模型和可本地测试的候选模型。
- [RAG / Knowledge](topics/rag/index.md)：RAG、检索、知识库、长上下文、知识图谱和数据治理。
- [推理 / Serving](topics/inference/index.md)：推理部署、服务化、网关、吞吐、延迟、显存和本地运行。
- [评测 / Benchmarks](topics/evals/index.md)：评测集、benchmark、回归测试、私有 eval 和工程质量门禁。
- [安全 / Alignment](topics/safety/index.md)：Prompt injection、越权、防护、对齐、安全评测和 agent 行为监控。
- [多模态](topics/multimodal/index.md)：图像、视频、语音、3D、embodied agent 和多模态模型。
- [LLM Infra](topics/llm-infra/index.md)：LLM gateway、平台化、容器、Kubernetes、观测、成本和企业治理。
- [论文](topics/papers/index.md)：论文、arXiv、Semantic Scholar、研究趋势和可转工程 checklist 的方法。
- [开源项目](topics/open-source/index.md)：GitHub 项目、开源工具、工程框架和可落地 POC 候选。

## 最近更新

- [2026-06-23 Daily Radar](daily/2026/06/23/index.md) · [原始归档](archive/2026/06/23/README.md)
- [2026-06-22 Daily Radar](daily/2026/06/22/index.md) · [原始归档](archive/2026/06/22/README.md)

## 仓库结构

- `daily/YYYY/MM/DD/index.md`：每日情报阅读入口。
- `topics/<topic>/index.md`：按主题聚合的长期索引。
- `items/YYYY/MM/DD/daily/*.md`：OKF-like 知识条目，包含 frontmatter、重要性、标签和来源。
- `archive/YYYY/MM/DD/`：Hermes 原始巡检产物，保留 Markdown / JSON 证据。
- `state/`：同步状态，不存密钥。

## 生成说明

本仓库由 Hermes 定时任务自动生成。内容用于工程情报追踪，重要决策前仍应打开来源链接二次核验。
