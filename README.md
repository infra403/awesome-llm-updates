# Awesome LLM Updates

面向中文 LLM / Agent 工程师的每日情报雷达。

自动追踪大模型、Agent、RAG、模型发布、论文、工程项目和技术博客，并按日期、主题和结构化条目沉淀。

## 适合谁

- 需要持续追踪 Agent runtime、coding agent、RAG、evals、安全、推理部署、多模态和 LLM infra 的工程师。
- 希望把新闻、论文、模型卡和开源项目沉淀成可检索知识库的团队。
- 想通过 Git 历史回看技术趋势、生成周报或同步到内部知识库的人。

## 方法论

- 采集侧先做时间窗口过滤，再输出 `quality_score`、`priority_hint`、`reason_codes` 和证据字段。
- GitHub 生成侧只把具备当前窗口、明确来源链接和工程影响的条目写入 `daily/` 与 `items/`。
- P0 / P1 / P2 表示工程优先级：P0 可能影响近期选型或架构，P1 适合阅读/实验，P2 只作观察。
- 低信号周期不补数：如果本周期只有 0-2 条强信号，daily 会直接说明，而不是塞入旧来源或泛 AI 新闻。

## 阅读入口

- [每日索引](daily/README.md)：按天查看当天主线、主题入口和原始归档。
- [主题索引](topics/README.md)：按 Agent、模型、RAG、评测、安全、推理等方向持续追踪。
- [原始归档](archive/)：保留 Hermes 每次巡检的 Markdown / JSON 证据。

## 最新更新

最新日期：[**2026-06-23 LLM 工程情报 Radar**](daily/2026/06/23/index.md)

- **P0** [Concordia：面向长运行 LLM Agent/Serving 的 GPU 常驻状态容错 checkpointing](items/2026/06/23/daily/top-01-concordia-llm-agent-serving-gpu.md)：Concordia：面向长运行 LLM Agent/Serving 的 GPU 常驻状态容错 checkpointing：核心变化是 arXiv 2026-06-22 新增论文提出 JIT-compiled persistent-kernel checkpointing，目标覆盖 KV cache、request s...
- **P0** [RAG retrieval-state lock-in：一致答案不等于可信答案](items/2026/06/23/daily/top-02-rag-retrieval-state-lock-in.md)：RAG retrieval-state lock-in：一致答案不等于可信答案：核心变化是 arXiv 2026-06-22 新增论文指出 black-box uncertainty/多采样一致性在 RAG 中会被“同一个错误检索状态”锁定，空检索或错误邻域都可能产生稳定但错误的高一致回答；工程影响在于 RAG 评测...
- **P0** [Agentic local model release cluster：Gemma/Fabliq 系列强调 tool-use、terminal、coding-agent](items/2026/06/23/daily/top-03-agentic-local-model-release-cluster.md)：Agentic local model release cluster：Gemma/Fabliq 系列强调 tool-use、terminal、coding-agent：核心变化是 Hugging Face 在当前 10 小时模型窗口出现多个 P0 模型更新，包括 tepirale/gemma-4-12B-agent...
- **P0** [Opik / Mastra / Dify：Agent/RAG/LLMOps 工具链在同一窗口高活跃](items/2026/06/23/daily/top-04-opik-mastra-dify-agent-rag.md)：Opik / Mastra / Dify：Agent/RAG/LLMOps 工具链在同一窗口高活跃：核心变化是 GitHub 当前 8 小时窗口内多个 P0 工具仓库更新：comet-ml/opik（2026-06-23T13:35Z，19,731 stars，LLM/RAG/agent tracing、eval、m...
- **P1** [Litmus：用代码驱动、零标签 metric specification 评估 AI 系统](items/2026/06/23/daily/top-05-litmus-metric-specification-ai-arxiv.md)：Litmus：用代码驱动、零标签 metric specification 评估 AI 系统：核心变化是 arXiv 2026-06-22 新增论文提出 zero-label、code-driven metric specification，用于评估 AI/Agent 系统；工程影响在评测平台和 CI gate：把评...
- **P1** [CUGA working examples：轻量 harness 上的 agentic app 样例集](items/2026/06/23/daily/top-06-cuga-working-examples-harness-agentic.md)：CUGA working examples：轻量 harness 上的 agentic app 样例集：核心变化是 Hugging Face Blog 2026-06-23 发布 IBM Research 文章，称基于 CUGA 提供 two dozen working examples；工程影响在 Agent 应用...

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
