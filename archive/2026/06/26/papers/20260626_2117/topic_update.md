## 2026-06-26 21:17 论文主题条目

### Agent 与多智能体

- OpenRCA 2.0: From Outcome Labels to Causal Process Supervision
  - 重要性：P0
  - 为什么值得看：把 RCA Agent 评测从“是否答对根因”推进到“是否能追踪故障传播路径”，适合改造运维 Agent、长上下文工具调用和 RAG 排障 eval。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27154v1
- MIRROR: Novelty-Constrained Memory-Guided MCTS Red-Teaming for Agentic RAG
  - 重要性：P0
  - 为什么值得看：把 Agentic RAG 红队从 prompt injection 扩展到文本投毒、图像注入、直接查询和工具编排操纵，并强调攻击样本新颖性。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26793v1
- Temporal Validity in Retrieval Memory: Eliminating Stale-Fact Errors for AI Agents over Evolving Knowledge
  - 重要性：P0
  - 为什么值得看：把 stale-fact 错误定义为 Agent/RAG 记忆架构问题，提示需要时间有效期、版本和冲突消解机制。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26511v1
- A hardware-safety-gated system for LLM-written native ARTIQ control code on a trapped-ion platform
  - 重要性：P0
  - 为什么值得看：给“LLM 写代码并操作真实设备/生产系统”提供硬安全 gate 思路，强调操作级权限、审计和人工授权边界。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27231v1
- When Does Combining Language Models Help? A Co-Failure Ceiling on Routing, Voting, and Mixture-of-Agents Across 67 Frontier Models
  - 重要性：P0
  - 为什么值得看：提出 co-failure ceiling，提醒多模型路由/投票/MoA 评测必须看所有模型共同失败的查询集合。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27288v1
- Agents That Know Too Much: A Data-Centric Survey of Privacy in LLM Agents
  - 重要性：P0
  - 为什么值得看：从数据源、工具调用、长期记忆、跨会话状态和日志角度梳理 Agent 隐私风险，适合补平台安全 checklist。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26627v1
- CHIA: An open-source framework for principled, agentic AI-driven hardware/software co-design research
  - 重要性：P0
  - 为什么值得看：把硬件/软件协同设计中的 Agent workflow 框架化，可观察专业研发 Agent 平台如何组织工具、评测与人类监督。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27350v1

### RAG 与知识工程

- OpenRCA 2.0: From Outcome Labels to Causal Process Supervision
  - 重要性：P0
  - 为什么值得看：RCA 场景通常依赖日志、指标、trace 和知识检索；过程级标签可用于评测 RAG 排障链条是否真正追因。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27154v1
- MIRROR: Novelty-Constrained Memory-Guided MCTS Red-Teaming for Agentic RAG
  - 重要性：P0
  - 为什么值得看：直接面向 Agentic RAG 的跨表面攻击生成和去重问题，适合转化为内部 RAG 安全回归集。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26793v1
- Temporal Validity in Retrieval Memory: Eliminating Stale-Fact Errors for AI Agents over Evolving Knowledge
  - 重要性：P0
  - 为什么值得看：指出 embedding 相似度难以区分重复事实与被新事实推翻的旧事实，推动 RAG 记忆加入时间语义。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26511v1

### 评测与基准

- OpenRCA 2.0: From Outcome Labels to Causal Process Supervision
  - 重要性：P0
  - 为什么值得看：代表从答案级评测转向过程级评测，对 Agent 可靠性和可解释性更有区分度。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27154v1
- MIRROR: Novelty-Constrained Memory-Guided MCTS Red-Teaming for Agentic RAG
  - 重要性：P0
  - 为什么值得看：把红队样本新颖性作为评测质量问题，避免 benchmark 被重复模板污染。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26793v1
- When Does Combining Language Models Help? A Co-Failure Ceiling on Routing, Voting, and Mixture-of-Agents Across 67 Frontier Models
  - 重要性：P0
  - 为什么值得看：给多模型组合系统提供上限诊断指标，能影响路由实验和报表设计。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27288v1

### 推理系统与工程工具

- A hardware-safety-gated system for LLM-written native ARTIQ control code on a trapped-ion platform
  - 重要性：P0
  - 为什么值得看：把 Agent 代码执行安全从策略文本推进到硬件/系统 gate，适合真实执行环境参考。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27231v1
- Resource-Aware Neuro-Symbolic Reasoning for Local Small Language Models
  - 重要性：P0
  - 为什么值得看：用符号求解器承担确定性推理，可能降低本地小模型多采样成本并增强可验证性。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27281v1
- CHIA: An open-source framework for principled, agentic AI-driven hardware/software co-design research
  - 重要性：P0
  - 为什么值得看：提供专业研发场景下 Agent workflow 编排框架线索，适合系统/编译器/硬件工具链团队跟进。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27350v1

### 推理、训练与后训练

- Resource-Aware Neuro-Symbolic Reasoning for Local Small Language Models
  - 重要性：P0
  - 为什么值得看：为小模型结构化推理提供 VFR-LLM 路线，强调 formalization、consistency check 和 deterministic solver。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27281v1

### 模型发布与模型能力

- When Does Combining Language Models Help? A Co-Failure Ceiling on Routing, Voting, and Mixture-of-Agents Across 67 Frontier Models
  - 重要性：P0
  - 为什么值得看：衡量多模型组合是否真的能突破单模型能力时，需要关注共同失败率，而不是只看平均性能。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27288v1
- Resource-Aware Neuro-Symbolic Reasoning for Local Small Language Models
  - 重要性：P0
  - 为什么值得看：把小模型能力边界与外部符号推理结合，可能改变端侧模型能力设计。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27281v1

### 多模态与生成媒体

- MIRROR: Novelty-Constrained Memory-Guided MCTS Red-Teaming for Agentic RAG
  - 重要性：P0
  - 为什么值得看：候选摘要明确覆盖 multimodal agentic RAG 与 image injection，可作为多模态 RAG 安全测试入口。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26793v1

### 数据集与数据工程

- Temporal Validity in Retrieval Memory: Eliminating Stale-Fact Errors for AI Agents over Evolving Knowledge
  - 重要性：P0
  - 为什么值得看：要求知识数据工程显式建模事实版本、有效时间与替代关系，否则 RAG 会混用新旧事实。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26511v1
- Agents That Know Too Much: A Data-Centric Survey of Privacy in LLM Agents
  - 重要性：P0
  - 为什么值得看：把隐私风险放在 Agent 全数据流上看，有助于设计最小权限、日志脱敏、记忆治理和审计策略。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26627v1

### 产品与商业化

- Agents That Know Too Much: A Data-Centric Survey of Privacy in LLM Agents
  - 重要性：P0
  - 为什么值得看：企业 Agent 产品上线前，隐私风险会影响合规、客户信任和权限模型，适合产品安全评审引用。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26627v1
