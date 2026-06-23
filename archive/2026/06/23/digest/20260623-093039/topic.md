## 2026-06-23 09:32 每日主题观察

### Agent runtime 与治理（P0）
- 方向：从“模型 + 函数调用”升级为“模型 + 容器/执行环境 + 状态 + 权限 + 审计”。
- 跟进：Responses API computer environment、Bedrock Stateful Runtime、OpenAI Frontier；同时对比 `superset`、`omnigent`、`gptme` 的本地/开源实现。
- 详情：<https://openai.com/index/equip-responses-api-computer-environment>；<https://openai.com/index/introducing-the-stateful-runtime-environment-for-agents-in-amazon-bedrock>；<https://github.com/superset-sh/superset>；<https://github.com/omnigent-ai/omnigent>；<https://github.com/gptme/gptme>

### Agent 安全、指令层级与闭环评测（P0）
- 方向：prompt injection 防护、instruction hierarchy、coding/security agent 监控与漏洞修复闭环成为工程基线。
- 跟进：把网页/邮件/文档/工具输出注入、敏感数据边界和高风险工具确认加入内部 eval。
- 详情：<https://openai.com/index/designing-agents-to-resist-prompt-injection>；<https://openai.com/index/instruction-hierarchy-challenge>；<https://openai.com/index/codex-security-now-in-research-preview>；<https://openai.com/index/introducing-evmbench>

### 小模型量化与子代理路由（P0/P1）
- 方向：3B/8B/32B finetune 与 GGUF/AWQ 候选服务于本地推理、低显存部署、子代理与批量预处理。
- 跟进：`VibeThinker-3B-LQ8-GGUF`、`AgenticRL-blackbox...`、`Qwen3-8B-AWQ-4bit`、`Llama-3.1-8B-Instruct-AWQ-4bit`；先做 license、模板、吞吐和任务回归评测。
- 详情：<https://huggingface.co/reecdev/VibeThinker-3B-LQ8-GGUF>；<https://huggingface.co/PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c>；<https://huggingface.co/yw223/Qwen3-8B-AWQ-4bit>；<https://huggingface.co/yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit>

### 可回滚、可学习的 Agent 控制（P1）
- 方向：从线性 scratchpad 转向可验证、可撤销、可沉淀规则的 agent 状态机。
- 跟进：GA-Rollback、IDEA/RULEARN、ClinicalAgent、药物发现 agent、OR-LLM-Agent；抽象为“执行—审计—回滚”和“观察—假设—验证—规则修订”。
- 详情：<https://www.semanticscholar.org/paper/743694e2defb4cd81d155e26b04c0fc4a024a9eb>；<https://www.semanticscholar.org/paper/0288769cd4d7777441449b9d379eea08fcc58dd7>；<https://www.semanticscholar.org/paper/e0aab37c1b584e6b0c773dd9e52863106824f1c7>；<https://www.semanticscholar.org/paper/0a63c9327d443b172bb4f755bae7dece52a6aa5c>

### AI Gateway 与前端 Agent UX（P0/P1）
- 方向：推理流量治理与 agent-native UI 正在成为 LLM 应用工程基础设施。
- 跟进：`envoyproxy/ai-gateway` 验证 provider/限流/endpoint picker/Kubernetes；`CopilotKit` 验证 human-in-the-loop、生成式 UI 和状态同步。
- 详情：<https://github.com/envoyproxy/ai-gateway>；<https://github.com/CopilotKit/CopilotKit>

### 数据/知识与长上下文 RAG（P1）
- 方向：skills/MCP/agents 能力目录、知识图谱式推荐与长上下文模型候选值得跟踪，但 license 与安全风险优先。
- 跟进：`stevesolun/ctx`、`heterodoxin/fastcontext-1.0-4b-sft-apostate`；后者候选含 uncensored/abliteration 标签，仅建议隔离研究。
- 详情：<https://github.com/stevesolun/ctx>；<https://huggingface.co/heterodoxin/fastcontext-1.0-4b-sft-apostate>

固定入口：每日汇总 [https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd](https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd)；时间索引 [https://my.feishu.cn/docx/QZjEdsjnRoDVGixlJTOcjx3Dn8b](https://my.feishu.cn/docx/QZjEdsjnRoDVGixlJTOcjx3Dn8b)；主题索引 [https://my.feishu.cn/docx/OeMPdOXCSoG6JDxWU3qc5fcRn1c](https://my.feishu.cn/docx/OeMPdOXCSoG6JDxWU3qc5fcRn1c)。
