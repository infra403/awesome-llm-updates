## 2026-07-10 09:07 GitHub 项目主题条目

### Agent 与多智能体

- xinhuangcs/agentmaker（P1）：适用场景：对照现有 Agent runtime 的工具调用、记忆、RAG、HITL、guardrails、observability、Trace Detective 和测试替身能力。成熟度：偏早期，README 有 CI/PyPI/docs/pip install 与完整 quickstart，但 stars 仅 22，社区验证弱。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/xinhuangcs/agentmaker
- agentscope-ai/agentscope-java（P1）：适用场景：JVM 后端接入 ReAct、tool calling、memory、多 Agent、MCP/A2A、sandbox 与 OpenTelemetry，而不是把 Agent 逻辑全部迁到 Python。成熟度：中等偏高，4k+ stars，README 有 JDK 17+、Maven Central、版本 1.0.12 与生产级特性；API 稳定性和生产案例未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/agentscope-ai/agentscope-java

### RAG 与知识工程

- codexu/note-gen（P0）：适用场景：个人/团队 Markdown 知识库、AI 笔记、知识库问答、向量/混合检索和 MCP 上下文入口。成熟度：偏高，12k+ stars，README 有下载入口、多端状态、同步方式和知识库能力；企业权限、索引质量和 MCP 细节需 POC。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/codexu/note-gen
- n24q02m/better-notion-mcp（P1）：适用场景：把 Notion 页面、数据库、blocks、comments 作为 Agent/RAG 知识源，通过 Markdown-first MCP 降低上下文拼装成本。成熟度：中低，README 有 CI、codecov、npm、Docker、Node.js >= 24、stdio/OAuth 双传输；复杂数据库和权限保真需实验。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/n24q02m/better-notion-mcp

### 产品与商业化

- dkships/pm-copilot（P1）：适用场景：把客服工单、功能请求、业务指标通过 MCP 接入 Agent，辅助需求优先级、产品计划和证据回溯。成熟度：偏早期，README 有真实数据规模样例、PII scrubbing、Claude Desktop/Code 配置和 npm build；评分方法泛化性、权限隔离和多系统适配未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g 原文：https://github.com/dkships/pm-copilot
