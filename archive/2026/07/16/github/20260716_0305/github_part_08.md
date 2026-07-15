### 7. Fmarzochi/EGC

- 仓库：Fmarzochi/EGC
- stars：32
- 更新时间：2026-07-15T19:01:39Z（GitHub Search 候选）；GitHub API 复核为 2026-07-15T19:01:49Z
- topics：ai-agents, aider, amazonq, claude-code, cli, codex, cohere, cursor, gemini-cli, goose, groq, kiro, mcp, open-source, openhands, persistent-memory, skills, trae, vertex-ai, warp
- 重要性：P1
- 主题标签：Agent 与多智能体；RAG 与知识工程
- 核心变化：README 已确认 EGC 是 local runtime，为多种 AI coding 工具提供跨会话持久记忆，安装命令为 `npm install -g @egchq/egc && egc install`，强调自动保存/加载项目状态、偏好、失败经验和下一步任务，并附带命令守护能力。
- 一句话定位：跨 Agent/IDE 的本地持久记忆和 MCP runtime。
- 解决的问题：不同 coding agent 与 IDE 会话割裂，每次重启都需要人工复述项目状态；EGC 试图把记忆层从单一 Agent 中抽离出来。
- 工程影响：可启发 Agent 记忆架构：项目级状态文件、跨工具上下文协议、自动恢复和命令安全守护；也可能与现有 Hermes skills/memory 形成对比。
- 成熟度判断：32 stars，JavaScript，MIT；README 已确认 npm 安装和多工具支持声明；但自动记忆质量、隐私边界、状态冲突处理和 MCP runtime 细节未确认。
- 证据边界：README 已确认；stars、topics、更新时间来自候选和 GitHub API；未安装，未验证对 Claude Code/Codex/Cursor 等工具的真实接入效果。
- 建议动作：今天应阅读。理由：跨工具持久记忆是 Agent 工程关键主题，虽早期但值得读其状态模型和安全守护设计。
- URL：https://github.com/Fmarzochi/EGC
