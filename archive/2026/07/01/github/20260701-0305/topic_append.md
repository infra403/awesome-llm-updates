## 2026-07-01 03:05 GitHub 项目主题条目

### Agent 与多智能体
- 0xSteph/pentest-ai（P0）｜适用场景：红队/漏洞验证 Agent、MCP 安全工具编排、OWASP/SPA 探测自动化。成熟度：stars 1160，README 有 PyPI/CI 信号；工具覆盖、误报率和危险动作隔离未实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/0xSteph/pentest-ai
- mohitagw15856/pm-claude-skills（P0）｜适用场景：企业 skill 目录、产品管理/运营流程 Agent、跨助手 skill 分发。成熟度：stars 1100，README 显示 npm/PyPI/MCP 分发；skill 质量一致性未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/mohitagw15856/pm-claude-skills
- osaurus-ai/osaurus（P0）｜适用场景：macOS 端侧 Agent runtime、本地 memory/tools/identity、离线桌面 Agent。成熟度：stars 6479，README 有 release 信号；仅 macOS/Swift 路线，跨平台性未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/osaurus-ai/osaurus
- corezoid/corezoid-ai-plugin（P0）｜适用场景：垂直 SaaS/流程平台接入 Claude Code/Codex，MCP tools + 领域 skills。成熟度：stars 67，README 有 Go MCP server 与 skill 列表；生产权限模型未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/corezoid/corezoid-ai-plugin
- speakeasy-api/gram（P0）｜适用场景：组织级 agent/MCP/skill 控制平面、MCP gateway、OpenAPI 工具治理。成熟度：stars 251，Speakeasy 背景强；开源边界和商业依赖需确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/speakeasy-api/gram
- msu-denver/bili-core（P1）｜适用场景：单 Agent、多 Agent、RAG app 与 adversarial security testing 的研究框架。成熟度：stars 14，README 有 CI/release/Python 3.11+/MIT；偏早期。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/msu-denver/bili-core
- kochetkov-ma/claude-brewcode（P1）｜适用场景：Claude Code 长任务上下文交接、skills/agents/hooks、quorum review。成熟度：stars 28，README 提供 release 和外部文档；生态绑定 Claude Code。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/kochetkov-ma/claude-brewcode
- lidge-jun/opencodex（P1）｜适用场景：Codex 生态多 provider 路由、LLM gateway/provider adapter。成熟度：stars 207，README 有 npm 入口；候选标注 actionability_needs_validation，需 POC。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/lidge-jun/opencodex

### RAG 与知识工程
- msu-denver/bili-core（P1）｜适用场景：RAG 应用构建/测试、多 Agent 研究和安全红队评测。成熟度：stars 14，CI/release 已见；模块能力未运行。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/msu-denver/bili-core
- GoogleCloudPlatform/db-context-enrichment（P1）｜适用场景：数据库 schema/context enrichment、NL2SQL、ContextSet 版本化和 MCP 化数据库工具。成熟度：stars 32，GoogleCloudPlatform 组织来源但 README 明确 not officially supported；Python/MCP 重组后稳定性未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/GoogleCloudPlatform/db-context-enrichment

### 推理、训练与后训练
- chrisliu298/awesome-on-policy-distillation（P0）｜适用场景：OPD、RLHF、自蒸馏、speculative decoding、teacher-student 训练路线调研。成熟度：stars 437，README 显示 Entries 391；awesome list 非工具库，条目质量未审计。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/chrisliu298/awesome-on-policy-distillation

### 推理系统与工程工具
- 0xSteph/pentest-ai（P0）｜适用场景：MCP 工具权限、安全审计、Agent 触发危险动作的策略设计。成熟度：stars 1160，README 已确认；安全边界未实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/0xSteph/pentest-ai
- mohitagw15856/pm-claude-skills（P0）｜适用场景：skill packaging、MCP/Remote MCP 分发、跨 Agent 工作流资产管理。成熟度：stars 1100，多分发徽章已见；质量分层未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/mohitagw15856/pm-claude-skills
- osaurus-ai/osaurus（P0）｜适用场景：端侧 Agent harness、本地推理/工具接入、memory 与身份隔离。成熟度：stars 6479，release 信号已见；API 稳定性未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/osaurus-ai/osaurus
- corezoid/corezoid-ai-plugin（P0）｜适用场景：流程引擎自然语言编排、MCP tool + skill 的企业流程插件形态。成熟度：stars 67，README 已确认；生产部署未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/corezoid/corezoid-ai-plugin
- speakeasy-api/gram（P0）｜适用场景：LLM/MCP gateway、组织级权限、OpenAPI-to-tool、可观测性。成熟度：stars 251，README 定位清晰；开源/托管边界需确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/speakeasy-api/gram
- kochetkov-ma/claude-brewcode（P1）｜适用场景：agentic coding 长任务生命周期、自动 review、项目规则持久化。成熟度：stars 28，README 已确认；低热度需观察。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/kochetkov-ma/claude-brewcode
- lidge-jun/opencodex（P1）｜适用场景：Codex provider proxy、OpenAI/Codex 协议兼容、多模型开发工具路由。成熟度：stars 207，npm 安装入口已见；兼容矩阵和安全需实验。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/lidge-jun/opencodex

### 模型发布与模型能力
- osaurus-ai/osaurus（P0）｜适用场景：Apple Foundation Models/MLX/本地模型接入的桌面 Agent 能力验证。成熟度：stars 6479，README 已确认本地/离线定位；具体模型支持需验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/osaurus-ai/osaurus
- chrisliu298/awesome-on-policy-distillation（P0）｜适用场景：模型蒸馏与后训练文献雷达，支撑小模型能力优化路线。成熟度：stars 437，entries 多；非可执行框架。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/chrisliu298/awesome-on-policy-distillation

### 评测与基准
- 0xSteph/pentest-ai（P0）｜适用场景：Agent 安全测试、漏洞验证闭环、红队工具评估。成熟度：stars 1160；误报率和测试基准未实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/0xSteph/pentest-ai
- chrisliu298/awesome-on-policy-distillation（P0）｜适用场景：后训练/蒸馏 benchmark 和论文工具入口。成熟度：awesome list，质量需抽样。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/chrisliu298/awesome-on-policy-distillation
- msu-denver/bili-core（P1）｜适用场景：LLM app benchmarking、adversarial testing、security red-teaming。成熟度：stars 14，研究框架早期。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/msu-denver/bili-core
- GoogleCloudPlatform/db-context-enrichment（P1）｜适用场景：NL2SQL 上下文集效果评估、数据库 schema enrichment 质量验证。成熟度：stars 32，重组后需观察。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/GoogleCloudPlatform/db-context-enrichment

### 产品与商业化
- mohitagw15856/pm-claude-skills（P0）｜适用场景：skill marketplace、产品管理 Agent、prompt/skill 资产商品化。成熟度：stars 1100，多分发通道；官方目录状态未二次核验。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/mohitagw15856/pm-claude-skills
- corezoid/corezoid-ai-plugin（P0）｜适用场景：企业流程平台 AI 插件化与自然语言 workflow automation。成熟度：stars 67，垂直场景清晰；生态规模待观察。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/corezoid/corezoid-ai-plugin
- speakeasy-api/gram（P0）｜适用场景：企业 AI 控制平面、MCP/agent 治理产品。成熟度：stars 251，厂商背景强；商业托管边界未确认。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/speakeasy-api/gram

### 数据集与数据工程
- GoogleCloudPlatform/db-context-enrichment（P1）｜适用场景：结构化数据库上下文集生成、schema/业务术语/SQL 模板管理。成熟度：stars 32，README 已确认 ContextSet 概念；真实数据库连接风险和权限策略需验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g｜原文：https://github.com/GoogleCloudPlatform/db-context-enrichment
