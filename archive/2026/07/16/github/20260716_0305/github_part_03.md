### 2. bartolli/codanna

- 仓库：bartolli/codanna
- stars：706
- 更新时间：2026-07-15T19:00:37Z（GitHub Search 候选）；GitHub API 复核为 2026-07-15T19:05:56Z
- topics：ai-agents, call-graph-analysis, code-indexing, code-intelligence, code-search, coding-agents, developer-tools-ai-agent, local-first, mcp, mcp-server, mcp-tools, rag, rust-cli, semantic-code-search, static-analysis, symbol-search
- 重要性：P0
- 主题标签：RAG 与知识工程；Agent 与多智能体；推理系统与工程工具
- 核心变化：README 已确认其定位是给代码助手提供“X-ray vision”：函数/符号理解、关系追踪、实现定位，并通过 MCP server/CLI 为 Agent 提供本地代码智能；提供 curl/Homebrew/Nix/PowerShell 安装和 `codanna init/index` 工作流。
- 一句话定位：本地优先的代码索引、语义搜索和调用图 MCP 服务器。
- 解决的问题：Coding Agent 在大型代码库中常陷入 grep/读文件循环，缺少符号级、调用图级上下文检索；codanna 把代码库做成本地可查询知识层。
- 工程影响：可作为 Agentic coding 的代码 RAG 基础设施，补齐“符号搜索 + 静态分析 + MCP 工具调用”的上下文检索层，尤其适合接入多 Agent 编码系统中的代码导航工具箱。
- 成熟度判断：706 stars，Rust 项目，Apache-2.0；README 已确认多平台安装、文档和索引命令；但具体语言覆盖、索引增量更新性能、大仓库规模上限需实测。
- 证据边界：README 已确认；stars、topics、更新时间来自候选和 GitHub API；未验证其 MCP schema、索引准确率、调用图质量和与现有 Agent 的延迟开销。
- 建议动作：今天应实验。理由：它直接提升 coding agent 的检索/定位能力，且安装链路明确，适合立即选一个真实仓库做索引和 MCP 调用测试。
- URL：https://github.com/bartolli/codanna
