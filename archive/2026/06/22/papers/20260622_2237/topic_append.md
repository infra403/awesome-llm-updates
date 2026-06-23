## 2026-06-22 22:37 论文主题条目

### Agent 与多智能体

- **Probe-and-Refine Tuning of Repository Guidance for Coding Agents**（P1）
  - 为什么值得看：直接回应 coding agents 使用 AGENTS.md/仓库指导是否有效的工程争议，关注如何通过 probe-and-refine 迭代指导内容。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20512v1
- **PACMS: Submodular Context Selection as a Pluggable Engine for LLM Agents**（P1）
  - 为什么值得看：把对话、持久记忆和工具输出共同竞争上下文窗口的问题抽象成可插拔选择引擎。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20047v1
- **LLM agent safety, multi-turn red-teaming, jailbreak benchmarks, adversarial robustness, safety-critical systems**（P1）
  - 为什么值得看：NRT-Bench 用安全关键系统模拟环境做多轮自适应红队，比单轮 jailbreak 更接近 Agent 部署风险。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20408v1
- **AutoPass: Evidence-Guided LLM Agents for Compiler Performance Tuning**（P2）
  - 为什么值得看：将 LLM Agent 用到编译性能调优，并强调以编译器/运行时证据驱动决策。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20373v1
- **Contagion Networks: Evaluator Bias Propagation in Multi-Agent LLM Systems**（P2）
  - 为什么值得看：关注 LLM evaluator 在多 Agent 交互网络中可能放大和传播系统性偏差。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20493v1

### RAG 与知识工程

- **When Does Streaming Tool Use Help? Characterizing Tool-Intent Stabilization in Streaming Retrieval-Augmented Generation**（P1）
  - 为什么值得看：指出 Streaming RAG 的收益取决于工具意图何时稳定，而不是所有查询都适合提前检索。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20113v1
- **PACMS: Submodular Context Selection as a Pluggable Engine for LLM Agents**（P1）
  - 为什么值得看：为 Agent/RAG 框架中的上下文预算管理提供比 recency truncation 更结构化的思路。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20047v1

### 推理系统与工程工具

- **Execution-State Capsules: Graph-Bound Execution-State Checkpoint and Restore for Low-Latency, Small-Batch, On-Device Physical-AI Serving**（P1）
  - 为什么值得看：面向端侧物理 AI 服务的分支、重置、中断、重入场景，补足只复用 KV cache 的 serving 设计盲区。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20537v1
- **Probe-and-Refine Tuning of Repository Guidance for Coding Agents**（P1）
  - 为什么值得看：仓库级指导是 coding agent 落地的基础设施，论文聚焦如何验证和迭代这些指导。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20512v1
- **When Does Streaming Tool Use Help? Characterizing Tool-Intent Stabilization in Streaming Retrieval-Augmented Generation**（P1）
  - 为什么值得看：给流式工具调用/检索系统一个可测的“何时值得提前调用”判断维度。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20113v1
- **AutoPass: Evidence-Guided LLM Agents for Compiler Performance Tuning**（P2）
  - 为什么值得看：性能工程 Agent 需要证据闭环而不是黑盒猜测，适合关注自动优化工具链的团队跟进。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20373v1

### 评测与基准

- **Multi-LCB: Extending LiveCodeBench to Multiple Programming Languages**（P1）
  - 为什么值得看：污染感知代码生成评测从 Python 扩展到多语言，更贴近企业代码库选型。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20517v1
- **LLM agent safety, multi-turn red-teaming, jailbreak benchmarks, adversarial robustness, safety-critical systems**（P1）
  - 为什么值得看：把 Agent 安全评测从单轮问答推进到持续多轮、状态化、安全关键系统场景。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20408v1
- **Contagion Networks: Evaluator Bias Propagation in Multi-Agent LLM Systems**（P2）
  - 为什么值得看：多 Agent 系统常用 judge/reviewer，评价偏差传播是评测可信度和系统设计都需要处理的问题。
  - 详情链接：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文链接：https://arxiv.org/abs/2606.20493v1
