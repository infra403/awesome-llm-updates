### 3. wellwelwel/lagune

- 仓库：wellwelwel/lagune
- stars：71
- 更新时间：2026-07-15T19:04:40Z（GitHub Search 候选）；GitHub API 复核为 2026-07-15T19:03:41Z
- topics：agent-skills, ai, ai-agents, ai-driven, blue-team, claude-code, codex, copilot, cursor-ai, llm, prd, prompt-engineering, prompt-toolkit, sdd, sdh, security, security-driven-hardening, skills, spec-driven, spec-kit
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：README 已确认 Lagune 面向“让 AI agent 帮项目做安全加固”，通过本地 dashboard/CLI 指导安全工作，声称支持 72 个 agents、无需 API key、可与 Claude/Codex 等现有 Agent 协作。
- 一句话定位：面向 AI coding agent 的本地安全加固与 blue-team 辅助层。
- 解决的问题：AI 编码流程通常先追求功能完成，安全建模、风险检查和加固任务容易滞后；Lagune 将安全需求拆进 Agent 工作流。
- 工程影响：可作为 Agent 开发流水线的安全检查/加固提示层，影响代码生成前后的威胁建模、spec-driven security、审计任务分解和人机协同检查。
- 成熟度判断：71 stars，TypeScript，MIT；README 已确认 `npx -y lagune@latest` 本地 dashboard 入口和无 API key 模式；但“72 agents 支持”的覆盖质量、是否有静态/动态分析能力、输出可验证性未确认。
- 证据边界：README 已确认；stars、topics、更新时间来自候选和 GitHub API；未运行 dashboard，未验证安全建议的深度、误报率和 CI 集成方式。
- 建议动作：今天应阅读。理由：安全 Agent 工作流方向重要，但星标和证据仍早期，先读 docs/支持 Agent 列表，再决定是否 POC。
- URL：https://github.com/wellwelwel/lagune
