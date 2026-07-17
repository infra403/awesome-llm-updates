## 2026-07-17 15:06 GitHub 项目主题条目

### 模型发布与模型能力

- **modelscope/mcore-bridge**（P1）：适用场景：Megatron-Core 训练/微调、多模型定义复用、LLM/多模态模型支持矩阵评估。成熟度：86 stars，中早期；支持模型数量、版本兼容矩阵、分布式训练稳定性和示例可复现性需要实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/modelscope/mcore-bridge

### Agent 与多智能体

- **cynative/cynative**（P0）：适用场景：Agent 安全边界、只读工具调用、云资产问答、威胁狩猎和 sandbox 设计参考。成熟度：129 stars，中低规模；安全场景定位清晰，但生产安装、支持的云资源深度与误报治理未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/cynative/cynative
- **RedPlanetHQ/core**（P0）：适用场景：个人/团队 Agent OS、记忆层、MCP 工具层、本地模型接入和自动化任务编排。成熟度：1901 stars，生态信号强；安装复杂度、插件稳定性、跨平台支持和数据迁移能力未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/RedPlanetHQ/core
- **repowise-dev/repowise**（P0）：适用场景：代码库 RAG、Agent coding 前置索引、静态分析、代码健康评分和 MCP 上下文暴露。成熟度：3675 stars，本批最高；支持语言范围、MCP schema 与 CI 集成方式仍需 README/实测确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/repowise-dev/repowise
- **TserenTserenov/FMT-exocortex-template**（P1）：适用场景：Claude Code 个人知识系统、agent skills 组织、MCP 与多智能体工作流模板参考。成熟度：42 stars，早期项目；部署脚本、权限模型和多用户协作能力未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/TserenTserenov/FMT-exocortex-template
- **keros68/metrik**（P1）：适用场景：Claude Code/Codex 等 Agent 的 token、配额、成本 observability 与桌面提醒。成熟度：13 stars，早期且弱 engagement；官方配额读取接口、provider 支持和数据采集准确性未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/keros68/metrik
- **yingyingxia666/awesome-agentic**（P1）：适用场景：Agentic RL、Reasoning RL、OPD 与多智能体方向的研究索引。成熟度：23 stars，curated list 类型；内容完整性、更新频率和论文质量筛选标准未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/yingyingxia666/awesome-agentic

### RAG 与知识工程

- **RedPlanetHQ/core**（P0）：适用场景：个人 AI OS 中的记忆层、长期上下文、自动化与 MCP 连接。成熟度：1901 stars，生态信号强；插件稳定性和数据迁移能力未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/RedPlanetHQ/core
- **repowise-dev/repowise**（P0）：适用场景：代码库文档自动生成、架构决策记录、Git 分析和代码健康索引，作为 coding agent 的 RAG 上下文。成熟度：3675 stars；支持语言范围和 MCP schema 需实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/repowise-dev/repowise
- **TserenTserenov/FMT-exocortex-template**（P1）：适用场景：个人知识库模板、second brain/exocortex、skills 与知识管理结构参考。成熟度：42 stars，早期项目；模板质量和部署链路未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/TserenTserenov/FMT-exocortex-template

### 推理、训练与后训练

- **yingyingxia666/awesome-agentic**（P1）：适用场景：后训练、推理强化、Agentic RL 和多智能体论文跟踪。成熟度：23 stars，研究列表类型；质量筛选标准未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/yingyingxia666/awesome-agentic
- **modelscope/mcore-bridge**（P1）：适用场景：Megatron-Core 模型定义、LLM/多模态模型训练和 PEFT/LoRA 工程接入。成熟度：86 stars，中早期；分布式训练稳定性和示例可复现性需要实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/modelscope/mcore-bridge

### 推理系统与工程工具

- **cynative/cynative**（P0）：适用场景：只读安全 Agent、云/代码/runtime 查询工具、权限分层与 sandbox 设计。成熟度：129 stars；云资源深度、误报治理和安装方式未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/cynative/cynative
- **RedPlanetHQ/core**（P0）：适用场景：MCP、Ollama、本地 automation 和开发工具聚合。成熟度：1901 stars；跨平台支持和插件稳定性未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/RedPlanetHQ/core
- **repowise-dev/repowise**（P0）：适用场景：静态分析、代码健康、死代码检测、Git analytics 与 MCP 工具暴露。成熟度：3675 stars；CI 集成和语言覆盖需实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/repowise-dev/repowise
- **keros68/metrik**（P1）：适用场景：Agent token/配额/成本观测，本地优先桌面监控。成熟度：13 stars，早期；数据采集准确性未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/keros68/metrik

### 多模态与生成媒体

- **modelscope/mcore-bridge**（P1）：适用场景：多模态大模型的 Megatron-Core 定义与训练接入。成熟度：86 stars；支持 200+ 多模态模型的范围和版本兼容性需核对。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/modelscope/mcore-bridge

### 产品与商业化

- **keros68/metrik**（P1）：适用场景：Agent 使用成本透明化、配额提醒、团队或个人用量治理产品参考。成熟度：13 stars，早期；官方配额读取能力和 provider 覆盖未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/keros68/metrik
