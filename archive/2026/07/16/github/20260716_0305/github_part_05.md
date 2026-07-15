### 4. hoophq/hoop

- 仓库：hoophq/hoop
- stars：760
- 更新时间：2026-07-15T19:02:56Z（GitHub Search 候选）；GitHub API 复核为 2026-07-15T19:02:50Z
- topics：agent, databases, grpc, llm, mcp, proxy, security
- 重要性：P0
- 主题标签：推理系统与工程工具；Agent 与多智能体
- 核心变化：README 已确认 hoop 是位于工程师、AI Agents、MCP Clients 与数据库/Kubernetes/API 之间的 L7 gateway，强调敏感数据掩码、危险命令拦截、风险写操作人工审批、会话记录；顶部标注 “Agent in the loop”。
- 一句话定位：面向人和 AI Agent 访问基础设施的统一安全网关。
- 解决的问题：LLM/MCP 工具一旦直连生产数据库、容器或 API，缺少统一审计、脱敏、审批和命令阻断；hoop 把控制面放到协议网关层。
- 工程影响：对 LLM gateway/MCP 安全治理有直接参考价值，可用于设计 Agent 工具调用的 wire-level policy、敏感数据出站控制和高风险操作审批链路。
- 成熟度判断：760 stars，Go，MIT；README 已确认 Docker/release/docs 链路和生产使用主张；但“under 5ms”延迟、各协议覆盖和企业部署复杂度未在本轮复测。
- 证据边界：README 已确认；stars、topics、更新时间来自候选和 GitHub API；未部署网关，未验证策略表达能力、MCP 兼容和审计数据结构。
- 建议动作：今天应阅读。理由：它正好切中 Agent 工具访问生产系统的安全边界，应优先读架构和 policy 模型；是否实验取决于是否有可控测试后端。
- URL：https://github.com/hoophq/hoop
