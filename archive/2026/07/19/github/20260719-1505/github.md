## 2026-07-19 15:05 北京时间 | GitHub 项目巡检

### 1. terrylica/cc-skills

- **仓库**：terrylica/cc-skills
- **stars**：59
- **更新时间**：2026-07-19T07:01:57Z
- **topics**：ai-agents, ai-tools, anthropic, automation, claude, claude-code, clickhouse, coding-assistant, developer-tools, devops, llm, marketplace, mcp, open-source, plugins, productivity, prompt-engineering, semantic-release, skills, workflow
- **重要性**：P0
- **主题标签**：Agent 与多智能体；推理系统与工程工具
- **核心变化**：本周期内更新的 Claude Code Skills Marketplace，把 skills、plugins、DevOps 自动化、ClickHouse 管理、语义化发布和 productivity workflow 组织成可复用市场；README 显示其表格由 `.claude-plugin/marketplace.json` 生成，并提供 `bun scripts/validate-plugins.mjs` 校验入口，说明它不仅是列表，也在尝试做插件元数据的单一事实源管理。
- **一句话定位**：面向 Claude Code 的技能/插件市场与自修复式 autonomous-loop 原语集合。
- **解决的问题**：降低团队复用 Claude Code 工作流、沉淀工程技能和分发插件的成本，尤其适合把 ADR、发布、DevOps、数据库运维等重复任务固化为 agent 可调用能力。
- **工程影响**：可作为内部 Agent skill marketplace / tool registry 的参考，影响 Agent 编排层的能力发现、插件校验、技能版本化和开发工作流复用；如果团队已有 Hermes/Claude Code/Codex skill 体系，今天值得对比其 marketplace 元数据结构。
- **成熟度判断**：stars 59，仓库较新或影响面仍在早期；README 已确认存在 36 个 plugins badge、MIT license badge、package version badge和插件校验脚本说明，但安装方式、真实使用案例、兼容版本和插件质量未逐项确认。
- **证据边界**：证据来自候选更新时间、stars、topics 与 README 首屏；未实际安装或运行插件；插件表完整性、执行安全边界、Claude Code 版本兼容性未确认。
- **建议动作**：今天应阅读。理由：P0 且直接涉及 Agent skill/plugin 市场化，适合抽取 registry schema、插件校验和团队技能治理做法。
- **URL**：https://github.com/terrylica/cc-skills

### 2. nirholas/XActions

- **仓库**：nirholas/XActions
- **stars**：392
- **更新时间**：2026-07-19T07:03:51Z
- **topics**：ai-agent, automation, claude, gpt, mass-unfollow, mcp, mcp-server, model-context-protocol, nodejs, open-source, puppeteer, twitter, twitter-automation, twitter-bot, twitter-scraper, unfollow-tool, x, xactions
- **重要性**：P0
- **主题标签**：Agent 与多智能体；产品与商业化；数据集与数据工程
- **核心变化**：本周期内更新的 X/Twitter 自动化工具集，README 明确覆盖 Scrapers、MCP Server for AI Agents、CLI、Browser Scripts、Browser Extension，并强调不依赖 X API key / 月费；候选 metadata 显示它已有 392 stars，是本轮候选中较高关注度的 Agent-MCP 工具。
- **一句话定位**：把 X/Twitter 抓取与账号自动化封装为 CLI、浏览器脚本和 MCP Server 的 Node.js 工具箱。
- **解决的问题**：为 Claude/GPT 等 Agent 提供无需官方 API 的 X 数据采集、互动和账号管理接口，降低社媒监控、增长分析与自动化操作的接入门槛。
- **工程影响**：对内容监控、舆情/竞品追踪、Agent 数据采集链路和 MCP 工具接入有直接参考价值；但自动 follow/like/comment/scrape 等能力有平台合规、账号风控和安全审计风险，不能直接进入生产自动化。
- **成熟度判断**：stars 392；README 已确认 npm badge、MCP Server、CLI、browser scripts/extension 等入口；但未实际安装，浏览器自动化稳定性、登录态管理、限流策略、平台 ToS 合规性和数据质量未确认。
- **证据边界**：证据来自候选更新时间、stars、topics 与 README 首屏；未运行抓取或 MCP server；是否违反平台规则、是否存在封号风险、是否适合企业环境均未确认。
- **建议动作**：今天应实验。理由：P0 且 MCP + 社媒数据采集对 Agent 外部情报能力有直接影响，但必须在隔离账号和合规边界下 POC。
- **URL**：https://github.com/nirholas/XActions

### 3. chuckwu0/larkway

- **仓库**：chuckwu0/larkway
- **stars**：11
- **更新时间**：2026-07-19T07:04:54Z
- **topics**：ai-agent, chatbot, claude, claude-code, codex, coding-agent, devtools, feishu, feishu-bot, lark, lark-bot, llm
- **重要性**：P1
- **主题标签**：Agent 与多智能体；推理系统与工程工具；产品与商业化
- **核心变化**：本周期内更新，定位为把 Claude Code / Codex 订阅变成团队可在飞书中 @ 的 Agent。README 已确认当前 release 为 v0.3.60，并说明 bot 在用户机器上运行、可读取真实 codebase、执行命令、打开 MR，再把结果回写飞书线程。
- **一句话定位**：面向飞书线程的本地代码 Agent 网关，把 Claude Code/Codex 暴露成团队协作 bot。
- **解决的问题**：让非工程成员通过飞书直接询问代码实现、指标口径、API 位置或复现上下文，减少工程师人工解释和粘贴代码的协作成本。
- **工程影响**：对“企业 IM + 本地代码执行 Agent”的产品化路径有参考价值，尤其影响 Feishu bot 消息桥接、权限隔离、工作区上下文注入、命令执行安全和 MR 自动化流程；也可作为 Hermes/Lark 集成体验的竞品/生态观察对象。
- **成熟度判断**：stars 11，社区成熟度弱；README 已确认 release、运行模式和飞书线程交互设计；安装部署复杂度、权限模型、审计日志、MR 平台支持和多用户隔离未确认。
- **证据边界**：证据来自候选更新时间、stars、topics 与 README 首屏；未实际部署；安全沙箱、凭据隔离、企业权限审批和生产稳定性未确认。
- **建议动作**：持续观察。理由：定位清晰且与飞书/代码 Agent 场景高度相关，但 stars 低，适合跟踪产品形态和权限设计，暂不直接依赖。
- **URL**：https://github.com/chuckwu0/larkway

### 4. AlexsJones/repo-steward

- **仓库**：AlexsJones/repo-steward
- **stars**：19
- **更新时间**：2026-07-19T06:56:50Z
- **topics**：ai-agent, claude-code, developer-tools, github-automation, maintainer-tools, open-source-maintenance, repository-management
- **重要性**：P1
- **主题标签**：Agent 与多智能体；推理系统与工程工具
- **核心变化**：本周期内更新的开源仓库维护 Agent。README 明确其目标是按计划或按钮触发，自动处理 issue triage、多轮 PR review、仓库讨论、bug-fix PR、网站监控，并通过 dashboard 只把 tie-break 和设计决策升级给维护者；同时强调 draft mode 默认开启、不会自行 merge/close。
- **一句话定位**：面向开源维护者的自主仓库运营 Agent，覆盖 issue/PR/讨论/网站监控闭环。
- **解决的问题**：减少维护者在 PR diff、issue triage、重复回复和例行检查中的手工循环，把低风险操作草拟出来，把关键决策留给人。
- **工程影响**：对 GitHub automation agent 的安全边界设计有参考价值，尤其是 draft-first、人类终态、dashboard escalation、多 backend（Claude Code/Codex/Gemini/opencode）等模式；可启发内部 repo bot 的权限分层和审批流。
- **成熟度判断**：stars 19，仍处早期；README 已确认核心功能愿景、默认 draft mode 和 AI backend badge；但安装方式、GitHub App/OAuth 权限、真实端到端 demo、任务调度可靠性和安全审计未确认。
- **证据边界**：证据来自候选更新时间、stars、topics 与 README 首屏；未运行；是否已有可用 release、支持哪些 GitHub 事件、如何处理 hallucinated review 未确认。
- **建议动作**：持续观察。理由：P1 且安全设计方向值得借鉴，但社区信号弱，应先观察实现成熟度再 POC。
- **URL**：https://github.com/AlexsJones/repo-steward

### 5. guihuashaoxiang/FreeLLM-API-KeyHub

- **仓库**：guihuashaoxiang/FreeLLM-API-KeyHub
- **stars**：154
- **更新时间**：2026-07-19T06:36:20Z
- **topics**：aigc, awesome-list, china, developer-tools, free-llm-api
- **重要性**：P1
- **主题标签**：模型发布与模型能力；产品与商业化；推理系统与工程工具
- **核心变化**：本周期内更新的国内免费 LLM API 资源汇总。README 已确认项目不提供 API Key，只整理官方公开免费资源，并列出硅基流动、火山方舟等平台的注册福利、额度、有效期、前置条件和备注；候选 reason_codes 标记为 actionability_needs_validation。
- **一句话定位**：面向中国开发者的免费/限时 LLM API 资源与接入情报列表。
- **解决的问题**：帮助工程团队快速发现低成本模型调用渠道，尤其适合 demo、POC、评测样例和备选供应商调研。
- **工程影响**：对 LLM gateway 的 provider inventory、成本策略、免费额度试用、国内模型接入路线有参考价值；但免费额度变化快，不能把该列表当作稳定 SLA 或生产供应商依据。
- **成熟度判断**：stars 154；README 已确认资源表格和“官方公开资源”边界；但每个平台额度是否仍有效、API 兼容性、密钥申请流程、地域/实名要求、速率限制和商业使用限制未逐项验证。
- **证据边界**：证据来自候选更新时间、stars、topics 与 README 首屏；未点击每个供应商官网，也未实际申请或调用 API；免费额度与条款可能随时变化。
- **建议动作**：今天应阅读。理由：P1 且可补充 LLM gateway 供应商备选清单，但进入 POC 前必须逐项验证官网条款和调用链路。
- **URL**：https://github.com/guihuashaoxiang/FreeLLM-API-KeyHub

### 6. Gloriaameng/Awesome-Agent-Harness

- **仓库**：Gloriaameng/Awesome-Agent-Harness
- **stars**：306
- **更新时间**：2026-07-19T05:54:27Z
- **topics**：agent, agent-framework, agent-harness, awesome-list, harness, harness-engineering, llm
- **重要性**：P1
- **主题标签**：Agent 与多智能体；评测与基准；推理系统与工程工具
- **核心变化**：本周期内更新的 Agent Harness survey/awesome repo。README 已确认其把 agent execution harness 建模为 H = (E, T, C, S, L, V)，覆盖 110+ papers/blogs/reports、23 systems 和 9 个开放技术挑战，并提供论文、preprints、HuggingFace Dataset 链接。
- **一句话定位**：围绕 LLM Agent harness 工程的论文/系统综述和资料库。
- **解决的问题**：为 Agent 可靠性工程提供结构化分类框架，帮助团队把模型、工具、上下文、状态、日志、验证等 harness 组件分开讨论和评估。
- **工程影响**：对 Agent 平台架构评审、评测指标设计、runtime/harness 分层、可靠性复盘和技术雷达建设有参考价值；更偏知识工程与评测框架，不是可直接部署的工具。
- **成熟度判断**：stars 306；README 已确认 v3、150+ papers badge、CC-BY-4.0 license badge、paper/preprints/dataset 入口；但论文质量、分类覆盖、dataset 可用性和与实际工程栈的映射未验证。
- **证据边界**：证据来自候选更新时间、stars、topics 与 README 首屏；未阅读 PDF 全文；未验证 HuggingFace dataset 内容；不是生产组件。
- **建议动作**：今天应阅读。理由：P1 且有助于统一 Agent harness 术语和评测/可靠性框架，可作为架构讨论材料。
- **URL**：https://github.com/Gloriaameng/Awesome-Agent-Harness

### 未入选说明

- **bbruceyuan/Hands-On-Large-Language-Models-CN**：本周期内有更新且 stars 高，但候选 reason_codes 标记 actionability_weak；README 显示主要是《Hands-On Large Language Models》中文学习资料和 notebook/视频配套，偏教育内容，不直接影响本轮 Agent/RAG/MCP/推理系统/评测工程方案，因此本次不写入重点条目。
