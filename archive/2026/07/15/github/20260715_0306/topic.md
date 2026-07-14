## 2026-07-15 03:06 GitHub 项目主题条目

### Agent 与多智能体
- **KnockOutEZ/wigolo**（P0）：适用场景：给 Claude Code/Codex/Cursor 等 Agent 接入本地 Web search/fetch/crawl/research MCP 工具层；成熟度：public beta、stars 89，README 已确认快速安装，实际稳定性未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/KnockOutEZ/wigolo
- **anthony-chaudhary/fak**（P1）：适用场景：Agent runtime/gateway 的长会话缓存、上下文压缩、模型路由和工具调用 guard 实验；成熟度：stars 12，README 已确认 Go 单二进制与 `fak guard` 形态，兼容性未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/anthony-chaudhary/fak
- **sumamovva/probeagent**（P1）：适用场景：Agent 预发布安全红队、prompt injection/credential exfiltration/guardrail 验证；成熟度：stars 16，README 已确认 CLI 和三类 verdict，grader 为文本启发式；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/sumamovva/probeagent
- **AI-Colleagues/orcheo**（P1）：适用场景：Agent workflow 编排、vibe-coding 平台 UX/SDK 参考；成熟度：Beta、stars 13，PyPI/npm/GHCR 发布形态已确认，生产稳定性未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/AI-Colleagues/orcheo
- **RA-CONSULTING/Aureon-OS**（P1）：适用场景：可审计 Agent 操作台/本地控制台概念参考；成熟度：stars 29，README 有测试/ruff/mypy badge，但产品叙事强于可复用接口，建议暂不跟进；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/RA-CONSULTING/Aureon-OS

### RAG 与知识工程
- **KnockOutEZ/wigolo**（P0）：适用场景：本地优先 Web/RAG 检索 sidecar，统一 search、fetch、crawl、extract、cache；成熟度：public beta、stars 89，README 已确认 Node ≥20 和 MCP 接入，检索质量未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/KnockOutEZ/wigolo
- **aws-samples/sample-amazon-bedrock-for-beginners**（P1）：适用场景：AWS Bedrock Knowledge Bases RAG、Guardrails、Converse API 和 Strands Agent 的团队入门样例；成熟度：AWS samples、stars 39，README 已确认运行步骤，依赖 AWS 账号/IAM；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/aws-samples/sample-amazon-bedrock-for-beginners

### 推理系统与工程工具
- **KnockOutEZ/wigolo**（P0）：适用场景：Agent 工具层统一与本地 sidecar 架构，降低外部 API 成本和数据外发；成熟度：public beta，跨平台资源占用与 crawl 合规未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/KnockOutEZ/wigolo
- **anthony-chaudhary/fak**（P1）：适用场景：prompt cache、local GGUF fallback、模型路由和工具调用判定的 Agent kernel 方案；成熟度：stars 12，README 已确认方向，性能数字未复测；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/anthony-chaudhary/fak
- **AI-Colleagues/orcheo**（P1）：适用场景：工作流平台、SDK/backend/studio 一体化发布与 Agent 自动部署设计参考；成熟度：Beta，实际运行语义和权限模型未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/AI-Colleagues/orcheo
- **aws-samples/sample-amazon-bedrock-for-beginners**（P1）：适用场景：Bedrock Converse API、tool use、Guardrails 的云上推理应用样例；成熟度：教学仓，运行成本与权限配置未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/aws-samples/sample-amazon-bedrock-for-beginners

### 推理、训练与后训练
- **yjyddq/DARE**（P1）：适用场景：diffusion LLM 的 SFT/RL 训练、rollout 与 eval infra 研究；成熟度：stars 213、Apache-2.0、work-in-progress，训练资源需求和支持模型清单未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/yjyddq/DARE

### 模型发布与模型能力
- **yjyddq/DARE**（P1）：适用场景：跟踪 dLLM 能力、训练范式和 HuggingFace 权重/infra 集成；成熟度：论文链接和 README 已确认，但候选 actionability weak，建议持续观察；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/yjyddq/DARE

### 评测与基准
- **sumamovva/probeagent**（P1）：适用场景：Agent 安全评测、红队攻击集和 guardrail 阻断效果验证；成熟度：README 已确认 verdict 逻辑，但 grader 非环境验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/sumamovva/probeagent
- **yjyddq/DARE**（P1）：适用场景：dLLM benchmark evaluation 扩展；成熟度：work-in-progress，评测覆盖未实测；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/yjyddq/DARE

### 产品与商业化
- **aws-samples/sample-amazon-bedrock-for-beginners**（P1）：适用场景：Bedrock 云上 AI 应用 onboarding、销售/方案验证和团队培训材料；成熟度：AWS samples 教学仓，非生产框架；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/aws-samples/sample-amazon-bedrock-for-beginners
- **RA-CONSULTING/Aureon-OS**（P1）：适用场景：AI 操作台产品叙事、审计与控制台概念参考；成熟度：早期且定位混杂，暂不建议工程投入；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/RA-CONSULTING/Aureon-OS
