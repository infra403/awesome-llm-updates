## 2026-07-03 15:06 北京时间 | GitHub 项目巡检

筛选口径：仅纳入本次 8 小时巡检窗口内确认有更新时间、来源链接和工程相关 reason_codes 的 P0/P1 候选；不为凑数纳入证据不足或 actionability weak 的条目。

### 1. hanyeol/model-compose
- 仓库：hanyeol/model-compose
- stars：75
- 更新时间：2026-07-03T06:53:06Z
- topics：agent-framework, ai-agents, ai-infrastructure, ai-workflow, anthropic, declarative, huggingface, langchain-alternative, llm, llm-framework, llm-orchestration, llmops, mcp, mcp-server, model-context-protocol, openai, rag, vector-database, workflow-orchestration, yaml
- 重要性：P0
- 主题标签：Agent 与多智能体；RAG 与知识工程；推理系统与工程工具
- 核心变化：本周期内仓库更新，候选信号显示其围绕 用类似 docker-compose 的 YAML 把 agent、RAG pipeline 与 MCP server 组合成可移植运行时。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：用类似 docker-compose 的 YAML 把 agent、RAG pipeline 与 MCP server 组合成可移植运行时。
- 解决的问题：Agent/RAG/MCP 组件在不同机器和环境中组合、启动、迁移成本高，缺少统一声明式入口。
- 工程影响：可作为 Agent 编排和 LLMOps 配置层候选，适合评估是否能替代零散脚本，把 RAG、工具服务和模型端点纳入同一部署描述。
- 成熟度判断：stars 75，仓库仍偏早期；但 topics 覆盖 MCP/RAG/LLMOps，定位明确。
- 证据边界：README 已确认（README.md，约 12956 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：今天应阅读：若配置模型足够简单，可能直接影响内部 Agent runtime 的 YAML 规范设计。
- URL：https://github.com/hanyeol/model-compose

### 2. trpc-group/trpc-agent-go
- 仓库：trpc-group/trpc-agent-go
- stars：1493
- 更新时间：2026-07-03T06:54:10Z
- topics：a2a, a2a-protocol, ag-ui, agent, agent-framework, ai, ai-agents, evaluation, go, golang, graph-workflows, llm, mcp, model-context-protocol, multi-agent, observability, opentelemetry, rag
- 重要性：P0
- 主题标签：Agent 与多智能体；评测与基准；RAG 与知识工程
- 核心变化：本周期内仓库更新，候选信号显示其围绕 面向生产 Agent 系统的 Go 框架，覆盖图工作流、工具、记忆、A2A、MCP、评测与可观测性。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：面向生产 Agent 系统的 Go 框架，覆盖图工作流、工具、记忆、A2A、MCP、评测与可观测性。
- 解决的问题：生产 Agent 不只是 prompt 调用，还需要工作流、工具协议、评估、遥测和多 Agent 通信的工程闭环。
- 工程影响：对 Go 技术栈的 Agent 服务很有参考价值，尤其是 graph workflow、OpenTelemetry、MCP/A2A 接入与 evaluation 组合方式。
- 成熟度判断：stars 1493，信号强；但具体 API 稳定性、示例覆盖和生产案例仍需进一步核验。
- 证据边界：README 已确认（README.md，约 29281 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：今天应实验：优先跑通最小 graph workflow + MCP tool + eval 示例，判断能否进入服务端 Agent 框架候选。
- URL：https://github.com/trpc-group/trpc-agent-go

### 3. automagik-dev/genie
- 仓库：automagik-dev/genie
- stars：322
- 更新时间：2026-07-03T07:03:01Z
- topics：ai-agents, ai-developer-tools, anthropic, automation, autonomous-agents, claude, claude-code, cli, coding-agents, context-engineering, developer-tools, llm, mcp, orchestration, parallel-agents, productivity, terminal, typescript, vibe-coding, worktrees
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：本周期内仓库更新，候选信号显示其围绕 “wishes in, PRs out”的 CLI coding agent，强调访谈需求、规划、隔离 worktree 并行派发 agent、提交前 review。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：“wishes in, PRs out”的 CLI coding agent，强调访谈需求、规划、隔离 worktree 并行派发 agent、提交前 review。
- 解决的问题：代码 Agent 落地时常缺少需求澄清、并行隔离、统一 review 和 PR 产物管理。
- 工程影响：对开发工作流自动化和多 Agent coding pipeline 有直接参考价值，可对比现有 Claude Code/Codex/worktree 编排方案。
- 成熟度判断：stars 322，中早期；依赖外部 coding agent 与 MCP，安装、权限隔离和失败恢复需实测。
- 证据边界：README 已确认（README.md，约 9068 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：今天应实验：若能在沙箱仓库中稳定生成 PR，可作为 coding-agent 编排层备选。
- URL：https://github.com/automagik-dev/genie

### 4. nicobailon/pi-mcp-adapter
- 仓库：nicobailon/pi-mcp-adapter
- stars：955
- 更新时间：2026-07-03T07:04:44Z
- topics：ai, claude, coding-agent, extension, llm, mcp, model-context-protocol, pi
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：本周期内仓库更新，候选信号显示其围绕 面向 Pi coding agent 的 token-efficient MCP adapter。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：面向 Pi coding agent 的 token-efficient MCP adapter。
- 解决的问题：Coding agent 接 MCP 工具时，工具描述、上下文和调用桥接可能带来 token 开销和协议适配成本。
- 工程影响：若其 adapter 设计有效，可为 MCP 工具网关压缩上下文和 coding agent 集成方式提供参考。
- 成熟度判断：stars 955，关注度较高；但摘要信息较窄，支持的 Pi 版本、压缩策略和通用性需 README/代码确认。
- 证据边界：README 已确认（README.md，约 21795 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：今天应阅读：重点看 token-efficient 的具体机制，判断是否可复用到 MCP gateway。
- URL：https://github.com/nicobailon/pi-mcp-adapter

### 5. 1jehuang/jcode
- 仓库：1jehuang/jcode
- stars：8105
- 更新时间：2026-07-03T07:03:42Z
- topics：ai, claude, cli, coding-agent, llm, mcp, openai, rust, terminal, tui
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：本周期内仓库更新，候选信号显示其围绕 Rust/TUI 形态的 Coding Agent Harness，支持 Claude/OpenAI/MCP/terminal。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：Rust/TUI 形态的 Coding Agent Harness，支持 Claude/OpenAI/MCP/terminal。
- 解决的问题：开发者需要统一的终端 coding-agent 宿主，整合模型、工具协议与交互界面。
- 工程影响：高 stars 表明生态关注度强，适合对比 TUI coding harness 的交互、工具权限、MCP 接入和本地执行模型。
- 成熟度判断：stars 8105，热度很强；但“harness”范围、插件模型、企业可控性和安全边界需进一步确认。
- 证据边界：README 已确认（README.md，约 37886 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：今天应阅读：优先梳理架构和安全模型，再决定是否 POC。
- URL：https://github.com/1jehuang/jcode

### 6. linearis-oss/linearis
- 仓库：linearis-oss/linearis
- stars：224
- 更新时间：2026-07-03T07:05:36Z
- topics：agent, cli, command-line-tool, linear, linearapp, llm
- 重要性：P0
- 主题标签：产品与商业化；推理系统与工程工具
- 核心变化：本周期内仓库更新，候选信号显示其围绕 面向 Linear.app 的 CLI，提供 JSON 输出、智能 ID 解析和优化 GraphQL 查询，明确服务 LLM agents 与人类。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：面向 Linear.app 的 CLI，提供 JSON 输出、智能 ID 解析和优化 GraphQL 查询，明确服务 LLM agents 与人类。
- 解决的问题：Agent 操作项目管理系统时需要稳定、结构化、可脚本化的接口，而不是脆弱网页自动化。
- 工程影响：可作为 LLM agent 接企业 SaaS 的“结构化 CLI facade”范式参考，尤其适合任务/Issue 编排链路。
- 成熟度判断：stars 224，定位清晰但垂直；仅适用于 Linear 场景，通用 Agent 框架价值有限。
- 证据边界：README 已确认（README.md，约 7721 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：持续观察：如果团队使用 Linear，可今天试用；否则作为 SaaS CLI 设计样式参考。
- URL：https://github.com/linearis-oss/linearis

### 7. ZHangZHengEric/Sage
- 仓库：ZHangZHengEric/Sage
- stars：1207
- 更新时间：2026-07-03T07:04:23Z
- topics：agents, ai, llm, manus, muilt-agents, workflow
- 重要性：P0
- 主题标签：Agent 与多智能体
- 核心变化：本周期内仓库更新，候选信号显示其围绕 面向复杂任务的 Multi-Agent System Framework。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：面向复杂任务的 Multi-Agent System Framework。
- 解决的问题：复杂任务需要多角色、多步骤 workflow 分解与协同，而单 Agent 容易上下文混乱或执行不可控。
- 工程影响：可用于观察 Manus 类多 Agent workflow 的开源实现方式，对任务分解、状态管理和协同接口有参考意义。
- 成熟度判断：stars 1207，热度不错；但 topics 拼写和摘要较粗，API 完整度、评测和生产可观测性需确认。
- 证据边界：README 已确认（README.md，约 11915 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：持续观察：先阅读架构与示例，不急于纳入生产 POC。
- URL：https://github.com/ZHangZHengEric/Sage

### 8. ondata/ckan-mcp-server
- 仓库：ondata/ckan-mcp-server
- stars：56
- 更新时间：2026-07-03T07:04:55Z
- topics：ai-tools, api-client, civic-tech, ckan, ckan-api, claude, cloudflare-workers, data-discovery, data-portal, datastore, government-data, mcp, model-context-protocol, nodejs, open-data, public-data, solr, typescript
- 重要性：P0
- 主题标签：数据集与数据工程；RAG 与知识工程；Agent 与多智能体
- 核心变化：本周期内仓库更新，候选信号显示其围绕 用于查询 CKAN 开放数据门户的 MCP server，覆盖 package search、DataStore SQL、组织、分组和标签。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：用于查询 CKAN 开放数据门户的 MCP server，覆盖 package search、DataStore SQL、组织、分组和标签。
- 解决的问题：开放数据门户常通过 CKAN 暴露，但 Agent/RAG 系统缺少标准工具接口来搜索、取数和执行 DataStore 查询。
- 工程影响：对数据发现、公共数据 RAG、政府/科研数据 Agent 很实用，可作为垂直 MCP server 模板。
- 成熟度判断：stars 56，较早期；Cloudflare Workers/Node 形态值得看，但认证、分页、SQL 限制和多 CKAN 兼容性需实测。
- 证据边界：README 已确认（README.md，约 34924 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：今天应实验：用公开 CKAN 实例跑 package search/DataStore SQL，验证数据工程可用性。
- URL：https://github.com/ondata/ckan-mcp-server

### 9. shenyangs/Guanlan
- 仓库：shenyangs/Guanlan
- stars：47
- 更新时间：2026-07-03T07:03:02Z
- topics：ai-agent, chinese-web, cli, llm-tools, mcp, python, research-tool, search, source-routing, web-reader
- 重要性：P1
- 主题标签：RAG 与知识工程；Agent 与多智能体
- 核心变化：本周期内仓库更新，候选信号显示其围绕 观澜：面向 AI Agent 的中文互联网研究、阅读与信源路由工具。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：观澜：面向 AI Agent 的中文互联网研究、阅读与信源路由工具。
- 解决的问题：中文互联网信息源分散，Agent 做研究时需要搜索、阅读、信源路由和可信来源选择。
- 工程影响：对中文 RAG/研究 Agent 有特定价值，可补充英文 web reader 不擅长的中文信源发现与路由。
- 成熟度判断：stars 47，早期且 engagement 偏弱；需要确认支持的搜索源、反爬策略、引用格式和 MCP 暴露能力。
- 证据边界：README 已确认（README.md，约 5816 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：持续观察：适合作为中文研究 Agent 工具储备，先看 README 和示例。
- URL：https://github.com/shenyangs/Guanlan

### 10. wuisabel-gif/MemWhale
- 仓库：wuisabel-gif/MemWhale
- stars：43
- 更新时间：2026-07-03T07:04:45Z
- topics：ai-agents, cli, command-line, debugging, developer-tools, jetson, knowledge-graph, local-first, mcp, memory, model-context-protocol, react, robotics, rust, second-brain, sqlite, tauri, terminal, terminal-recorder, typescript
- 重要性：P1
- 主题标签：Agent 与多智能体；数据集与数据工程；推理系统与工程工具
- 核心变化：本周期内仓库更新，候选信号显示其围绕 Rust/Tauri local-first 终端记忆系统，把命令、参数、日志、会话、错误、书签和调试历史写入 SQLite。 这一方向继续活跃；工程价值来自其把问题聚焦到可落地的 Agent/RAG/MCP/开发工具链组件，而非单纯论文或列表。
- 一句话定位：Rust/Tauri local-first 终端记忆系统，把命令、参数、日志、会话、错误、书签和调试历史写入 SQLite。
- 解决的问题：开发者和 Agent 在跨机器、SSH、容器和崩溃场景下容易丢失终端上下文与调试历史。
- 工程影响：可能补强 coding agent 的长期记忆、调试复盘和本地可检索日志，为 MCP memory/terminal recorder 提供实现参考。
- 成熟度判断：stars 43，早期且 engagement 偏弱；本地隐私、日志体量、索引质量、跨机器同步仍需验证。
- 证据边界：README 已确认（README.md，约 8937 字符）；未做完整安装与端到端压测；本条不推断 README 之外能力。
- 建议动作：持续观察：适合调研本地 terminal memory 设计，暂不优先接入生产。
- URL：https://github.com/wuisabel-gif/MemWhale
