## 2026-06-26 09:13 论文主题条目

### Agent 与多智能体

- Probabilistic Agents in Deterministic Audits: Evaluating Multi-Agent Systems for Automated Audits Based on the German IT-Grundschutz
  - 重要性：P0
  - 为什么值得看：把多 Agent 放进 IT-Grundschutz / NIS-2 合规审计这类确定性、高责任场景中评估，能帮助工程团队思考 Agent 的证据链、流程约束、可审计性和人工复核接口。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.25622v1

### RAG 与知识工程

- Invoice Haystack: Benchmarking Document Retrieval and Visual Question Answering Under Strong Visual Homogeneity
  - 重要性：P0
  - 为什么值得看：针对企业真实文档库中“模板高度相似”的检索难题，提醒多模态 RAG 不能只在文档类型差异明显的数据集上验收，需要额外验证同模板召回、重排和字段定位。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.25343v1

### 多模态与生成媒体

- Invoice Haystack: Benchmarking Document Retrieval and Visual Question Answering Under Strong Visual Homogeneity
  - 重要性：P0
  - 为什么值得看：从 VLM 单文档 VQA 扩展到大规模相似文档集合，适合用来检查视觉文档理解系统是否在真实企业票据场景中退化。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.25343v1

- TriViewBench: Controlled Complexity Scaling for Multi-View Structural Reasoning in MLLMs
  - 重要性：P1
  - 为什么值得看：用合成 3D 场景显式控制对象数量、遮挡和三视图信息，有助于构建更可解释的 MLLM 空间/结构推理压力测试。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.26029v1

### 评测与基准

- Probabilistic Agents in Deterministic Audits: Evaluating Multi-Agent Systems for Automated Audits Based on the German IT-Grundschutz
  - 重要性：P0
  - 为什么值得看：安全合规审计是高价值但高约束的 Agent 评测场景，可用于观察多智能体系统在标准条款映射、文档核验和审计可追踪性上的工程短板。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.25622v1

- Invoice Haystack: Benchmarking Document Retrieval and Visual Question Answering Under Strong Visual Homogeneity
  - 重要性：P0
  - 为什么值得看：提出高视觉同质性文档集合这一更贴近企业场景的评测维度，能补足传统多文档 benchmark 对 embedding 空间可分性的乐观假设。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.25343v1

- TriViewBench: Controlled Complexity Scaling for Multi-View Structural Reasoning in MLLMs
  - 重要性：P1
  - 为什么值得看：提供按复杂度分级的多视角结构推理评测思路，便于工程团队观察模型在对象数和遮挡增加时的能力边界。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.26029v1

### 推理、训练与后训练

- TriViewBench: Controlled Complexity Scaling for Multi-View Structural Reasoning in MLLMs
  - 重要性：P1
  - 为什么值得看：复杂度可控的多视图结构 QA 可作为多模态推理训练/后训练数据设计参考，但真实场景迁移效果仍需验证。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.26029v1

### 推理系统与工程工具

- Probabilistic Agents in Deterministic Audits: Evaluating Multi-Agent Systems for Automated Audits Based on the German IT-Grundschutz
  - 重要性：P0
  - 为什么值得看：自动化审计系统需要把概率式 LLM Agent 包进确定性流程、日志和复核机制中，对工程化编排、权限控制和审计日志设计有参考价值。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.25622v1

### 数据集与数据工程

- Invoice Haystack: Benchmarking Document Retrieval and Visual Question Answering Under Strong Visual Homogeneity
  - 重要性：P0
  - 为什么值得看：提示企业文档数据集构造要覆盖“同模板、高相似、字段级差异”样本，否则评测集可能无法暴露生产环境最常见的误召回问题。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.25343v1
