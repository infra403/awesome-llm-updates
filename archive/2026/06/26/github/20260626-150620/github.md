## 2026-06-26 15:06 北京时间 | GitHub 项目巡检

本次只纳入候选报告中 8 小时窗口内有更新时间、且 priority_hint 为 P0/P1 的仓库；未读取 README 的条目均显式标注“README 未确认”。

### 1. CoWork-OS/CoWork-OS（P0）
- 仓库：CoWork-OS/CoWork-OS
- stars：365
- 更新时间：2026-06-26T07:02:00Z
- topics：ai-assistants, ai-automation, claude, desktop-app, discord-bot, electron, gemini, guardrails, llm, local-first, macos, mcp, model-context-protocol, openai, personal-ai, security, self-hosted, slack-bot, telegram, whatsapp-bot
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具；产品与商业化
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在 local-first 个人 agentic OS，把编码、知识工作、Web 设计、自动化和多渠道 bot 集成到桌面工作台。
- 一句话定位：Local-first 个人 agentic OS，把编码、知识工作、Web 设计、自动化和多渠道 bot 集成到桌面工作台。
- 解决的问题：个人/团队 AI 工作流分散在 IDE、聊天工具、MCP server 和自动化脚本中，缺少本地优先的统一操作面。
- 工程影响：可作为 Agent 工作台、MCP 接入、权限/guardrails 与本地数据边界设计的参考；对 LLM gateway 与桌面 agent 编排有方案借鉴价值。
- 成熟度判断：365 stars，topics 覆盖 MCP、security、self-hosted、Electron 与多渠道 bot，显示工程范围较完整；生产稳定性未确认。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，安装方式、真实 guardrails 能力和安全边界未确认。
- 建议动作：今天应阅读：P0 且覆盖 Agent OS + MCP + 安全/本地优先，适合快速判断是否纳入桌面 agent 技术储备。
- URL：https://github.com/CoWork-OS/CoWork-OS

### 2. sachitrafa/YourMemory（P0）
- 仓库：sachitrafa/YourMemory
- stars：247
- 更新时间：2026-06-26T07:03:08Z
- topics：agent-memory, ai-agents, claude, devtools, ebbinghaus, llm-memory, mcp, mcp-server, memory, model-context-protocol, persistent-memory, pgvector, rag
- 重要性：P0
- 主题标签：Agent 与多智能体；RAG 与知识工程；评测与基准
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在面向 Agent 的长期记忆层，主张用 Ebbinghaus 遗忘曲线衰减并报告 LoCoMo 召回提升。
- 一句话定位：面向 Agent 的长期记忆层，主张用 Ebbinghaus 遗忘曲线衰减并报告 LoCoMo 召回提升。
- 解决的问题：Agent 长期记忆容易无限膨胀、过时信息污染上下文，且缺少可解释的遗忘/保留策略。
- 工程影响：对 personal memory、MCP memory server、RAG recall/decay 策略有直接参考价值；可能影响记忆写入、检索排序和过期策略。
- 成熟度判断：247 stars，topics 指向 pgvector、MCP server、persistent memory；候选摘要提到 +16pp LoCoMo，但评测细节未确认。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，LoCoMo 实验设置、数据集切分和复现脚本未确认。
- 建议动作：今天应实验：记忆衰减策略可直接进入 Agent memory POC，先验证 API、存储结构和召回评测。
- URL：https://github.com/sachitrafa/YourMemory

### 3. iikarus/Dragon-Brain（P0）
- 仓库：iikarus/Dragon-Brain
- stars：50
- 更新时间：2026-06-26T07:04:01Z
- topics：ai-memory, claude, codex-cli, cursor, falkordb, gemini-cli, knowledge-graph, llm-tools, mcp, memory, model-agnostic, qdrant, vector-search
- 重要性：P0
- 主题标签：Agent 与多智能体；RAG 与知识工程；数据集与数据工程
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在用 MCP 暴露 Agent 长期记忆，组合知识图谱、向量检索和 GPU embedding，面向多种编码/聊天客户端。
- 一句话定位：用 MCP 暴露 Agent 长期记忆，组合知识图谱、向量检索和 GPU embedding，面向多种编码/聊天客户端。
- 解决的问题：单一向量库记忆难以表达实体关系，且不同 Agent/IDE 客户端之间缺少可共享的记忆层。
- 工程影响：对知识图谱 + Qdrant 混合记忆、MCP 工具设计、跨客户端共享上下文有工程参考；也能用于评估 graph memory 的维护成本。
- 成熟度判断：50 stars，但候选摘要声称 30 tools、1121 tests；topics 指向 FalkorDB、Qdrant、CUDA embeddings，工程依赖较重。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，测试数、工具数、部署复杂度和 GPU 依赖未确认。
- 建议动作：今天应阅读：概念与依赖组合值得看，但 stars 较低，先读架构和测试目录再决定 POC。
- URL：https://github.com/iikarus/Dragon-Brain

### 4. usemoss/moss（P0）
- 仓库：usemoss/moss
- stars：429
- 更新时间：2026-06-26T07:01:56Z
- topics：ai-agents, ai-infra, hybrid-search, rag, real-time, retrieval, semantic-search, voice-ai
- 重要性：P0
- 主题标签：RAG 与知识工程；推理系统与工程工具
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在生产 AI 系统检索层，主张无需向量数据库即可在浏览器、边缘、端侧和云侧做低延迟搜索。
- 一句话定位：生产 AI 系统检索层，主张无需向量数据库即可在浏览器、边缘、端侧和云侧做低延迟搜索。
- 解决的问题：RAG 检索依赖外部向量数据库时，端侧/边缘部署、冷启动、延迟和运维复杂度较高。
- 工程影响：可能影响轻量 RAG、on-device search、voice AI 实时检索和 Agent 本地知识库方案；值得与现有向量库路线对比。
- 成熟度判断：429 stars，topics 指向 hybrid-search、real-time、semantic-search；摘要声称 \<10ms，但基准环境未确认。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，\<10ms 测试条件、索引规模、召回质量和语言支持未确认。
- 建议动作：今天应实验：检索层替代向量库的主张很强，应用小语料和中等语料做延迟/召回 quick bench。
- URL：https://github.com/usemoss/moss

### 5. ayuayue/PiDeck（P0）
- 仓库：ayuayue/PiDeck
- stars：169
- 更新时间：2026-06-26T07:05:26Z
- topics：ai-agent, coding-agent, desktop-app, electron, pi, react, rpc, typescript
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在管理多个 pi coding-agent session 的桌面工作台，聚焦跨项目目录的编码 Agent 会话编排。
- 一句话定位：管理多个 pi coding-agent session 的桌面工作台，聚焦跨项目目录的编码 Agent 会话编排。
- 解决的问题：多编码 Agent 并行跑在不同项目目录时，终端/session/状态管理分散，缺少统一可视化控制台。
- 工程影响：对多 Agent 编码任务调度、session 生命周期、RPC 控制面和桌面 UX 有参考价值；可借鉴到内部 agent runner。
- 成熟度判断：169 stars，Electron/React/TypeScript topics 明确；仅针对 pi coding-agent 的适配深度和通用性未确认。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，支持的 agent 类型、隔离模型、日志/权限控制未确认。
- 建议动作：持续观察：适用场景明确，但需要先确认是否只绑定特定 pi agent，暂不立即接入。
- URL：https://github.com/ayuayue/PiDeck

### 6. huabeitech/agent-desk（P0）
- 仓库：huabeitech/agent-desk
- stars：150
- 更新时间：2026-06-26T07:00:36Z
- topics：ai-agent, chatbot, customer-service, customer-support, customer-support-ai, golang, helpdesk, knowledge-base, live-chat, rag
- 重要性：P0
- 主题标签：Agent 与多智能体；RAG 与知识工程；产品与商业化
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在开源 AI 客服系统，强调 AI-first 支持与人工接管流程。
- 一句话定位：开源 AI 客服系统，强调 AI-first 支持与人工接管流程。
- 解决的问题：客服场景需要把知识库 RAG、对话机器人、live chat 和人工运营整合，而不仅是单轮问答。
- 工程影响：可作为垂直 Agent 产品化样板，观察 RAG 知识库、human-in-the-loop、会话分流和运营后台设计。
- 成熟度判断：150 stars，Go/helpdesk/live-chat/RAG topics 显示产品工程方向清晰；部署成熟度未确认。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，渠道集成、权限、多租户和知识库同步能力未确认。
- 建议动作：持续观察：业务场景明确，适合产品化参考；若要用于客服 POC 再深入部署。
- URL：https://github.com/huabeitech/agent-desk

### 7. wazionapps/nexo（P1）
- 仓库：wazionapps/nexo
- stars：27
- 更新时间：2026-06-26T07:05:38Z
- topics：ai-memory, atkinson-shiffrin, autonomous-agent, claude-code, claude-code-plugin, codex, cognitive-architecture, knowledge-graph, local-first, mcp, mcp-server, memory, metacognition, model-context-protocol, natural-forgetting, rag, semantic-search, shared-brain, trust-scoring, vector-search
- 重要性：P1
- 主题标签：Agent 与多智能体；RAG 与知识工程
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在本地优先的 Agent 共享记忆/大脑，强调自然遗忘、元认知 guard、trust scoring 和 MCP 工具。
- 一句话定位：本地优先的 Agent 共享记忆/大脑，强调自然遗忘、元认知 guard、trust scoring 和 MCP 工具。
- 解决的问题：多个 coding agents 或 MCP client 缺少共享的可信记忆层，且很难处理遗忘、可信度和跨会话上下文。
- 工程影响：对 shared memory、trust scoring、metacognitive guard 设计有启发；可用于对比 YourMemory/Dragon-Brain 的记忆架构。
- 成熟度判断：27 stars，候选质量因弱 GitHub engagement 被限制为 P1；topics 丰富但成熟度偏早期。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，150+ MCP tools、trust scoring 实现和本地部署体验未确认。
- 建议动作：持续观察：概念密集但 stars 较低，先跟踪 README/示例成熟度，暂不投入大规模 POC。
- URL：https://github.com/wazionapps/nexo

### 8. IlhamriSKY/TEDI（P1）
- 仓库：IlhamriSKY/TEDI
- stars：39
- 更新时间：2026-06-26T07:03:13Z
- topics：ai, ai-agent, claude-code, cmd, code-editor, codex, open-source, opencode, powershell, rust, sftp, source-control, ssh, tauri, terminal
- 重要性：P1
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在轻量开发工作台，把 code editor、终端、SSH/SFTP、source control 与多个 coding agent 工具放在单窗口。
- 一句话定位：轻量开发工作台，把 code editor、终端、SSH/SFTP、source control 与多个 coding agent 工具放在单窗口。
- 解决的问题：开发者在 Claude Code、Codex、OpenCode、终端和源码管理之间频繁切换，缺少统一轻量 IDE shell。
- 工程影响：对 coding-agent IDE wrapper、Tauri/Rust 桌面集成、远程开发和 source-control 工作流有参考价值。
- 成熟度判断：39 stars，弱 engagement；topics 指向 Tauri/Rust/agent/terminal，但功能完整度和跨平台稳定性未确认。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，八个功能的实际完成度、agent 适配方式和安全模型未确认。
- 建议动作：持续观察：定位清楚但早期，适合作为开发工作台 UX 参考，不建议今天 POC。
- URL：https://github.com/IlhamriSKY/TEDI

### 9. trip2g/trip2g（P1）
- 仓库：trip2g/trip2g
- stars：17
- 更新时间：2026-06-26T07:04:29Z
- topics：ai-agents, digitalgarden, knowledge-base, mcp, obsidian, publishing-platform, second-brain, self-hosted, selfhosted, static-site-generator, telegrambot
- 重要性：P1
- 主题标签：Agent 与多智能体；RAG 与知识工程
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在开源 MCP knowledge mesh，把自托管 second brain 暴露给 AI agents，并支持与 peers 联邦。
- 一句话定位：开源 MCP knowledge mesh，把自托管 second brain 暴露给 AI agents，并支持与 peers 联邦。
- 解决的问题：个人知识库通常封闭在 Obsidian/静态站点中，Agent 访问和跨人/跨节点知识联邦能力不足。
- 工程影响：对 MCP 化知识库、federated knowledge mesh、digital garden 与 Agent 检索入口设计有参考。
- 成熟度判断：17 stars，弱 engagement；topics 指向 Obsidian、static-site-generator、Telegram bot，自托管生态取向明显。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，联邦协议、权限控制、同步冲突和 MCP 接口稳定性未确认。
- 建议动作：持续观察：知识联邦方向值得跟踪，但成熟度较低，暂不跟进工程接入。
- URL：https://github.com/trip2g/trip2g

### 10. bzsanti/oxidizePdf（P1）
- 仓库：bzsanti/oxidizePdf
- stars：179
- 更新时间：2026-06-26T07:01:05Z
- topics：ai, chunking, data-extraction, digital-signatures, document-processing, embeddings, encryption, invoice, langchain, llamaindex, ocr, pdf, pdf-generation, pdf-manipulation, pdf-parser, pdfa, rag, rust, table-extraction, text-extraction
- 重要性：P1
- 主题标签：RAG 与知识工程；数据集与数据工程
- 核心变化：本轮 8 小时巡检窗口内更新；候选元数据显示其近期活跃，定位集中在纯 Rust PDF 库，面向 AI/RAG 的结构感知 chunking、文本/表格抽取与 PDF 处理。
- 一句话定位：纯 Rust PDF 库，面向 AI/RAG 的结构感知 chunking、文本/表格抽取与 PDF 处理。
- 解决的问题：RAG 文档摄取中 PDF 解析、结构保留、表格抽取和无 C 依赖部署经常成为数据工程瓶颈。
- 工程影响：可能改善 PDF ingestion pipeline、结构化 chunking、LlamaIndex/LangChain 数据接入和边缘/服务端部署简化。
- 成熟度判断：179 stars，topics 覆盖 PDF parser/generation、table extraction、RAG、Rust；actionability 标记需要验证。
- 证据边界：证据来自候选元数据、stars、topics、更新时间；README 未确认，OCR 能力、复杂 PDF 兼容性、chunking API 和性能未确认。
- 建议动作：今天应实验：PDF RAG 摄取是高频痛点，建议用一份表格 PDF 和扫描 PDF 做解析质量 quick test。
- URL：https://github.com/bzsanti/oxidizePdf
