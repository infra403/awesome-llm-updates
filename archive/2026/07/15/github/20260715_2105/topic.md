## 2026-07-15 21:05 GitHub 项目主题条目

### Agent 与多智能体

- GlitterKill/sdl-mcp（P0）：适用场景：可作为 Claude/Codex/Hermes 类 agentic coding 工作流的 context layer 或 MCP 工具层候选，影响代码图谱、检索、上下文裁剪和多语言代码理解链路。 成熟度：442 stars；topics 覆盖 tree-sitter、vector search、MCP、coding-agent；工程定位清晰但生产稳定性、索引成本、语言覆盖和与现有 IDE/CI 集成深度需 POC。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/GlitterKill/sdl-mcp
- flytohub/flyto-core（P0）：适用场景：可影响 Agent 编排、浏览器自动化、RPA、MCP server 注册、任务审计与 replay 设计；也可作为 LLM workflow engine 的架构参照。 成熟度：447 stars；声称 451 registry-backed modules；topics 包含 Playwright、security、workflow-engine；真实模块质量、权限隔离、长任务队列可靠性和 metering 机制需验证。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/flytohub/flyto-core
- Dryxio/auto-re-agent（P0）：适用场景：对安全 Agent、静态分析、代码恢复、二进制审计工作流有参考价值，也能启发“工具调用 + LLM 验证”的闭环设计。 成熟度：1039 stars；领域垂直且依赖 Ghidra/LLM；适用范围、准确率、验证基准、对不同架构/编译器的鲁棒性需确认。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/Dryxio/auto-re-agent

### 数据集与数据工程

- rasinmuhammed/misata（P0）：适用场景：可用于数据工程测试、RAG fixture 构造、评测样本扩增、数据库 seed 和 CI 中的确定性测试数据生成。 成熟度：63 stars；topics 覆盖 dbt、pytest、numpy/pandas、MCP server；规模化性能、隐私约束、分布控制和 schema 质量需实测。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/rasinmuhammed/misata
- LeastAction-Labs/LeastAction（P1）：适用场景：可作为数据集成平台、MCP 化数据工作流、self-hosted workflow automation 的观察对象；对 RAG 数据管线治理有间接价值。 成熟度：13 stars，候选标记 weak_github_engagement_cap；license、source-available 限制、连接器成熟度和部署方式需确认。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/LeastAction-Labs/LeastAction

### RAG 与知识工程

- mloda-ai/mloda（P0）：适用场景：可作为 RAG 数据接入、feature lineage、LLMOps/ML pipelines 的抽象层参考，尤其适合评估插件协议和 traceability 设计。 成熟度：72 stars；topics 覆盖 lineage、plugin-framework、rag、mlops；连接器覆盖、版本兼容、权限控制和观测指标需验证。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/mloda-ai/mloda
- ScrapeGraphAI/Scrapegraph-ai（P1）：适用场景：可影响 RAG ingest、web extraction、搜索增强、网页到 Markdown/结构化数据流程；也可作为 Firecrawl 替代方案评估对象。 成熟度：28387 stars，生态信号很强；但候选来自 Search/stars 且 actionability_needs_validation，近期具体变更、安装体验、反爬稳定性和模型成本需确认。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/ScrapeGraphAI/Scrapegraph-ai

### 推理系统与工程工具

- TencentCloudBase/CloudBase-MCP（P0）：适用场景：可影响 LLM coding agent 的部署工具调用、云资源编排、数据库接入、prompt-to-app devops 路径；对国内云生态尤其相关。 成熟度：1050 stars；云厂商/CloudBase 背景，topics 覆盖 database、PostgreSQL、Supabase、MCP；云账号权限、资源成本、可移植性和安全边界需确认。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/TencentCloudBase/CloudBase-MCP

### 评测与基准

- fboiero/MIESC（P1）：适用场景：可作为安全评测编排、多工具 orchestration、LLM/RAG 辅助漏洞 triage 的参考；对 Web3 安全团队更直接。 成熟度：11 stars，候选标记 weak_github_engagement_cap；虽然证据完整但社区采用度弱，工具安装复杂度和误报率需确认。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/fboiero/MIESC
- maxim-saplin/llm_chess（P1）：适用场景：可作为轻量 eval harness 或 reasoning benchmark 的参考，尤其用于比较模型在规则约束环境中的稳定性。 成熟度：110 stars；候选未给 topics；actionability_needs_validation，评测方法、样本规模、对棋力/记忆污染的控制需确认。 详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/maxim-saplin/llm_chess
