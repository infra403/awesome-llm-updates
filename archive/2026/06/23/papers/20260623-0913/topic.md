## 2026-06-23 09:13 论文主题条目

### Agent 与多智能体

- **Generator-Assistant Stepwise Rollback Framework for Large Language Model Agent**（P1）：针对 agent 单向轨迹中的错误传播，引入生成器执行与助手检查/回滚；值得关注其可验证、可撤销 agent 流程设计。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/743694e2defb4cd81d155e26b04c0fc4a024a9eb
- **IDEA: Enhancing the Rule Learning Ability of Large Language Model Agent through Induction, Deduction, and Abduction**（P1）：聚焦交互式规则学习，把归纳、演绎、溯因组合成 agent 推理框架，并配套 RULEARN benchmark。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0288769cd4d7777441449b9d379eea08fcc58dd7
- **ClinicalAgent: Clinical Trial Multi-Agent System with Large Language Model-based Reasoning**（P1）：将 GPT-4、多智能体、Least-to-Most 与 ReAct 接入临床试验任务，适合参考垂直行业 agent 的知识/工具集成。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/e0aab37c1b584e6b0c773dd9e52863106824f1c7
- **Large Language Model Agent for Modular Task Execution in Drug Discovery**（P1）：覆盖药物发现早期管线的检索、问答、分子生成、性质预测和结构生成，值得关注模块化科研 agent 编排。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0a63c9327d443b172bb4f755bae7dece52a6aa5c
- **OR-LLM-Agent: Automating Modeling and Solving of Operations Research Optimization Problem with Reasoning Large Language Model**（P1）：面向运筹优化自动建模与求解，适合关注 LLM 到优化求解器链路的团队。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0d38227805325c625c72defba576d62d19e2bfc6
- **AirVista: Empowering UAVs with 3D Spatial Reasoning Abilities Through a Multimodal Large Language Model Agent**（P2）：把 MLLM agent 用于 UAV 3D 空间推理，适合作为 embodied/multimodal agent 案例。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/7f797106e8b3d8d9300aaed917bd0686a1fc8caa
- **Large Language Model Agent as a Mechanical Designer**（P2）：把 LLM 和 FEM 仿真模块组成闭环机械设计 agent，适合 CAD/CAE 自动化参考。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/2174286ae1e3fa3537b8cfa602173f8d6222c225
- **Evaluation of Different Large Language Model Agent Frameworks for Design Engineering Tasks**（P2）：比较 agent/多 agent 框架在工程设计任务中的效果，适合框架选型与评测参考。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/b41cf21fd55d3ba5ae951c114d4cd8736b60458a

### 推理、训练与后训练

- **Generator-Assistant Stepwise Rollback Framework for Large Language Model Agent**（P1）：用逐步检查/回滚减少推理轨迹中错误中间思考的不可逆传播。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/743694e2defb4cd81d155e26b04c0fc4a024a9eb
- **IDEA: Enhancing the Rule Learning Ability of Large Language Model Agent through Induction, Deduction, and Abduction**（P1）：把归纳、演绎、溯因放入同一交互推理循环，适合参考长期任务中的规则沉淀。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0288769cd4d7777441449b9d379eea08fcc58dd7
- **OR-LLM-Agent: Automating Modeling and Solving of Operations Research Optimization Problem with Reasoning Large Language Model**（P1）：关注推理模型如何把问题语义转为优化模型和求解流程。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0d38227805325c625c72defba576d62d19e2bfc6
- **AirVista: Empowering UAVs with 3D Spatial Reasoning Abilities Through a Multimodal Large Language Model Agent**（P2）：强调 UAV 任务中的 3D 空间推理能力。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/7f797106e8b3d8d9300aaed917bd0686a1fc8caa

### RAG 与知识工程

- **ClinicalAgent: Clinical Trial Multi-Agent System with Large Language Model-based Reasoning**（P1）：候选摘要强调外部临床知识可及性问题，适合参考医疗知识工具接入。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/e0aab37c1b584e6b0c773dd9e52863106824f1c7
- **Large Language Model Agent for Modular Task Execution in Drug Discovery**（P1）：包含生物医学数据检索、FASTA/SMILES/文献获取和上下文问答，适合参考科研 RAG 管线。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0a63c9327d443b172bb4f755bae7dece52a6aa5c

### 推理系统与工程工具

- **OR-LLM-Agent: Automating Modeling and Solving of Operations Research Optimization Problem with Reasoning Large Language Model**（P1）：可作为“LLM 需求解析 + 优化求解器执行 + 结果校验”的工程工具链参考。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0d38227805325c625c72defba576d62d19e2bfc6
- **Large Language Model Agent as a Mechanical Designer**（P2）：LLM 与 FEM 数值仿真闭环结合，说明工程 agent 应依赖专业验证器。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/2174286ae1e3fa3537b8cfa602173f8d6222c225
- **Evaluation of Different Large Language Model Agent Frameworks for Design Engineering Tasks**（P2）：对 LangChain 等 agent 框架在设计工程任务中的选型有参考意义。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/b41cf21fd55d3ba5ae951c114d4cd8736b60458a

### 多模态与生成媒体

- **AirVista: Empowering UAVs with 3D Spatial Reasoning Abilities Through a Multimodal Large Language Model Agent**（P2）：MLLM agent 用于 UAV 城市空中交通场景，关注细粒度空间感知与推理。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/7f797106e8b3d8d9300aaed917bd0686a1fc8caa

### 评测与基准

- **IDEA: Enhancing the Rule Learning Ability of Large Language Model Agent through Induction, Deduction, and Abduction**（P1）：引入 RULEARN 用于评估交互环境中的规则学习。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0288769cd4d7777441449b9d379eea08fcc58dd7
- **Generator-Assistant Stepwise Rollback Framework for Large Language Model Agent**（P1）：关注 agent 轨迹可靠性，可转化为“每步可验证/可回滚”的评测维度。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/743694e2defb4cd81d155e26b04c0fc4a024a9eb
- **Evaluation of Different Large Language Model Agent Frameworks for Design Engineering Tasks**（P2）：直接比较不同 agent 框架在设计工程任务上的效果。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/b41cf21fd55d3ba5ae951c114d4cd8736b60458a

### 产品与商业化

- **ClinicalAgent: Clinical Trial Multi-Agent System with Large Language Model-based Reasoning**（P1）：临床试验工具化场景明确，适合观察合规垂直 agent 的产品形态。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/e0aab37c1b584e6b0c773dd9e52863106824f1c7
- **Large Language Model Agent as a Mechanical Designer**（P2）：工业设计自动化具备明确商业落点，但必须绑定仿真和专家审查。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/2174286ae1e3fa3537b8cfa602173f8d6222c225

### 数据集与数据工程

- **Large Language Model Agent for Modular Task Execution in Drug Discovery**（P1）：涉及 FASTA、SMILES、文献等多源生物医学数据检索和结构化，适合参考科研数据管线。详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc；原文：https://www.semanticscholar.org/paper/0a63c9327d443b172bb4f755bae7dece52a6aa5c
