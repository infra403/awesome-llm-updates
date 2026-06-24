## 2026-06-24 21:10 论文主题条目

### 模型发布与模型能力

- Qwen-AgentWorld: Language World Models for General Agents
  - 重要性：P0
  - 为什么值得看：把 Qwen 系模型与 Agent 世界模型结合，目标是模拟 agentic environments；可能改变 Agent 训练、规划验证和离线评测的数据来源。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24597v1

### Agent 与多智能体

- Are We Ready For An Agent-Native Memory System?
  - 重要性：P0
  - 为什么值得看：把长期记忆从黑盒 RAG 成功率拆成存储、检索、更新、合并、生命周期治理等系统能力，适合作为 Agent memory eval 的工程清单。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24775v1
- SHERLOC: Structured Diagnostic Localization for Code Repair Agents
  - 重要性：P0
  - 为什么值得看：面向代码修复 Agent 的故障定位，强调输出诊断上下文而不是文件级检索结果，可减少定位阶段工具预算浪费。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24820v1
- Poisoned Playbooks: Demystifying Knowledge Poisoning Effects on AI Security Agents
  - 重要性：P0
  - 为什么值得看：把 RAG 投毒从问答污染扩展到行动型安全 Agent，提醒团队检查 playbook 来源、证据链和行动前验证。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24402v1
- Grading the Grader: Lessons from Evaluating an Agentic Data Analysis System
  - 重要性：P0
  - 为什么值得看：评估数据分析 Agent 时，自动 grader 可能把自身 artifact 误判为 Agent 错误；适合改进 LLM-as-judge 流程。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24839v1
- Qwen-AgentWorld: Language World Models for General Agents
  - 重要性：P0
  - 为什么值得看：语言世界模型可成为 Agent 规划、仿真和后训练的新组件，但需确认开放程度、模拟偏差和部署成本。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24597v1

### RAG 与知识工程

- Privacy-Preserving RAG via Multi-Agent Semantic Rewriting: Achieving Confidentiality Without Compromising Contextual Fidelity
  - 重要性：P0
  - 为什么值得看：在检索内容进入生成前做多 Agent 语义改写脱敏，适合企业敏感知识库评估隐私与语义保真的折中。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24623v1
- Poisoned Playbooks: Demystifying Knowledge Poisoning Effects on AI Security Agents
  - 重要性：P0
  - 为什么值得看：RAG 知识源一旦被污染，安全 Agent 可能把错误 write-up 操作化；需要知识库 provenance 和 sandbox 验证。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24402v1

### 推理、训练与后训练

- Qwen-AgentWorld: Language World Models for General Agents
  - 重要性：P0
  - 为什么值得看：如果世界模型能生成高质量交互轨迹，将影响 Agent 后训练、规划器训练和安全 rehearsal；证据仍需完整论文确认。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24597v1

### 推理系统与工程工具

- SHERLOC: Structured Diagnostic Localization for Code Repair Agents
  - 重要性：P0
  - 为什么值得看：将定位阶段改造成结构化诊断，可作为代码 Agent 中间表示，帮助后续编辑器更快收敛。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24820v1
- AVOC: Enhancing Hour-Level Audio-Video Understanding in Omni-Modal LLMs via Retrieval-Inspired Token Compression
  - 重要性：P0
  - 为什么值得看：把长音视频理解瓶颈转化为 token 压缩问题，适合启发会议/长视频 Agent 的索引与上下文预算设计。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24286v1
- Grad Detect: Gradient-Based Hallucination Detection in LLMs
  - 重要性：P0
  - 为什么值得看：尝试用模型内部梯度信号检测幻觉；工程上要重点核查 forward-backward 带来的显存、延迟和闭源 API 不可用问题。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24790v1

### 多模态与生成媒体

- AVOC: Enhancing Hour-Level Audio-Video Understanding in Omni-Modal LLMs via Retrieval-Inspired Token Compression
  - 重要性：P0
  - 为什么值得看：针对小时级音视频理解的 token 冗余和上下文窗口限制，提出可学习压缩层，值得长视频问答和会议理解系统关注。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24286v1

### 评测与基准

- Are We Ready For An Agent-Native Memory System?
  - 重要性：P0
  - 为什么值得看：提示 Agent memory 评测应从端到端成功率扩展到内部数据管理能力，能直接改造测试集设计。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24775v1
- Grad Detect: Gradient-Based Hallucination Detection in LLMs
  - 重要性：P0
  - 为什么值得看：为幻觉检测提供内部信号路线，适合作为高风险输出校验的研究备选。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24790v1
- Grading the Grader: Lessons from Evaluating an Agentic Data Analysis System
  - 重要性：P0
  - 为什么值得看：指出自动 grader 本身的可靠性问题，适合所有依赖 LLM-as-judge 的 Agent 评测平台复查。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24839v1

### 产品与商业化

- Privacy-Preserving RAG via Multi-Agent Semantic Rewriting: Achieving Confidentiality Without Compromising Contextual Fidelity
  - 重要性：P0
  - 为什么值得看：企业 RAG 商业化经常卡在敏感信息泄漏；该方向可作为检索后脱敏与合规审计中间层的参考。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24623v1

### 数据集与数据工程

- Grading the Grader: Lessons from Evaluating an Agentic Data Analysis System
  - 重要性：P0
  - 为什么值得看：数据分析 Agent 评测需要保存代码、数值结果和诊断文本等复合产物，这会影响数据集 schema 与评测流水线设计。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.24839v1
