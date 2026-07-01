## 2026-07-02 03:06 北京时间 | GitHub 项目巡检

本次依据候选报告的 8 小时 recency window 过滤，只写入 P0/P1 且能解释工程价值的仓库；`Tomotsugu-dev/Hindsight` 偏个人时间追踪产品，LLM 工程相关性和 actionability 较弱，本轮不写入。

### 1. `fw-ai/cookbook`
- 仓库：`fw-ai/cookbook`
- stars：173
- 更新时间：2026-07-01T18:59:21Z
- topics：agentic-systems, ai-workflows, fireworks-ai, function-calling, generative-ai, integrations, jupyter-notebooks, machine-learning, production-examples, rag, tutorials
- 重要性：P0：Fireworks 官方/生态 cookbook，README 显示训练目录正在活跃开发，覆盖 RL、偏好优化、SFT 与部署链路。
- 主题标签：推理、训练与后训练；Agent 与多智能体；RAG 与知识工程
- 核心变化：近期更新落在本轮窗口；README 不只是泛化示例，而是把 actively developed 范围收敛到 training/，并提供 GRPO、DAPO、GSPO、CISPO、DPO、ORPO、SFT 等可运行训练 recipe，以及面向 agent 的 SKILL.md 入口。
- 一句话定位：Fireworks 上构建、微调、评测到部署生成式 AI 应用的工程 recipe 集。
- 解决的问题：降低团队把后训练/微调方案从 notebook 或样例迁移到生产训练脚本的成本。
- 工程影响：对后训练流水线、agent 自动微调、RAG/工具调用示例和 LLM gateway 的模型适配有直接参考价值；尤其适合评估 Fireworks Training SDK 是否能进入实验平台。
- 成熟度判断：stars 173；README 已确认；安装方式、目录结构和测试目录明确，但 cookbook 型项目成熟度仍取决于各 recipe 覆盖率与 Fireworks 平台绑定程度。
- 证据边界：证据来自候选元数据、GitHub README 与 topics；未实际运行 recipe，训练成本、账号权限、最新 API 兼容性未确认。
- 建议动作：今天应阅读：P0，建议先读 training/README.md 与 skills/fireworks-agent/SKILL.md，判断是否能复用到内部微调/部署闭环。
- URL：https://github.com/fw-ai/cookbook

### 2. `jeremylongshore/claude-code-plugins-plus-skills`
- 仓库：`jeremylongshore/claude-code-plugins-plus-skills`
- stars：2459
- 更新时间：2026-07-01T19:03:32Z
- topics：agent-skills, ai, ai-agents, anthropic, automation, claude-code, claude-code-plugins, developer-tools, devops, llm, marketplace, mcp, plugin-marketplace, plugin-system, saas, skills
- 重要性：P0：高 star 且近期更新，README 宣称是 Claude Code 插件/技能/agent marketplace，并带 CLI、validator 与公开规范。
- 主题标签：Agent 与多智能体；推理系统与工程工具；产品与商业化
- 核心变化：本轮窗口内更新；README 显示 catalog 规模已到数百 plugins、数千 skills、数百 agents，并强调 marketplace JSON、frontmatter、100 分 rubric 和 ccpi CLI 安装链路。
- 一句话定位：Claude Code 生态的插件、技能、agent 市场和包管理器。
- 解决的问题：解决 agent 工具生态分散、安装规范不一致、技能质量不可验证的问题。
- 工程影响：可影响内部 agent skill/plugin 注册表、MCP 工具分发、质量门禁与企业模板化 agent 工作流；也可作为“技能市场化”的竞品/参考实现。
- 成熟度判断：stars 2459；README 已确认；pnpm/ccpi 安装和 marketplace 入口明确；但主要面向 Claude Code，跨 agent 兼容性和供应链安全仍需审查。
- 证据边界：证据来自候选元数据、README 与 topics；未安装 ccpi，未审计 marketplace 中插件安全、维护者身份和执行权限。
- 建议动作：今天应实验：P0，建议安装 ccpi 到隔离环境，检查插件 schema、权限模型与 validator 是否可借鉴。
- URL：https://github.com/jeremylongshore/claude-code-plugins-plus-skills

### 3. `chrisliu298/awesome-llm-unlearning`
- 仓库：`chrisliu298/awesome-llm-unlearning`
- stars：603
- 更新时间：2026-07-01T16:56:59Z
- topics：ai-safety, alignment, awesome, awesome-list, evaluation, knowledge-erasure, large-language-model, llm, llm-safety, llm-unlearning, machine-learning, machine-unlearning, model-editing, nlp, paper-list, privacy, responsible-ai, right-to-be-forgotten, selective-forgetting, unlearning
- 重要性：P0：LLM unlearning 资料库，直接关系模型安全、隐私合规和知识擦除评测。
- 主题标签：评测与基准；推理、训练与后训练；模型发布与模型能力
- 核心变化：本轮窗口内更新；README 显示收录 588 篇论文、18 篇 survey/position、3 个 framework，并已包含 2026 ACL 条目和 code LLM API 演进相关 unlearning 论文。
- 一句话定位：面向 LLM 机器遗忘/知识擦除的论文、benchmark、framework 索引。
- 解决的问题：为“删除训练/记忆中的敏感、过期或侵权知识”提供技术路线和评测入口。
- 工程影响：对模型后训练、模型编辑、隐私删除请求、RAG/agent memory 的遗忘策略设计有研究与评测价值；更偏情报和 benchmark，不是即插即用工程库。
- 成熟度判断：stars 603；README 已确认；awesome-list 成熟度取决于维护频率和条目质量，工程可执行性低于框架项目。
- 证据边界：证据来自候选元数据、README 与 topics；未逐项核验 588 篇论文和 framework 可用性，代码/数据许可证未确认。
- 建议动作：今天应阅读：P0，建议优先抽取 benchmark/framework 条目，补到模型安全与记忆删除技术储备。
- URL：https://github.com/chrisliu298/awesome-llm-unlearning

### 4. `bug-ops/zeph`
- 仓库：`bug-ops/zeph`
- stars：41
- 更新时间：2026-07-01T19:02:23Z
- topics：a2a, acp, ai-agent, claude, cli, gemini, graph-memory, llm, local-llm, mcp, multi-agent, multi-model, ollama, openai, rag, rust, self-learning, semantic-memory, telegram-bot, tui
- 重要性：P1：低 star 但工程定位清晰，单 Rust binary 的 memory-first agent，覆盖本地/云模型、多模型路由与 MCP/ACP/A2A。
- 主题标签：Agent 与多智能体；RAG 与知识工程；推理系统与工程工具
- 核心变化：本轮窗口内更新；README 强调跨天/跨会话记忆、why 决策记忆、Graph memory、本地 Ollama 和团队聊天机器人集成，安装方式为 release install.sh + zeph init。
- 一句话定位：带长期图记忆和多模型路由的本地优先 AI agent。
- 解决的问题：缓解长周期任务中 agent 上下文丢失、项目决策理由不可追溯和工具链部署复杂的问题。
- 工程影响：可作为 agent memory、local-first agent、ACP/MCP 接口和 TUI/聊天入口的一体化参考；若实现扎实，可能影响 Hermes/Claude/OpenCode 类 agent 的持久记忆架构。
- 成熟度判断：stars 41；README 已确认；安装路径明确，但弱 GitHub engagement，发布质量、记忆检索准确性和 sandbox 安全性未确认。
- 证据边界：证据来自候选元数据、README 与 topics；未安装二进制，未验证 graph memory、A2A/ACP/MCP 兼容性和安全确认机制。
- 建议动作：持续观察：P1，建议等 release/issue 活跃度进一步稳定；可短时 POC 其 memory graph 设计。
- URL：https://github.com/bug-ops/zeph

### 5. `skynetcmd/m3-memory`
- 仓库：`skynetcmd/m3-memory`
- stars：14
- 更新时间：2026-07-01T19:03:39Z
- topics：agentic-memory, ai-agents, ai-memory, aider, claude-code, fips-140-3, gdpr, gemini, gemini-cli, homelab, local-llm, long-term-memory-llm, longmemeval, mcp, mcp-server, openclaw, privacy, rag, rag-memory, vector-search
- 重要性：P1：低 star 但命中 agent memory 基础设施方向，README 声称 bitemporal、矛盾管理、MCP API、FTS5 + vector + MMR。
- 主题标签：Agent 与多智能体；RAG 与知识工程；数据集与数据工程
- 核心变化：本轮窗口内更新；README 将 memory 定位为多 agent/多机器共享的长期知识库，并宣称 LongMemEval-S k=10 99.2% retrieval、离线/云两种模式、GDPR/FIPS 140-3 ready。
- 一句话定位：面向多 agent 的本地优先长期记忆框架与 MCP server。
- 解决的问题：解决不同 coding agent 各自记忆割裂、压缩前聊天日志丢失、历史版本和纠错时间线不可追踪的问题。
- 工程影响：对 RAG memory、agent 长期记忆、合规本地化部署和跨工具记忆共享有参考价值；可作为 Hermes/Claude/Gemini/OpenCode 共享 memory 层的 POC 对象。
- 成熟度判断：stars 14；README 已确认；安装方式存在，但 claim 很强、社区验证弱，benchmark 复现与安全合规声明需谨慎。
- 证据边界：证据来自候选元数据、README 与 topics；未复现 LongMemEval-S，未审计 FIPS/GDPR 声明，未验证 MCP 插件兼容性。
- 建议动作：今天应实验：P1，建议在隔离仓库跑 quickstart，重点验证写入/检索/冲突管理和 MCP 接口。
- URL：https://github.com/skynetcmd/m3-memory

### 6. `danieljustus/symaira-vault`
- 仓库：`danieljustus/symaira-vault`
- stars：22
- 更新时间：2026-07-01T19:04:41Z
- topics：age-encryption, agent-skills, ai-agents, claude-code, cli, codex-cli, golang, hermes-agent, hermes-skill, mcp, mcp-server, openclaw, openclaw-skill, opencode, own-your-data, password-manager, security
- 重要性：P1：AI agent 使用密钥/凭据的安全交互工具，MCP-ready，命中 agent 工具安全。
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：本轮窗口内更新；README 显示 age 加密、TOTP、剪贴板自动清除、secret execution、OS keyring cache、Git sync、多用户 vault、MCP stdio/HTTP 和面向 Claude/OpenCode/Hermes 的 slash commands。
- 一句话定位：带 MCP server 的终端密码管理器，用于 agent 安全使用凭据。
- 解决的问题：减少 agent 在聊天上下文中暴露密码/API key，并提供受控凭据注入与轮换工作流。
- 工程影响：对 agent 工具调用安全、MCP 权限边界、密钥注入、凭据轮换和零遥测本地工具链有参考价值；可作为内部 agent secret broker 方案备选。
- 成熟度判断：stars 22；README 已确认；Go CLI 和安装方式明确，但低 star，安全工具需要代码审计和恢复流程验证后才能使用。
- 证据边界：证据来自候选元数据、README 与 topics；未审计加密实现、MCP scope token、keyring 缓存和 Git sync 风险。
- 建议动作：持续观察：P1，安全类项目不宜直接接入生产；建议先代码审计，再做 sandbox POC。
- URL：https://github.com/danieljustus/symaira-vault

### 7. `AmirShayegh/codex-claude-bridge`
- 仓库：`AmirShayegh/codex-claude-bridge`
- stars：19
- 更新时间：2026-07-01T19:04:10Z
- topics：ai-code-review, claude-code, cli, code-review, codex, developer-tools, mcp, openai, precommit, typescript
- 重要性：P1：低 star 但工作流明确，把 Codex/Gemini 作为 Claude Code 的第二模型 code review MCP。
- 主题标签：Agent 与多智能体；评测与基准；推理系统与工程工具
- 核心变化：本轮窗口内更新；README 描述 Claude Code 写代码，Codex/Gemini 进行结构化 review 并回传，支持 provider failover；安装为 claude mcp add + npx 包。
- 一句话定位：为 Claude Code 接入 Codex/Gemini 自动 code review 的 MCP bridge。
- 解决的问题：解决单一 coding agent 自写自审可靠性不足，以及跨模型 review 需要复制粘贴的问题。
- 工程影响：对开发工作流、pre-commit 质量门禁、多模型协作和 MCP reviewer 工具设计有直接启发；也可用于比较 Codex/Gemini 作为审查模型的表现。
- 成熟度判断：stars 19；README 已确认；Node.js 18+、Claude Code、Codex/Gemini 登录前置明确，但社区采用度和 review 质量未确认。
- 证据边界：证据来自候选元数据、README 与 topics；未安装 npx 包，未验证 OAuth token 读取、failover 和结构化反馈格式。
- 建议动作：今天应实验：P1，建议用小型 PR 在隔离 repo 试跑，评估误报率和权限暴露面。
- URL：https://github.com/AmirShayegh/codex-claude-bridge

### 8. `GenAI-Security-Project/GenAI-LLM-Top10`
- 仓库：`GenAI-Security-Project/GenAI-LLM-Top10`
- stars：31
- 更新时间：2026-07-01T18:27:57Z
- topics：未提供 topics
- 重要性：P1：LLM 应用安全基线，工程 actionability 中等但权威性强。
- 主题标签：评测与基准；推理系统与工程工具
- 核心变化：本轮窗口内更新；README 显示其为 OWASP Top 10 for Large Language Model Applications 的 companion repository，面向开发者、数据科学家和安全专家。
- 一句话定位：OWASP LLM 应用 Top 10 风险清单的官方配套仓库。
- 解决的问题：为 LLM app/plugin/agent 的威胁建模、安全评审和上线检查提供通用风险分类。
- 工程影响：可影响 agent/MCP 工具权限、RAG 数据泄露、prompt injection、供应链与评测安全 checklist；更适合作为安全门禁与审查模板，不是功能库。
- 成熟度判断：stars 31；README 已确认；OWASP/GenAI Security Project 背书，但候选未提供 topics，仓库工程代码属性弱。
- 证据边界：证据来自候选元数据与 README；未确认当前 Top10 版本差异、具体条目变更和配套测试工具。
- 建议动作：今天应阅读：P1，建议把最新条目映射到内部 agent/RAG/MCP 安全 review checklist。
- URL：https://github.com/GenAI-Security-Project/GenAI-LLM-Top10
