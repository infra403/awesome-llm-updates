## 2026-06-23 21:11 论文主题条目

### 推理系统与工程工具

- Concordia: JIT-Compiled Persistent-Kernel Checkpointing for Fault-Tolerant LLM Inference（P0）：如果团队在做长会话 Agent、超长任务或多 GPU serving，这篇值得今天优先看恢复模型和运行时插入点。为什么值得看：把“请求状态”和“GPU 执行上下文”视为一等可恢复对象；设计 SLA 时不只考虑吞吐/延迟，还要度量 GPU/communicator failure 后的恢复粒度、状态一致性和 replay 成本。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.23521v1

### RAG 与知识工程

- When Confidence Takes the Wrong Path: Diagnosing Retrieval-State Lock-In in RAG（P0）：RAG 评测不能只看 answer agreement；需要把检索状态本身纳入不确定性诊断。为什么值得看：增加 retrieval-state logging、query rewrite 多样性、检索集合扰动测试、无检索/错检索对照，以及把“检索证据是否变化”作为置信度特征。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.22728v1
- HAKARI-Bench: A Lightweight Benchmark for Comparing Retrieval Architectures and Efficiency Settings under Unified Conditions（P0）：RAG 选型不应只看大榜单；需要能在本地快速跑的 retrieval efficiency/quality trade-off 基准。为什么值得看：把 embedding 维度、ANN 参数、量化、reranker 延迟统一纳入回归测试，避免只优化 recall 或只优化 latency。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.22778v1

### 评测与基准

- Can LLMs Reliably Self-Report Adversarial Prefills, and How?（P0）：不要把“让模型自报是否被 prompt/prefill 攻击影响”当成可靠安全边界。为什么值得看：prefill/上下文注入检测应放在外部策略、日志审计和输入规范化层，模型自检最多作为弱信号；评测要覆盖 compromised output 后验解释，而非只测拒答率。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.23671v1
- Litmus: Zero-Label, Code-Driven Metric Specification for Evaluating AI Systems（P0）：评测平台应从“堆指标”转向“指标规格即代码”，否则多 Agent/业务任务指标很难解释。为什么值得看：把 eval spec 纳入 CI：每个任务定义输入空间、允许失败、严重失败、聚合方式和审计样例；适合 Agent 工作流、RAG 答案质量和工具调用安全的持续评估。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.23403v1
- The Table Says Otherwise: Testing LLMs with Counterfactual Relational Data（P0）：数据库/BI/RAG 场景必须评测“上下文优先于记忆”的能力，而不只是表格 QA 准确率。为什么值得看：构造反事实回归集，把已知实体属性、价格、库存、权限等字段改写，验证模型是否引用提供表格；可用于检测参数记忆污染和上下文遵循失败。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.23667v1

### Agent 与多智能体

- MAS-PromptBench: When Does Prompt Optimization Improve Multi-Agent LLM Systems?（P0）：多 Agent prompt 优化不能照搬单模型 prompt tuning；需要按角色、拓扑和聚合方式评估。为什么值得看：记录 agent role prompt 的版本、位置和依赖关系，把 prompt 优化当成 workflow-level search；上线前要分离单 Agent 提升和协同结构带来的提升。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.23664v1

### 推理、训练与后训练

- Randomized YaRN Improves Length Generalization for Long-Context Reasoning（P1）：如果自训/继续训练长上下文模型，这篇提供一个比单纯拉长 context 更细的训练变量。为什么值得看：把位置编码随机化、长度 curriculum 和长上下文 reasoning eval 一起设计；对只做推理服务的团队则主要用于判断模型供应商的长上下文声明是否可靠。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc 原文：https://arxiv.org/abs/2606.23687v1
