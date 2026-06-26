## 2026-06-26 21:17 北京时间 | 论文巡检

摘要：本次候选 18 篇；入选 8 篇；P0/P1 入选 8 篇（P0：8，P1：0）。筛选优先级依据候选中的 `priority_hint=P0/P1`、工程相关 `reason_codes`、证据完整性与时间窗口；全部入选论文发布日期均为 2026-06-25，处于本次 36h 窗口内。

### 1. OpenRCA 2.0: From Outcome Labels to Causal Process Supervision

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：Agent 与多智能体；评测与基准；RAG 与知识工程
- 核心变化：论文把 Root Cause Analysis（RCA）从“只标最终根因”的 outcome label，推进到对故障传播路径做 step-wise process supervision，并引入 PAVE 标注协议，目标是减少模型靠模式匹配猜根因的空间。
- 一句话结论：如果团队在做 Agent 运维、RAG 排障或工具调用链评测，这篇的关键价值是把“答对根因”拆成“能否解释和追踪传播过程”。
- 工程影响：可启发 Agent 评测从 final answer scoring 升级为过程级 trace scoring；对 SRE Copilot、日志/指标/trace 联合 RCA、长上下文工具调用 Agent 都有直接参考价值，尤其适合作为内部 eval schema 的设计样板。
- 证据边界：当前仅基于 arXiv 摘要与候选元数据；作者、完整数据规模、开放代码、模型对比结果和具体指标未在候选中确认，不能据此判断可复现实验成熟度。
- 建议动作：今天应阅读。理由：RCA 是 Agent 工程落地中的高价值场景，过程监督的评测粒度比普通根因标签更接近真实排障需求。
- 原文 URL：https://arxiv.org/abs/2606.27154v1

### 2. MIRROR: Novelty-Constrained Memory-Guided MCTS Red-Teaming for Agentic RAG

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：RAG 与知识工程；Agent 与多智能体；评测与基准；多模态与生成媒体
- 核心变化：论文面向 multimodal agentic RAG 的跨表面攻击面，提出 memory-guided Monte Carlo Tree Search red-teaming，并强调 novelty constraint，用来避免红队样本大量复用已知攻击模板；候选摘要指出其观察到文本投毒 benchmark 中有 73–84% exact duplication。
- 一句话结论：这篇把 Agentic RAG 安全评测从单一 prompt injection 扩展到文本投毒、图像注入、直接查询攻击和编排器级工具操纵。
- 工程影响：对有工具编排、向量库、图像/网页输入和长期记忆的 RAG Agent，建议把攻击生成器设计成“搜索 + 记忆 + 去重”的闭环，而不是手写模板集；也提示安全回归集需要检查样本新颖性，否则安全分数可能虚高。
- 证据边界：当前仅基于 arXiv 摘要与候选元数据；MCTS 状态空间、攻击成功率、数据集细节、是否开源和跨模态实验完整结果未确认。73–84% duplication 为候选摘要中给出的背景观察，未核验全文方法细节。
- 建议动作：今天应实验。理由：Agentic RAG 的攻击面正在从提示词层变成系统编排层，红队搜索框架可直接转化为内部安全测试任务。
- 原文 URL：https://arxiv.org/abs/2606.26793v1

### 3. Temporal Validity in Retrieval Memory: Eliminating Stale-Fact Errors for AI Agents over Evolving Knowledge

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：RAG 与知识工程；Agent 与多智能体；数据集与数据工程
- 核心变化：论文指出普通 RAG 记忆没有时间模型：当事实发生变化时，过期事实与当前事实在 embedding 相似度上接近，导致 Agent 检索到冲突事实后错误回答或拒答；候选摘要提到在校准数据上 cosine similarity 区分 contradicted fact 与 duplicated fact 的 AUROC 仅 0.59。
- 一句话结论：这篇把“知识过期”定义为 RAG 架构层问题，而不是单纯靠更好 embedding 就能解决的问题。
- 工程影响：对企业知识库、API 文档 Copilot、代码库问答和长期记忆 Agent，应引入时间有效期、版本、supersedes/contradicts 关系、检索后冲突消解，而不只是按相似度 top-k；也适合加入 stale-fact eval，专门测模型是否引用已废弃事实。
- 证据边界：当前仅基于 arXiv 摘要与候选元数据；数据集构造、消除 stale-fact 的具体算法、完整指标和开源状态未确认。AUROC 0.59 为候选摘要中给出的单项观察，需读全文核验。
- 建议动作：今天应实验。理由：几乎所有生产 RAG 都会遇到文档版本变化，时间有效性比常规召回率更贴近线上故障。
- 原文 URL：https://arxiv.org/abs/2606.26511v1

### 4. A hardware-safety-gated system for LLM-written native ARTIQ control code on a trapped-ion platform

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：论文将 LLM Agent 放进 trapped-ion 实验控制环路，让其编写并运行 native ARTIQ 控制代码，同时通过 hardware-safety gate 在每个操作边界上区分人类授权/监督与 Agent 决策，避免 unchecked code 损坏设备。
- 一句话结论：这篇的泛化意义不在量子实验本身，而在“LLM 写代码并操作真实设备”时如何设置硬安全边界。
- 工程影响：对机器人、实验自动化、IoT、DevOps 自动变更和生产控制系统，提示不能只依赖 prompt/策略文本约束 Agent；需要把安全约束下沉为可执行 gate、权限边界、操作级审计和人工授权点。
- 证据边界：当前仅基于 arXiv 摘要与候选元数据；硬件 gate 的形式化模型、失败案例、延迟/吞吐开销、代码与系统实现细节未确认。
- 建议动作：今天应阅读。理由：LLM Agent 从生成文本走向执行代码和控制物理/生产系统时，安全边界是工程上线前的硬门槛。
- 原文 URL：https://arxiv.org/abs/2606.27231v1

### 5. When Does Combining Language Models Help? A Co-Failure Ceiling on Routing, Voting, and Mixture-of-Agents Across 67 Frontier Models

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：Agent 与多智能体；模型发布与模型能力；评测与基准
- 核心变化：论文提出多模型系统的收益上限由 co-failure rate β 约束：对于输出只能选某个成员模型答案的策略，准确率上限不能超过 1−β；并指出常用的平均 pairwise error correlation ρ 无法识别这种共同失败结构。
- 一句话结论：这篇给模型路由、投票、cascade、fusion 和 mixture-of-agents 提供了一个比“模型多样性直觉”更硬的上限诊断。
- 工程影响：构建多模型 Agent 或路由系统时，不应只比较单模型分数和 pairwise 相关性，还要测 query-level all-wrong 集合；如果 β 高，再复杂的 routing/voting 也很难突破天花板，资源应转向数据/工具/检索/验证器而不是堆更多模型。
- 证据边界：当前仅基于 arXiv 摘要与候选元数据；67 个 frontier models 的名单、任务集、β 的估计方法和是否覆盖生成式自由回答未确认。
- 建议动作：今天应阅读。理由：多模型组合是常见提效路线，co-failure ceiling 可直接改变路由评测报表和实验设计。
- 原文 URL：https://arxiv.org/abs/2606.27288v1

### 6. Agents That Know Too Much: A Data-Centric Survey of Privacy in LLM Agents

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：Agent 与多智能体；数据集与数据工程；产品与商业化
- 核心变化：论文从 data-centric 视角综述 LLM Agent 隐私风险，关注 Agent 会查询数据库、检索文档、调用 API、保留跨会话状态并以委托权限行动，因此泄漏不只发生在最终回答，也可能出现在查询、工具调用、记忆和工作流中。
- 一句话结论：这篇适合作为 Agent 隐私威胁建模清单，而不是单点防 prompt leakage 的论文。
- 工程影响：Agent 平台需要把隐私控制覆盖到数据源权限、检索 query、tool arguments、scratchpad/trace、长期记忆、日志与审计，而不是只在最终输出做 DLP；对企业 Agent、个人助理和多租户工作流尤其重要。
- 证据边界：这是 survey；当前仅基于 arXiv 摘要与候选元数据，未确认其分类法完整性、引用范围和具体防护方案可操作性。
- 建议动作：持续观察。理由：survey 不一定立刻给出新算法，但可用来补齐 Agent 平台隐私 checklist。
- 原文 URL：https://arxiv.org/abs/2606.26627v1

### 7. Resource-Aware Neuro-Symbolic Reasoning for Local Small Language Models

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：推理、训练与后训练；推理系统与工程工具；模型发布与模型能力
- 核心变化：论文研究本地 small language model 的资源受限推理：模型先把问题翻译为 typed finite-domain rules/constraints，符号层检查 traceability 和 consistency，再由确定性 solver 完成推理；候选摘要称该流程为 Verifiable Formalization and Repair（VFR-LLM）。
- 一句话结论：这篇给本地小模型提供了“用符号求解器换采样预算”的路线。
- 工程影响：对端侧 Agent、离线 Copilot、低成本推理服务，可以考虑把部分结构化推理任务改造成 formalization + solver + repair，而不是依赖多次采样或升级大模型；同时也便于输出可验证 trace，降低幻觉风险。
- 证据边界：当前仅基于 arXiv 摘要与候选元数据；支持的任务类型、solver 选择、失败模式、延迟成本和与大模型/多采样的完整对比未确认。
- 建议动作：持续观察。理由：方向有工程吸引力，但需要确认任务覆盖和形式化失败率后再投入实验。
- 原文 URL：https://arxiv.org/abs/2606.27281v1

### 8. CHIA: An open-source framework for principled, agentic AI-driven hardware/software co-design research

- 来源：arXiv
- 发布日期：2026-06-25
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：论文介绍 CHIA，一个面向硬件/软件协同设计研究的开源 Agentic AI 框架，目标是把计算机体系结构、系统、编译器、VLSI 等领域中零散的小规模 AI workflow，组织成可设计、可部署的复杂 AI-infused 工作流。
- 一句话结论：这篇值得关注的是 Agentic workflow 在硬件/系统研发中的框架化，而不是单个设计任务的 demo。
- 工程影响：对自动化性能调优、编译器探索、系统设计空间搜索和 EDA workflow，CHIA 可能提供如何编排 Agent、工具、评测和人类监督的参考；也可作为观察“Agent 工程平台如何服务专业研发流程”的案例。
- 证据边界：当前仅基于 arXiv 摘要与候选元数据；虽然标题称 open-source，但仓库地址、许可证、可运行性、支持任务和实验规模未在候选中确认。
- 建议动作：持续观察。理由：若代码和案例成熟，会成为专业研发 Agent workflow 的可复用参考；但需先核验开源质量。
- 原文 URL：https://arxiv.org/abs/2606.27350v1
