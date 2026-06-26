## 2026-06-26 21:36 每日主题观察

### Agent
- **方向**：Agent 评测从“最终答案”转向“过程可监督、路径可审计”。
- **核心变化**：OpenRCA 2.0/PAVE 候选强调 root cause propagation path 的逐步标签；GitHub 侧 Dify、Neo.mjs、OpenLoomi 显示 Agentic workflow、memory、MCP、多 Agent 编排继续活跃。
- **工程影响**：AIOps Agent、终端 Agent、工作流 Agent 需要记录工具调用、因果链和失败传播路径，方便回放与评分。
- **建议动作**：今天应阅读 OpenRCA 2.0；持续观察 Dify/Neo.mjs/OpenLoomi 具体 release/commit。详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd

### RAG
- **方向**：RAG 的核心风险从“检索不到”扩展到“检索到过期/冲突事实”。
- **核心变化**：Temporal Validity 指出 embedding 相似度难以区分 contradicted fact 和 duplicated fact，候选摘要给出 AUROC 0.59。
- **工程影响**：知识库需要时间有效性、版本、来源优先级和冲突处理策略；代码/API RAG 尤其容易受旧事实影响。
- **建议动作**：今天应阅读，并审计现有 RAG 的 stale-fact 测试集。来源：https://arxiv.org/abs/2606.26511v1

### 安全
- **方向**：Agentic RAG 红队覆盖面扩大。
- **核心变化**：MIRROR 候选覆盖 text poisoning、image injection、direct-query attacks、orchestrator-level tool manipulation，并用 novelty-constrained memory-guided MCTS 减少攻击样本重复。
- **工程影响**：安全评测应覆盖检索、输入模态、工具编排和 orchestrator，而非只测 prompt injection。
- **建议动作**：今天应阅读，抽取攻击面 taxonomy 做内部 checklist。来源：https://arxiv.org/abs/2606.26793v1

### 模型发布
- **方向**：Agent/world-model/多模态模型的 GGUF 量化候选增加。
- **核心变化**：FreedomAISVR 更新 Qwen-AgentWorld-35B-A3B NVFP4 与 MXFP4-MOE GGUF 分支；LFM2.5 8B A1B 出现 RLVR/GRPO adapter 候选。
- **工程影响**：本地/边缘 Agent 原型可更快试验，但必须验证量化精度、多模态链路、模型卡和许可证。
- **建议动作**：今天应实验 Qwen-AgentWorld 的最小 smoke test；持续观察 LFM2.5 adapters。详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd

### 推理 / LLM Infra
- **方向**：短期推理服务启动继续低门槛化。
- **核心变化**：HF Blog 发布一行命令在 HF Jobs 上跑 vLLM server。
- **工程影响**：临时 benchmark、demo、模型 smoke test 的环境准备成本下降；生产仍需另行评估 SLA、配额、冷启动、监控与成本。
- **建议动作**：今天应实验一个非敏感小模型的 OpenAI-compatible endpoint。来源：https://huggingface.co/blog/vllm-jobs

### 评测
- **方向**：过程监督、时间有效性和攻击新颖性成为新 eval 维度。
- **核心变化**：OpenRCA 2.0、Temporal Validity、MIRROR 分别对应因果路径、过期事实、红队样本重复度。
- **工程影响**：内部 eval harness 应增加 trace/path scoring、temporal conflict cases、cross-surface attack suites。
- **建议动作**：今天应阅读三篇论文并拆成可执行测试项。详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd

### 多模态
- **方向**：多模态 Agent 的能力与攻击面同步扩大。
- **核心变化**：Qwen-AgentWorld 候选含 vision/multimodal 标签；MIRROR 将 image injection 纳入 Agentic RAG 攻击面。
- **工程影响**：多模态输入不能只做内容安全过滤，还要考虑检索污染和工具调用误导。
- **建议动作**：持续观察，等模型卡和复现实验更完整后再扩大实验。详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd

### 开源项目
- **方向**：Agent/RAG 平台围绕 workflow、MCP、memory、GraphRAG 集成。
- **核心变化**：Dify、RAGFlow、Neo.mjs、OpenLoomi 在当前窗口有高质量候选。
- **工程影响**：平台选型应看上下文工程、权限、安全、评测、可观测性，而不是只看 stars 或一次更新时间。
- **建议动作**：持续观察，建立对比矩阵，不立即迁移。来源：https://github.com/langgenius/dify ，https://github.com/infiniflow/ragflow ，https://github.com/neomjs/neo ，https://github.com/melandlabs/openloomi
