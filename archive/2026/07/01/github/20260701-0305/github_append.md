## 2026-07-01 03:05 北京时间 | GitHub 项目巡检

### 1. 0xSteph/pentest-ai
- 仓库：0xSteph/pentest-ai
- stars：1160
- 更新时间：2026-06-30T19:04:32Z
- topics：ai-security, bug-bounty, claude, ctf, cybersecurity, exploit, exploit-chaining, hacking-tools, mcp, model-context-protocol, nmap, offensive-security, osint, penetration-testing, pentest-ai, pentesting, python, red-team, security, vulnerability-scanner
- 重要性：P0
- 主题标签：Agent 与多智能体、评测与基准、推理系统与工程工具
- 核心变化：本周期窗口内更新的 offensive-security MCP/CLI 项目，把渗透测试工具、专门 agents 和 SPA-aware probes 组织成面向 LLM 的安全测试工作台；README 已确认其定位为“证明发现”的 pentest 工具，并展示 PyPI、Python 3.10+、CI 与许可徽章。
- 一句话定位：面向红队/漏洞验证的 MCP 安全工具编排层。
- 解决的问题：把 nmap、OSINT、OWASP Top 10 探测、漏洞验证等安全动作封装成可由 Agent 调用的工具链，降低安全测试工作流接入 LLM/MCP 的成本。
- 工程影响：对 Agent 工具权限、安全沙箱、MCP tool registry、审计日志和“LLM 触发危险动作”的策略设计有直接参考价值；也适合作为内部安全评测/红队自动化的 POC 样本。
- 成熟度判断：stars 已过千，README 有 PyPI/CI/许可证信号，候选摘要给出 205 wrapped tools、17 specialist agents、60 probes；但真实覆盖率、误报率、危险操作隔离和企业合规仍需本地验证。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；工具数量和 agent 数来自候选摘要，未逐项审计；安装和运行路径除 README 徽章外未实测。
- 建议动作：今天应实验。理由：安全 MCP 工具链可能直接影响内部 Agent 安全评测与红队自动化方案，需尽快验证权限边界和可控性。
- URL：https://github.com/0xSteph/pentest-ai

### 2. mohitagw15856/pm-claude-skills
- 仓库：mohitagw15856/pm-claude-skills
- stars：1100
- 更新时间：2026-06-30T19:04:48Z
- topics：agent-skills, ai-agents, chatgpt, claude-ai, claude-code, claude-skills, codex, cursor, gemini, hermes-agent, llm-tools, mcp, product-management, product-manager, productivity, prompt-engineering, skill-md, skills, slash-commands, subagents
- 重要性：P0
- 主题标签：Agent 与多智能体、产品与商业化、推理系统与工程工具
- 核心变化：本周期窗口内更新，候选摘要称其进入 Anthropic 官方 Claude plugin directory，并提供跨 Claude、ChatGPT、Gemini、Cursor、Codex 的专业 Agent Skills；README 已确认标题为 391 Professional Agent Skills，并展示 npm、PyPI、MCP/Remote MCP 等安装和分发信号。
- 一句话定位：产品管理与业务流程导向的 Agent Skill/插件集合。
- 解决的问题：把 PRD、launch、合规、简历等产品/运营任务沉淀为可复用 skill，尝试把“提示词/流程模板”产品化并跨多个 AI 编程/助手生态分发。
- 工程影响：对内部 skill 目录治理、跨 Agent skill 包格式、MCP/Remote MCP 分发、技能质量评测和企业 prompt/skill 资产管理有参考价值。
- 成熟度判断：stars 过千，README 展示 npm/PyPI/MCP 多通道分发；但 skill 数量、官方目录状态、质量一致性和安全审计未逐项验证。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；“官方目录”来自候选与 README badge，未到 Anthropic 目录二次核验；安装未实测。
- 建议动作：今天应阅读。理由：它代表 skill marketplace/agent workflow packaging 的快速演化，应抽样研究其 skill 结构和分发方式。
- URL：https://github.com/mohitagw15856/pm-claude-skills

### 3. osaurus-ai/osaurus
- 仓库：osaurus-ai/osaurus
- stars：6479
- 更新时间：2026-06-30T19:04:03Z
- topics：anthropic, apple-foundation-models, apple-intelligence, apple-neural-engine, llm, mcp, mcp-server, mlx, openai, swift
- 重要性：P0
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：本周期窗口内更新，README 已确认其定位为 macOS 本地 AI harness，强调 agents、memory、tools、identity 均在 Mac 本地运行，Swift 实现、离线、开源，并提供 release badge。
- 一句话定位：macOS 端侧 Agent 运行时与本地 AI 控制面。
- 解决的问题：将模型接入、长期记忆、工具调用和身份能力从云端服务下沉到本地 Mac，服务于隐私敏感或离线场景下的 Agent 执行。
- 工程影响：对本地 Agent runtime、端侧 memory store、MCP server、本地模型/Apple Neural Engine/MLX 结合、密钥与身份隔离方案有参考意义。
- 成熟度判断：stars 最高，README 有 release 信号和明确平台边界；但仅 macOS/Swift 路线，跨平台可复用性、插件 API 稳定性和真实 autonomous execution 能力需验证。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；“cryptographic identity”等细节来自候选摘要，未从源码审计；安装未实测。
- 建议动作：今天应阅读。理由：端侧 Agent harness 与本地隐私架构对桌面 Agent 方向有高参考价值，但先阅读架构再决定 POC。
- URL：https://github.com/osaurus-ai/osaurus

### 4. corezoid/corezoid-ai-plugin
- 仓库：corezoid/corezoid-ai-plugin
- stars：67
- 更新时间：2026-06-30T19:05:11Z
- topics：ai-plugin, api-orchestration, claude-code, claude-plugin, codex, codex-plugin, corezoid, developer-tools, mcp, process-engine, workflow-automation
- 重要性：P0
- 主题标签：Agent 与多智能体、推理系统与工程工具、产品与商业化
- 核心变化：本周期窗口内更新，README 已确认它是 Corezoid 面向 Claude Code 与 Codex 的插件，通过 MCP 让 Claude 访问 Corezoid 流程，并内置多个平台 skill 覆盖初始化、创建、编辑、审查和部署工作流。
- 一句话定位：企业流程平台的 AI-native MCP 管理层。
- 解决的问题：把 Corezoid 的 process engine、schema、模板和操作手册封装为 agent 可调用的 MCP tools + skills，使自然语言驱动工作流创建/部署成为可能。
- 工程影响：对“垂直 SaaS/流程平台如何接入 Claude Code/Codex”的插件形态、领域 skill 设计、MCP 工具权限和生产流程发布审计有借鉴价值。
- 成熟度判断：stars 较低但定位清晰，README 有 Go MCP server、技能列表和工作流描述；真实企业生产可用性、权限模型和部署安全未确认。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；候选摘要中的 marketplace/模板等范围未逐项验证；安装未实测。
- 建议动作：持续观察。理由：垂直平台插件化方向重要，但当前开源热度较低，适合跟踪其 MCP/skill 结构而非立即集成。
- URL：https://github.com/corezoid/corezoid-ai-plugin

### 5. speakeasy-api/gram
- 仓库：speakeasy-api/gram
- stars：251
- 更新时间：2026-06-30T19:03:36Z
- topics：agents, aisdk, clis, golang, mcp, mcp-gateway, mcp-server, mcp-servers, mcp-tools, openapi, openrouter, serverless, skills, typescript
- 重要性：P0
- 主题标签：Agent 与多智能体、推理系统与工程工具、产品与商业化
- 核心变化：本周期窗口内更新，README 已确认 Gram/Speakeasy AI Control Plane 的定位是“Securely scale AI usage across your organization”，强调面向 humans and agents 的控制平面。
- 一句话定位：组织级 AI/MCP/Agent 控制平面与分发栈。
- 解决的问题：为企业内部连接、保护、观测和分发 agents、MCP servers、skills 提供统一栈，特别适合 OpenAPI/MCP 工具规模化治理。
- 工程影响：对 LLM gateway、MCP gateway、OpenAPI-to-tool、组织级权限、可观测性和工具目录治理有直接参考价值。
- 成熟度判断：stars 中等，Speakeasy 背景强，topics 覆盖 MCP gateway、OpenRouter、serverless、TypeScript/Go；但开源边界、商业托管依赖和完整部署路径需确认。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；候选摘要中的 Connect/Secure/Observe/Distribute 细节未实测；安装未实测。
- 建议动作：今天应阅读。理由：MCP/agent 组织级控制平面是近期工程热点，需评估其架构能否映射到内部 gateway。
- URL：https://github.com/speakeasy-api/gram

### 6. chrisliu298/awesome-on-policy-distillation
- 仓库：chrisliu298/awesome-on-policy-distillation
- stars：437
- 更新时间：2026-06-30T17:21:16Z
- topics：awesome, awesome-list, distillation, gkd, knowledge-distillation, llm, llm-distillation, llm-training, minillm, on-policy-distillation, opd, post-training, reinforcement-learning, rl, rlhf, self-distillation, speculative-decoding
- 重要性：P0
- 主题标签：推理、训练与后训练、模型发布与模型能力、评测与基准
- 核心变化：本周期窗口内更新，README 已确认其是 On-Policy Distillation 主题 awesome list，并显示 Entries 391、stars/forks/last-commit 徽章；候选摘要说明收集 papers、technical reports、frameworks、tools。
- 一句话定位：LLM on-policy distillation / post-training 资源索引。
- 解决的问题：集中跟踪 OPD、RLHF、自蒸馏、speculative decoding 等与后训练和推理效率相关的论文/工具，降低研究和工程选型的信息搜集成本。
- 工程影响：对小模型蒸馏、teacher-student 训练、在线策略数据生成、推理加速路线调研有较强参考价值；可作为训练/评测路线规划的文献入口。
- 成熟度判断：awesome list 而非工具库，工程可执行性取决于具体条目；entries 多但质量分层、更新机制和去重准确性未确认。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；条目质量和覆盖完整性未逐项审计；无安装路径需要验证。
- 建议动作：今天应阅读。理由：OPD 与后训练是短期模型能力优化关键主题，应把该列表作为文献雷达入口。
- URL：https://github.com/chrisliu298/awesome-on-policy-distillation

### 7. msu-denver/bili-core
- 仓库：msu-denver/bili-core
- stars：14
- 更新时间：2026-06-30T19:04:24Z
- topics：adversarial-testing, agentic-ai, ai, benchmarking, c3-lab, langchain, langgraph, llm, msu-denver, multi-agent-systems, nsf, open-source, python, rag, red-teaming, research, security-testing
- 重要性：P1
- 主题标签：Agent 与多智能体、RAG 与知识工程、评测与基准
- 核心变化：本周期窗口内更新，README 已确认其为 BiliCore Open-Source LLM Framework，展示 CI/CD、latest release、Python 3.11+、MIT license；候选摘要指出包含 IRIS 单 Agent 编排、AETHER 声明式多 Agent、AEGIS 对抗安全测试。
- 一句话定位：学术实验室出品的 LLM 应用构建与安全测试框架。
- 解决的问题：把单 Agent、多 Agent、RAG/应用测试和 adversarial security testing 放在同一框架中，支持研究型 LLM app 的构建与验证。
- 工程影响：对多 Agent 编排 DSL、RAG app 测试、安全红队 benchmark、LangChain/LangGraph 集成有参考意义；可作为评测框架备选观察。
- 成熟度判断：stars 很低，偏研究/早期；但 README 有 CI、release、Python/License 信号，且 topic 覆盖 benchmark/RAG/security。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；IRIS/AETHER/AEGIS 模块能力来自候选摘要，未逐项运行；安装未实测。
- 建议动作：持续观察。理由：方向贴合评测和安全，但社区热度低，先跟踪 release 与示例质量。
- URL：https://github.com/msu-denver/bili-core

### 8. kochetkov-ma/claude-brewcode
- 仓库：kochetkov-ma/claude-brewcode
- stars：28
- 更新时间：2026-06-30T19:04:38Z
- topics：ai-agent, ai-tools, anthropic, claude-code, claude-code-agents, claude-code-plugin, claude-code-skill, developer-tools, llm-tools, marketplace, mcp, prompt-engineering
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具
- 核心变化：本周期窗口内更新，README 已确认其是 Claude Code plugin suite，包含 development、documentation、text utility、visual workflows 四类插件，并强调 25 skills、14 agents、9 lifecycle hooks 以及 context compaction 后的知识传递。
- 一句话定位：面向 Claude Code 的开发流程插件与上下文持久化套件。
- 解决的问题：缓解长任务中 context compaction 导致的状态丢失，并把开发、文档、评审、规则管理等动作封装为技能/agent/hook。
- 工程影响：对 agentic coding 的长任务交接、项目规则管理、自动 code review quorum、skill/agent 生成和知识持久化有参考价值。
- 成熟度判断：stars 低但 README 结构较完整，提供 release badge 和外部文档链接；生态绑定 Claude Code，通用性与安全边界需验证。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；hook 和 agent 数量来自 README/候选摘要，未运行；安装未实测。
- 建议动作：持续观察。理由：上下文持久化和 lifecycle hook 值得借鉴，但低热度项目先做结构阅读即可。
- URL：https://github.com/kochetkov-ma/claude-brewcode

### 9. GoogleCloudPlatform/db-context-enrichment
- 仓库：GoogleCloudPlatform/db-context-enrichment
- stars：32
- 更新时间：2026-06-30T18:24:41Z
- topics：未提供 topics
- 重要性：P1
- 主题标签：RAG 与知识工程、数据集与数据工程、评测与基准
- 核心变化：本周期窗口内更新，README 已确认该仓库从原 Go CLI 重组为 Python-based Context Engineering Agent / MCP Server，用于从数据库 schema 生成和维护结构化 ContextSet，提升自然语言到 SQL 的准确性。
- 一句话定位：面向数据库 NL2SQL 的上下文工程 Agent/MCP server。
- 解决的问题：把 schema、业务逻辑、术语、自然语言问题到 SQL 的模板映射沉淀成 ContextSet，减少 LLM 直连数据库时对结构和业务语义的误解。
- 工程影响：对数据库 RAG、text-to-SQL、上下文集合版本化、schema enrichment、MCP 化数据库工具和自动评估闭环有直接参考意义。
- 成熟度判断：GoogleCloudPlatform 组织来源强，但 README 明确“not officially supported Google product”；stars 低，仓库重组后新 Python/MCP 路线稳定性需观察。
- 证据边界：README 已确认；stars、更新时间来自候选 GitHub metadata；候选未提供 topics；数据库访问风险、评估指标和 MCP server 部署未实测。
- 建议动作：今天应阅读。理由：结构化数据库上下文工程是 RAG/NL2SQL 的高价值方向，且仓库重组信号值得跟进。
- URL：https://github.com/GoogleCloudPlatform/db-context-enrichment

### 10. lidge-jun/opencodex
- 仓库：lidge-jun/opencodex
- stars：207
- 更新时间：2026-06-30T19:04:29Z
- topics：ai-tools, anthropic, claude, codex, codex-cli, developer-tools, gemini, kiro, llm, openai, proxy, typescript
- 重要性：P1
- 主题标签：推理系统与工程工具、Agent 与多智能体
- 核心变化：本周期窗口内更新，README 已确认其主张“make codex open”，提供 `npm install -g @bitkyc08/opencodex`、`ocx start`、localhost:10100 的入口，用作 Codex CLI/App/SDK 的 universal provider proxy。
- 一句话定位：面向 OpenAI Codex 生态的多模型 provider proxy。
- 解决的问题：让 Codex CLI、App、SDK 通过代理接入 Anthropic、Gemini、Kiro 等非 OpenAI provider，降低单一模型供应商绑定。
- 工程影响：对 LLM gateway、provider adapter、开发者工具多模型路由、兼容 OpenAI/Codex 协议的代理层有参考价值；也提示需关注凭据管理和协议兼容风险。
- 成熟度判断：stars 中等，README 有 npm 安装入口和 node 版本徽章；候选 reason_codes 标注 actionability_needs_validation，说明真实可用性/兼容矩阵还需验证。
- 证据边界：README 已确认；stars、topics、更新时间来自候选 GitHub metadata；支持 provider 范围来自 README/候选摘要，未实测；安全与协议兼容未确认。
- 建议动作：今天应实验。理由：provider proxy 若可用会直接影响 Codex/Agent 工具链的模型路由策略，应小范围验证兼容性与凭据安全。
- URL：https://github.com/lidge-jun/opencodex
