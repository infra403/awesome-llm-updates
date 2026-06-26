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

最新日期：[**2026-06-26 LLM 工程情报 Radar**](daily/2026/06/26/index.md)

- **P0** [Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性](items/2026/06/26/daily/top-01-temporal-validity-in-retrieval-memory.md)：Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性：核心变化是论文指出传统 embedding 相似度无法可靠区分“重复事实”和“已过期/被推翻事实”，候选摘要给出 contradicted vs duplicated fact 的 AUROC 0.59（接近随...
- **P0** [MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架](items/2026/06/26/daily/top-02-mirror-agentic-rag-novelty-constrained.md)：MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架：核心变化是用 novelty-constrained memory-guided MCTS 生成更少重复的攻击样本，覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level tool manipul...
- **P0** [OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测](items/2026/06/26/daily/top-03-openrca-pave-rca-agent-root.md)：OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测：核心变化是候选摘要指出现有 RCA 数据集只标 root cause，容易退化成模式匹配；新协议强调 fault propagation path 的逐步标签；工程影响是 AIOps/可观测性 Agent、日志分析 Agen...
- **P1** [Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支](items/2026/06/26/daily/top-04-qwen-agentworld-35b-a3b-gguf.md)：Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支：核心变化是 HF 上新增/更新 FreedomAISVR 的 Qwen-AgentWorld-35B-A3B-NVFP4-GGUF 与 MXFP4-MOE-GGUF，标签包含 agent、world-mode...
- **P1** [GitHub Agent/RAG 工程栈集中活跃：Dify、RAGFlow、Neo.mjs、OpenLoomi](items/2026/06/26/daily/top-05-agent-rag-dify-ragflow-neo.md)：GitHub Agent/RAG 工程栈集中活跃：Dify、RAGFlow、Neo.mjs、OpenLoomi：核心变化是 2026-06-26 20:51-21:34 北京时间窗口内，多条高星/明确工程元数据项目更新，覆盖 production-ready agentic workflow、Agentic RAG、...
- **P1** [HF Jobs 一行命令运行 vLLM Server](items/2026/06/26/daily/top-06-hf-jobs-vllm-server-blog.md)：HF Jobs 一行命令运行 vLLM Server：核心变化是 Hugging Face Blog 发布 “Run a vLLM Server on HF Jobs in One Command”，把 vLLM server 与 HF Jobs 的启动流程包装为更短路径；工程影响是临时 benchmark、演示、短...

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

- [2026-06-26 Daily Radar](daily/2026/06/26/index.md) · [原始归档](archive/2026/06/26/README.md)
- [2026-06-25 Daily Radar](daily/2026/06/25/index.md) · [原始归档](archive/2026/06/25/README.md)
- [2026-06-24 Daily Radar](daily/2026/06/24/index.md) · [原始归档](archive/2026/06/24/README.md)
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
