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

最新日期：[**2026-06-27 LLM 工程情报 Radar**](daily/2026/06/27/index.md)

- **P0** [MIRROR：面向 Agentic RAG 的跨表面红队框架](items/2026/06/27/daily/top-01-mirror-agentic-rag-novelty-constrained.md)：MIRROR：面向 Agentic RAG 的跨表面红队框架：核心变化是提出 novelty-constrained、memory-guided MCTS，用于覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level tool manipulation，并指出既有红队模...
- **P0** [Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模](items/2026/06/27/daily/top-02-temporal-validity-in-retrieval-memory.md)：Temporal Validity in Retrieval Memory：RAG 记忆的时效性问题被单独建模：核心变化是把 stale-fact errors 明确为结构性检索问题：事实变更后，旧事实与新事实 embedding 相似度接近，候选摘要报告 cosine similarity 区分矛盾事实和重复事实...
- **P0** [OpenRCA 2.0：从结果标签转向因果过程监督](items/2026/06/27/daily/top-03-openrca-root-cause-analysis-pattern.md)：OpenRCA 2.0：从结果标签转向因果过程监督：核心变化是针对 root cause analysis 任务，指出只标 root cause 容易退化成 pattern matching，并引入 PAVE step-wise labeling protocol 来标注从故障到症状的传播路径；工程影响是评测 LLM...
- **P1** [Hugging Face Jobs 一行启动 vLLM Server](items/2026/06/27/daily/top-04-jobs-vllm-server-blog-hf.md)：Hugging Face Jobs 一行启动 vLLM Server：核心变化是 Hugging Face Blog 发布在 HF Jobs 中运行 vLLM server 的工程路径；工程影响是临时模型服务、benchmark、demo/评测环境可以更低摩擦地拉起 vLLM，而不必先维护长期 GPU 服务；建议动作...
- **P1** [InternScience/Agents-A1：Apache-2.0 的 Agent 向模型候选](items/2026/06/27/daily/top-05-internscience-agents-a1-apache-agent.md)：InternScience/Agents-A1：Apache-2.0 的 Agent 向模型候选：核心变化是 Hugging Face 在 2026-06-26T22:18:39Z 更新 InternScience/Agents-A1，标签包含 qwen3_5_moe、image-text-to-text、text-...
- **P0** [LLM-OS-Models/LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters：面向 terminal-agent 的 LoRA/adapter 信号](items/2026/06/27/daily/top-06-llm-os-models-lfm2-8b.md)：LLM-OS-Models/LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters：面向 terminal-agent 的 LoRA/adapter 信号：核心变化是 Hugging Face 在 2026-06-27T01:16:44Z 更新基于 LiquidAI/LFM2.5-8B-A...

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

- [2026-06-27 Daily Radar](daily/2026/06/27/index.md) · [原始归档](archive/2026/06/27/README.md)
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
