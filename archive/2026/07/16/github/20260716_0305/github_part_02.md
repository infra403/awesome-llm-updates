### 1. mlhher/late-cli

- 仓库：mlhher/late-cli
- stars：379
- 更新时间：2026-07-15T19:02:08Z（GitHub Search 候选）；GitHub API 复核为 2026-07-15T18:59:00Z，仍在本轮窗口内
- topics：agent, ai-agent, ai-agents, ai-coding-agent, ai-coding-assistant, ai-skills, autonomous-agents, claude, coding-agent, coding-agents, deepseek, gemini, harness, llm, llm-orchestration, local-ai, local-llm, mcp, qwen, tui
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：项目把“主编排器 + 临时子 Agent”作为核心工作流，声称通过隔离编辑、重试和实现细节来减少主上下文污染；README 已确认提供 Homebrew、安装脚本、静态二进制、本地 llama-server 默认支持和 OpenAI-compatible API 适配。
- 一句话定位：面向本地/云模型的零配置 AI coding agent，重点押注 ephemeral subagents 和低上下文噪声。
- 解决的问题：长任务编码 Agent 容易把执行细节塞满上下文，导致规划能力下降；late-cli 尝试用一次性子 Agent 把执行噪声隔离在子上下文中。
- 工程影响：值得对照 Claude Code/OpenCode 类工具评估“子 Agent 隔离 + 短系统提示 + 本地小模型”的编码吞吐模式，可能影响 Agent 编排、上下文预算管理、MCP/Skills 接入和本地模型工作流设计。
- 成熟度判断：379 stars，Go 项目；README 已确认安装路径和模型接入说明，但许可证在 GitHub API 中为 NOASSERTION，生产合规需再查 LICENSE；性能和 token 节省为 README/社区引用主张，尚未本地复测。
- 证据边界：README 已确认；stars、topics、更新时间来自候选和 GitHub API；未运行二进制，未验证真实 benchmark、MCP 兼容面和安全隔离边界。
- 建议动作：今天应实验。理由：P0 且直接对应 coding agent 编排和上下文控制，适合用一个中等复杂代码修复任务与现有 Agent CLI 做小样本对比。
- URL：https://github.com/mlhher/late-cli
