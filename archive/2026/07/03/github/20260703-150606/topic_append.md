## 2026-07-03 15:06 GitHub 项目主题条目

### Agent 与多智能体

- hanyeol/model-compose（P0）：适用场景：可作为 Agent 编排和 LLMOps 配置层候选，适合评估是否能替代零散脚本，把 RAG、工具服务和模型端点纳入同一部署描述。；成熟度：stars 75，仓库仍偏早期；但 topics 覆盖 MCP/RAG/LLMOps，定位明确。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/hanyeol/model-compose
- trpc-group/trpc-agent-go（P0）：适用场景：对 Go 技术栈的 Agent 服务很有参考价值，尤其是 graph workflow、OpenTelemetry、MCP/A2A 接入与 evaluation 组合方式。；成熟度：stars 1493，信号强；但具体 API 稳定性、示例覆盖和生产案例仍需进一步核验。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/trpc-group/trpc-agent-go
- automagik-dev/genie（P0）：适用场景：对开发工作流自动化和多 Agent coding pipeline 有直接参考价值，可对比现有 Claude Code/Codex/worktree 编排方案。；成熟度：stars 322，中早期；依赖外部 coding agent 与 MCP，安装、权限隔离和失败恢复需实测。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/automagik-dev/genie
- nicobailon/pi-mcp-adapter（P0）：适用场景：若其 adapter 设计有效，可为 MCP 工具网关压缩上下文和 coding agent 集成方式提供参考。；成熟度：stars 955，关注度较高；但摘要信息较窄，支持的 Pi 版本、压缩策略和通用性需 README/代码确认。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/nicobailon/pi-mcp-adapter
- 1jehuang/jcode（P0）：适用场景：高 stars 表明生态关注度强，适合对比 TUI coding harness 的交互、工具权限、MCP 接入和本地执行模型。；成熟度：stars 8105，热度很强；但“harness”范围、插件模型、企业可控性和安全边界需进一步确认。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/1jehuang/jcode
- ZHangZHengEric/Sage（P0）：适用场景：可用于观察 Manus 类多 Agent workflow 的开源实现方式，对任务分解、状态管理和协同接口有参考意义。；成熟度：stars 1207，热度不错；但 topics 拼写和摘要较粗，API 完整度、评测和生产可观测性需确认。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/ZHangZHengEric/Sage
- ondata/ckan-mcp-server（P0）：适用场景：对数据发现、公共数据 RAG、政府/科研数据 Agent 很实用，可作为垂直 MCP server 模板。；成熟度：stars 56，较早期；Cloudflare Workers/Node 形态值得看，但认证、分页、SQL 限制和多 CKAN 兼容性需实测。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/ondata/ckan-mcp-server
- shenyangs/Guanlan（P1）：适用场景：对中文 RAG/研究 Agent 有特定价值，可补充英文 web reader 不擅长的中文信源发现与路由。；成熟度：stars 47，早期且 engagement 偏弱；需要确认支持的搜索源、反爬策略、引用格式和 MCP 暴露能力。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/shenyangs/Guanlan
- wuisabel-gif/MemWhale（P1）：适用场景：可能补强 coding agent 的长期记忆、调试复盘和本地可检索日志，为 MCP memory/terminal recorder 提供实现参考。；成熟度：stars 43，早期且 engagement 偏弱；本地隐私、日志体量、索引质量、跨机器同步仍需验证。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/wuisabel-gif/MemWhale

### RAG 与知识工程

- hanyeol/model-compose（P0）：适用场景：可作为 Agent 编排和 LLMOps 配置层候选，适合评估是否能替代零散脚本，把 RAG、工具服务和模型端点纳入同一部署描述。；成熟度：stars 75，仓库仍偏早期；但 topics 覆盖 MCP/RAG/LLMOps，定位明确。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/hanyeol/model-compose
- trpc-group/trpc-agent-go（P0）：适用场景：对 Go 技术栈的 Agent 服务很有参考价值，尤其是 graph workflow、OpenTelemetry、MCP/A2A 接入与 evaluation 组合方式。；成熟度：stars 1493，信号强；但具体 API 稳定性、示例覆盖和生产案例仍需进一步核验。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/trpc-group/trpc-agent-go
- ondata/ckan-mcp-server（P0）：适用场景：对数据发现、公共数据 RAG、政府/科研数据 Agent 很实用，可作为垂直 MCP server 模板。；成熟度：stars 56，较早期；Cloudflare Workers/Node 形态值得看，但认证、分页、SQL 限制和多 CKAN 兼容性需实测。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/ondata/ckan-mcp-server
- shenyangs/Guanlan（P1）：适用场景：对中文 RAG/研究 Agent 有特定价值，可补充英文 web reader 不擅长的中文信源发现与路由。；成熟度：stars 47，早期且 engagement 偏弱；需要确认支持的搜索源、反爬策略、引用格式和 MCP 暴露能力。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/shenyangs/Guanlan

### 推理系统与工程工具

- hanyeol/model-compose（P0）：适用场景：可作为 Agent 编排和 LLMOps 配置层候选，适合评估是否能替代零散脚本，把 RAG、工具服务和模型端点纳入同一部署描述。；成熟度：stars 75，仓库仍偏早期；但 topics 覆盖 MCP/RAG/LLMOps，定位明确。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/hanyeol/model-compose
- automagik-dev/genie（P0）：适用场景：对开发工作流自动化和多 Agent coding pipeline 有直接参考价值，可对比现有 Claude Code/Codex/worktree 编排方案。；成熟度：stars 322，中早期；依赖外部 coding agent 与 MCP，安装、权限隔离和失败恢复需实测。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/automagik-dev/genie
- nicobailon/pi-mcp-adapter（P0）：适用场景：若其 adapter 设计有效，可为 MCP 工具网关压缩上下文和 coding agent 集成方式提供参考。；成熟度：stars 955，关注度较高；但摘要信息较窄，支持的 Pi 版本、压缩策略和通用性需 README/代码确认。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/nicobailon/pi-mcp-adapter
- 1jehuang/jcode（P0）：适用场景：高 stars 表明生态关注度强，适合对比 TUI coding harness 的交互、工具权限、MCP 接入和本地执行模型。；成熟度：stars 8105，热度很强；但“harness”范围、插件模型、企业可控性和安全边界需进一步确认。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/1jehuang/jcode
- linearis-oss/linearis（P0）：适用场景：可作为 LLM agent 接企业 SaaS 的“结构化 CLI facade”范式参考，尤其适合任务/Issue 编排链路。；成熟度：stars 224，定位清晰但垂直；仅适用于 Linear 场景，通用 Agent 框架价值有限。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/linearis-oss/linearis
- wuisabel-gif/MemWhale（P1）：适用场景：可能补强 coding agent 的长期记忆、调试复盘和本地可检索日志，为 MCP memory/terminal recorder 提供实现参考。；成熟度：stars 43，早期且 engagement 偏弱；本地隐私、日志体量、索引质量、跨机器同步仍需验证。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/wuisabel-gif/MemWhale

### 评测与基准

- trpc-group/trpc-agent-go（P0）：适用场景：对 Go 技术栈的 Agent 服务很有参考价值，尤其是 graph workflow、OpenTelemetry、MCP/A2A 接入与 evaluation 组合方式。；成熟度：stars 1493，信号强；但具体 API 稳定性、示例覆盖和生产案例仍需进一步核验。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/trpc-group/trpc-agent-go

### 产品与商业化

- linearis-oss/linearis（P0）：适用场景：可作为 LLM agent 接企业 SaaS 的“结构化 CLI facade”范式参考，尤其适合任务/Issue 编排链路。；成熟度：stars 224，定位清晰但垂直；仅适用于 Linear 场景，通用 Agent 框架价值有限。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/linearis-oss/linearis

### 数据集与数据工程

- ondata/ckan-mcp-server（P0）：适用场景：对数据发现、公共数据 RAG、政府/科研数据 Agent 很实用，可作为垂直 MCP server 模板。；成熟度：stars 56，较早期；Cloudflare Workers/Node 形态值得看，但认证、分页、SQL 限制和多 CKAN 兼容性需实测。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/ondata/ckan-mcp-server
- wuisabel-gif/MemWhale（P1）：适用场景：可能补强 coding agent 的长期记忆、调试复盘和本地可检索日志，为 MCP memory/terminal recorder 提供实现参考。；成熟度：stars 43，早期且 engagement 偏弱；本地隐私、日志体量、索引质量、跨机器同步仍需验证。；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/wuisabel-gif/MemWhale
