## 2026-07-16 03:05 GitHub 项目主题条目

### Agent 与多智能体

- mlhher/late-cli（P0）：适用场景为 AI coding agent 编排、上下文隔离、本地/云模型混合开发流；成熟度为 379 stars，README 已确认静态二进制和安装方式，但 benchmark 未本地复测；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/mlhher/late-cli
- wellwelwel/lagune（P0）：适用场景为 Agent 参与安全加固、spec-driven security、开发期 blue-team 辅助；成熟度为 71 stars，README 已确认 npx 本地 dashboard 和多 Agent 支持声明，安全效果未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/wellwelwel/lagune
- hoophq/hoop（P0）：适用场景为 AI Agent/MCP Client 访问数据库、Kubernetes、API 时的网关治理、审批和审计；成熟度为 760 stars，README 已确认生产访问控制定位，实际部署延迟和协议覆盖未复测；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/hoophq/hoop
- kagent-dev/kagent（P0）：适用场景为 Kubernetes 原生 Agent 部署、DevOps Agent 和云原生多 Agent 管理；成熟度为 3312 stars，README 已确认 release/CI/社区信号，集群内 API 稳定性未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/kagent-dev/kagent
- Fmarzochi/EGC（P1）：适用场景为跨 coding agent/IDE 的项目级持久记忆、状态恢复和命令守护；成熟度为 32 stars，README 已确认 npm 安装和多工具支持声明，实际跨工具接入未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/Fmarzochi/EGC
- dzianisv/opencode-mobile（P1）：适用场景为移动端 coding agent 会话、tool call approval、diff review 和远程会话管理；成熟度为 25 stars，README 已确认 Android/F-Droid/APK，iOS 与 Google Play 未正式可用；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/dzianisv/opencode-mobile
- fastagent-sh/fastagent（P1）：适用场景为把本地 Agent directory 服务化为 HTTP/SSE、Webhook、GitHub bot、Telegram bot；成熟度为 15 stars，README 已确认 serving/adapters 设计，但生产采用弱；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/fastagent-sh/fastagent

### RAG 与知识工程

- bartolli/codanna（P0）：适用场景为 coding agent 的本地代码 RAG、符号搜索、调用图分析和 MCP 工具层；成熟度为 706 stars，Rust/Apache-2.0，README 已确认安装与索引命令，语言覆盖和大仓库性能未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/bartolli/codanna
- SynapseKit/SynapseKit（P1）：适用场景为 async-first RAG、Agent 和 Graph workflow 应用开发；成熟度为 21 stars，README 已确认 PyPI/docs/多 provider 与 vector store 声明，生态仍早期；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/SynapseKit/SynapseKit
- Fmarzochi/EGC（P1）：适用场景为项目上下文记忆、偏好和失败经验沉淀，可作为 Agent 记忆层设计参考；成熟度为 32 stars，README 已确认本地 runtime 定位，隐私边界和状态冲突处理未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/Fmarzochi/EGC

### 推理系统与工程工具

- mlhher/late-cli（P0）：适用场景为小模型/云模型结合的 coding agent、MCP/Skills 接入和低上下文成本编排；成熟度为 379 stars，README 已确认本地 llama-server 与 OpenAI-compatible API 支持，实际模型效果未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/mlhher/late-cli
- bartolli/codanna（P0）：适用场景为 Agent 工具箱中的代码索引与检索基础设施；成熟度为 706 stars，README 已确认 CLI/MCP server 方向，延迟和增量索引未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/bartolli/codanna
- hoophq/hoop（P0）：适用场景为 LLM gateway、MCP 安全代理、生产系统访问控制；成熟度为 760 stars，README 已确认会话审计/审批/脱敏功能，策略能力未实测；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/hoophq/hoop
- kagent-dev/kagent（P0）：适用场景为 K8s Agent runtime、云原生 Agent 平台、DevOps 自动化；成熟度为 3312 stars，README 已确认 Kubernetes native 定位，部署复杂度未验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/kagent-dev/kagent
- timothystewart6/vllm-gb10（P1）：适用场景为 NVIDIA DGX Spark GB10/sm_121a 上的 vLLM 推理镜像和可复现版本 pinning；成熟度为 33 stars，README 已确认 GHCR/Docker 示例和硬件限制，未在 GB10 硬件验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/timothystewart6/vllm-gb10

### 评测与基准

- SynapseKit/SynapseKit（P1）：适用场景为观察轻量 LLM 框架的测试、可观测性和 structured output 设计；成熟度为 21 stars，README 有测试徽章声明但未独立复核；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/SynapseKit/SynapseKit

### 产品与商业化

- dzianisv/opencode-mobile（P1）：适用场景为 AI coding agent 的移动端产品形态、远程审批和自托管连接；成熟度为 25 stars，README 已确认 F-Droid/直接 APK 和功能列表，平台覆盖有限；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/dzianisv/opencode-mobile
- fastagent-sh/fastagent（P1）：适用场景为把本地 Agent 发布为用户可访问的服务、bot 或 webhook handler；成熟度为 15 stars，README 已确认 channel adapter 方向，早期项目需观察；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/fastagent-sh/fastagent
