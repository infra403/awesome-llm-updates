## 2026-06-23 09:13 北京时间 | 论文巡检

**巡检摘要**：本次候选 8 篇，入选 8 篇；P0/P1 共 5 篇。整体以 LLM Agent 在垂直任务、交互式规则学习与多智能体临床/工程应用为主；未发现严格意义上的 P0 新模型发布或系统级突破，因此本轮最高定为 P1。

### P1｜Generator-Assistant Stepwise Rollback Framework for Large Language Model Agent

- **来源**：Semantic Scholar；Conference on Empirical Methods in Natural Language Processing；citations=7
- **发布日期**：2025-03-04
- **重要性**：P1
- **主题标签**：Agent 与多智能体；推理、训练与后训练；评测与基准
- **一句话结论**：GA-Rollback 用“生成器执行 + 助手逐步检查/回滚”的方式缓解 agent 轨迹中错误思考被一路继承的问题。
- **为什么值得看**：候选摘要明确指出它针对 step-by-step agent 的 one-pass error propagation，在每一步动作后引入检查与回滚；这正是工具调用 agent、浏览器 agent、代码 agent 常见的失败模式。
- **工程启发**：生产 agent 不应只保存线性 scratchpad，可把关键动作设计成可验证、可撤销的事务；在工具调用前后插入轻量 critic/assistant，将“继续执行”改成“执行—审计—必要时回滚”。
- **原文 URL**：https://www.semanticscholar.org/paper/743694e2defb4cd81d155e26b04c0fc4a024a9eb

### P1｜IDEA: Enhancing the Rule Learning Ability of Large Language Model Agent through Induction, Deduction, and Abduction

- **来源**：Semantic Scholar；Annual Meeting of the Association for Computational Linguistics；citations=20
- **发布日期**：2024-08-19
- **重要性**：P1
- **主题标签**：Agent 与多智能体；推理、训练与后训练；评测与基准
- **一句话结论**：IDEA 将归纳、演绎、溯因组合起来增强 agent 在交互环境中的规则学习能力，并配套 RULEARN benchmark。
- **为什么值得看**：相比静态问答推理，它聚焦 agent 通过交互收集观察、形成假设并解题，贴近真实工具环境中的“先探索、再固化规则”。
- **工程启发**：可把长期任务 agent 的状态机拆成“观察收集—假设生成—假设验证—规则修订”，并把规则学习结果沉淀为可复用 memory/skill，而不是每次从零规划。
- **原文 URL**：https://www.semanticscholar.org/paper/0288769cd4d7777441449b9d379eea08fcc58dd7

### P1｜ClinicalAgent: Clinical Trial Multi-Agent System with Large Language Model-based Reasoning

- **来源**：Semantic Scholar；ACM International Conference on Bioinformatics, Computational Biology and Biomedicine；citations=44
- **发布日期**：2024-04-23
- **重要性**：P1
- **主题标签**：Agent 与多智能体；RAG 与知识工程；产品与商业化
- **一句话结论**：ClinicalAgent 将 GPT-4、多智能体、Least-to-Most 与 ReAct 结合，用于临床试验相关任务并接入外部临床工具/知识。
- **为什么值得看**：临床试验是强知识、强合规、强工具链场景；候选摘要强调问题在于外部知识可及性，多智能体架构用于提升临床上下文中的可用性。
- **工程启发**：垂直行业 agent 的关键不是“单模型更强”，而是知识源、预测工具、推理分解和角色边界的集成；医疗/合规场景尤其需要把数据来源和工具调用链记录清楚。
- **原文 URL**：https://www.semanticscholar.org/paper/e0aab37c1b584e6b0c773dd9e52863106824f1c7

### P1｜Large Language Model Agent for Modular Task Execution in Drug Discovery

- **来源**：Semantic Scholar；bioRxiv；citations=12
- **发布日期**：2025-06-26
- **重要性**：P1
- **主题标签**：Agent 与多智能体；RAG 与知识工程；数据集与数据工程
- **一句话结论**：该工作把 LLM 推理与生物医药专用工具组合，覆盖检索、问答、分子生成、性质预测、分子优化和 3D 蛋白-配体结构生成等早期药物发现环节。
- **为什么值得看**：它展示了 agent 在药物发现管线中的模块化任务编排方式，候选摘要还给出 BCL-2/淋巴细胞白血病案例，属于高价值垂直工程落地范式。
- **工程启发**：复杂科研 agent 应按“数据检索—结构化表示—候选生成—性质评估—迭代优化—结果溯源”拆模块；每个模块尽量绑定确定性工具，LLM 负责路由、解释和异常恢复。
- **原文 URL**：https://www.semanticscholar.org/paper/0a63c9327d443b172bb4f755bae7dece52a6aa5c

### P1｜OR-LLM-Agent: Automating Modeling and Solving of Operations Research Optimization Problem with Reasoning Large Language Model

- **来源**：Semantic Scholar；arXiv.org；citations=24
- **发布日期**：2025
- **重要性**：P1
- **主题标签**：Agent 与多智能体；推理系统与工程工具；推理、训练与后训练
- **一句话结论**：OR-LLM-Agent 面向运筹优化问题，尝试自动完成建模与求解流程。
- **为什么值得看**：虽然候选缺少摘要细节，但题名和来源显示它针对“自然语言问题到优化模型/求解器”的工程断点；对排产、路由、资源分配类 LLM 应用很有参考价值。
- **工程启发**：LLM 适合承担优化问题的需求解析、变量/约束草拟和求解器调用封装，但生产中必须加入模型校验、约束单元测试和求解结果可解释性检查。
- **原文 URL**：https://www.semanticscholar.org/paper/0d38227805325c625c72defba576d62d19e2bfc6

### P2｜AirVista: Empowering UAVs with 3D Spatial Reasoning Abilities Through a Multimodal Large Language Model Agent

- **来源**：Semantic Scholar；2024 IEEE 27th International Conference on Intelligent Transportation Systems (ITSC)；citations=10
- **发布日期**：2024-09-24
- **重要性**：P2
- **主题标签**：多模态与生成媒体；Agent 与多智能体；推理、训练与后训练
- **一句话结论**：AirVista 将多模态大模型 agent 用于城市空中无人机框架，强调细粒度 3D 空间感知与推理。
- **为什么值得看**：对机器人/无人机类 embodied agent 有参考意义，尤其是把 MLLM 接入 ACP 框架和空间推理任务。
- **工程启发**：多模态 agent 若进入物理世界，需要把视觉/空间状态、任务规划和安全约束分层；LLM/MLLM 只应处理高层语义和推理，低层控制需由稳定模块接管。
- **原文 URL**：https://www.semanticscholar.org/paper/7f797106e8b3d8d9300aaed917bd0686a1fc8caa

### P2｜Large Language Model Agent as a Mechanical Designer

- **来源**：Semantic Scholar；Journal of engineering design；citations=34
- **发布日期**：2024-04-26
- **重要性**：P2
- **主题标签**：Agent 与多智能体；推理系统与工程工具；产品与商业化
- **一句话结论**：该工作把预训练 LLM 与 FEM 有限元模块结合，自动生成、评估并迭代结构设计。
- **为什么值得看**：它是“LLM + 专业仿真器”闭环设计的代表案例，适合关注 CAD/CAE、工业设计自动化的工程团队。
- **工程启发**：LLM 生成设计方案后必须进入数值仿真闭环；工程设计 agent 的价值来自自动迭代和指标约束，而不是一次性文本方案。
- **原文 URL**：https://www.semanticscholar.org/paper/2174286ae1e3fa3537b8cfa602173f8d6222c225

### P2｜Evaluation of Different Large Language Model Agent Frameworks for Design Engineering Tasks

- **来源**：Semantic Scholar；Proceedings of NordDesign 2024；citations=9
- **发布日期**：2024
- **重要性**：P2
- **主题标签**：评测与基准；Agent 与多智能体；推理系统与工程工具
- **一句话结论**：该论文比较了不同 LLM agent/多 agent 推理框架在工程设计任务中的表现，并用 LangChain 实现实验。
- **为什么值得看**：增量不如新框架论文，但它对“agent 框架是否真的提升工程任务质量”这个落地问题有直接参考价值。
- **工程启发**：选 LangChain/多 agent/单 agent 框架前，应先定义工程任务的质量评价和所有权边界；不要只以 agent 数量或框架复杂度作为架构升级理由。
- **原文 URL**：https://www.semanticscholar.org/paper/b41cf21fd55d3ba5ae951c114d4cd8736b60458a
