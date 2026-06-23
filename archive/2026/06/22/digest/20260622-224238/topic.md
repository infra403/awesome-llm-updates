## 2026-06-22 22:42 每日主题观察

### 评测与上线准入
- **P0：部署前仿真成为模型发布流程核心能力**。OpenAI Deployment Simulation 用真实 conversation data 模拟部署场景，建议跟进真实流量匿名化、场景分层、行为回放、安全/拒答/工具调用回归。详情：https://openai.com/index/deployment-simulation ，每日汇总：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
- **P1：评测从静态题库扩展到领域专家、多语言代码和多轮安全关键红队**。关注 LifeSciBench、Multi-LCB、NRT-Bench、Contagion Networks。详情：https://openai.com/index/introducing-life-sci-bench ，https://arxiv.org/abs/2606.20517v1 ，https://arxiv.org/abs/2606.20408v1 ，https://arxiv.org/abs/2606.20493v1

### Coding Agent / 企业 Agent
- **P0：Coding Agent 企业化基线是持久环境 + sandbox + approvals + telemetry**。OpenAI 收购 Ona、Codex on AWS、Dell hybrid/on-prem 与 Codex 安全运行实践应合并跟踪。详情：https://openai.com/index/openai-to-acquire-ona ，https://openai.com/index/openai-frontier-models-and-codex-are-now-available-on-aws ，https://openai.com/index/dell-codex-enterprise-partnership ，https://openai.com/index/running-codex-safely
- **P1：仓库指导需要可迭代评测**。Probe-and-Refine 提示 AGENTS.md 不应一次性编写，而应通过失败任务探测、精炼说明、回归验证来维护。详情：https://arxiv.org/abs/2606.20512v1

### Agent/RAG 上下文工程
- **P1：上下文预算管理从 recency truncation 走向显式选择器**。PACMS 将上下文保留建模为 submodular context selection，适合跟进 Agent memory、工具输出、对话历史的预算管理。详情：https://arxiv.org/abs/2606.20047v1
- **P1：流式 RAG 的关键不是越早检索越好，而是 tool intent 何时稳定**。建议后续实验标注意图稳定点，并比较提前检索与输入结束后检索的成本/延迟/错误上下文。详情：https://arxiv.org/abs/2606.20113v1

### 推理系统与端侧实时 Agent
- **P1：端侧/物理 AI serving 需要可恢复执行状态**。Execution-State Capsules 将复用对象从 KV cache 扩到图绑定 execution-state checkpoint/restore，适合关注低延迟、小 batch、分支/重置/中断/重入场景。详情：https://arxiv.org/abs/2606.20537v1
- **P2：性能工程 Agent 要结构化使用证据**。AutoPass 展示 compiler/runtime 证据引导多 Agent 调优，适合后续跟进 profile、IR、测量噪声与置信度如何进入 Agent loop。详情：https://arxiv.org/abs/2606.20373v1

### 垂直科学与数据工程
- **P1：生命科学正在形成专用模型 + 专家评测闭环**。GPT-Rosalind 与 LifeSciBench 指向 biological reasoning、medicinal chemistry、genomics analysis、experimental workflow 与专家评审。详情：https://openai.com/index/introducing-new-capabilities-to-gpt-rosalind ，https://openai.com/index/introducing-life-sci-bench
- **P1：医疗诊断类 reasoning model 必须保留专家确认和证据链**。OpenAI 报道罕见儿童遗传病诊断案例，应作为专家辅助方向观察，不应无监督自动化。详情：https://openai.com/index/diagnose-rare-childhood-diseases

### 待补齐入口
- 模型发布固定文档本轮未提供新增模型卡/开源权重条目；下一轮需要补齐参数、上下文、许可证、权重状态与推理框架适配。
- GitHub 固定文档本轮未提供新增项目条目；下一轮需要补齐 Agent/RAG/MCP/推理框架/评测工具项目的 stars、增长和成熟度。
