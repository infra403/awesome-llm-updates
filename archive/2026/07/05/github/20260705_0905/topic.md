## 2026-07-05 09:05 GitHub 项目主题条目

### Agent 与多智能体

- `Justin0504/Aegis`（P0）：适用场景：Agent 运行时策略执行、安全审计、人工审批与 kill switch；成熟度：362 stars，接入方式、策略表达能力、支持的 agent runtime 和部署形态未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/Justin0504/Aegis
- `aofp/yume`（P0）：适用场景：Claude Code/子代理桌面编排、后台 agents、多 provider coding agent UI；成熟度：142 stars，功能完整度、跨平台安装包和安全沙箱策略未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/aofp/yume
- `rikkahub/rikkahub`（P0）：适用场景：移动端 LLM provider 聚合、聊天 UI、MCP/agent 端侧交互参考；成熟度：5838 stars，MCP 能力深度、provider 配置模型、隐私/本地存储策略未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/rikkahub/rikkahub
- `gptme/gptme-rag`（P1）：适用场景：Agent tools 的本地 RAG 检索插件、离线知识工程 CLI；成熟度：48 stars，索引后端、chunk 策略、增量更新、eval 指标和安装方式未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/gptme/gptme-rag
- `cesp99/spettro`（P1）：适用场景：终端 coding agent、多 agent workflow、TUI 状态管理和 provider 抽象参考；成熟度：25 stars，模型 provider、沙箱/权限控制、测试执行安全策略未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/cesp99/spettro
- `fractalmind-ai/fractalbot`（P1）：适用场景：多渠道消息到外部 agents 的 CLI/HTTP gateway、Slack/Telegram bot 路由；成熟度：15 stars，协议模型、鉴权、重试、队列和生产部署方式未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/fractalmind-ai/fractalbot

### RAG 与知识工程

- `Sandermage/sndr_core_engine`（P0）：适用场景：自托管推理栈中的长上下文、本地 RAG/pgvector、tool-calling 与 vLLM 优化组合参考；成熟度：119 stars，生产成熟度、安装路径、benchmark 复现实验未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/Sandermage/sndr_core_engine
- `gptme/gptme-rag`（P1）：适用场景：轻量本地 RAG CLI、standalone 检索或 gptme agent tool；成熟度：48 stars，索引后端、chunk 策略、增量更新、eval 指标和安装方式未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/gptme/gptme-rag

### 推理系统与工程工具

- `Sandermage/sndr_core_engine`（P0）：适用场景：消费级 NVIDIA 多卡上的 Qwen/Gemma vLLM patch-overlay、KV cache 量化、speculative decoding、cudagraph 与长上下文部署；成熟度：119 stars，安装路径、上游 vLLM 兼容性和 benchmark 复现未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/Sandermage/sndr_core_engine
- `cesp99/spettro`（P1）：适用场景：开发者终端内的模型选择、planning/coding/testing 自动化与多 agent workflow；成熟度：25 stars，模型 provider 列表、权限控制和实际自动化能力未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/cesp99/spettro

### 评测与基准

- `Justin0504/Aegis`（P0）：适用场景：Agent 行为审计、安全策略执行、审批流和 kill switch 的安全评估基线；成熟度：362 stars，审计日志格式、策略覆盖面和运行时支持范围未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/Justin0504/Aegis

### 产品与商业化

- `aofp/yume`（P0）：适用场景：coding-agent 桌面端产品、Claude Code 编排 UI、后台 agents 可视化；成熟度：142 stars，插件生态、跨平台安装和安全沙箱未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/aofp/yume
- `rikkahub/rikkahub`（P0）：适用场景：Android LLM 客户端、多 provider 聚合、移动端 MCP/agent 入口；成熟度：5838 stars，MCP 能力深度、provider 配置模型和隐私策略未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/rikkahub/rikkahub
- `fractalmind-ai/fractalbot`（P1）：适用场景：Slack/Telegram 等消息渠道到外部 agents 的网关化接入；成熟度：15 stars，协议模型、鉴权、队列和生产部署方式未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/fractalmind-ai/fractalbot
