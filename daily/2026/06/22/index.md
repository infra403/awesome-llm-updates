---
type: DailyRadar
date: "2026-06-22"
language: zh-CN
audience: "中文 LLM / Agent 工程师"
tags: [agents, evals, inference, llm-infra, model-releases, papers, rag, safety]
source: "../../../../archive/2026/06/22/digest/20260622-224238/daily.md"
---

# 2026-06-22 LLM 工程情报 Radar

> 面向中文 LLM / Agent 工程师，优先关注模型、Agent、RAG、评测、安全、推理和基础设施的工程价值。

## 快速入口

- [项目首页](../../../../README.md)
- [主题索引](../../../../topics/README.md)
- [原始归档](../../../../archive/2026/06/22/README.md)

## 2026-06-22 22:42 北京时间 | 每日大模型情报

### 今日最重要的 6 条

1. **OpenAI 将“上线前部署仿真”作为评测方向推到台前**：2026-06-16 发布的 Deployment Simulation 用真实会话数据模拟部署场景，在模型发布前预测行为与安全风险。这对工程团队的含义是：eval 不应只停留在静态题库，应加入匿名化真实流量回放、场景分层和工具调用回归。来源：https://openai.com/index/deployment-simulation
2. **OpenAI frontier models 与 Codex 已在 AWS 一般可用**：2026-06-01 发布，意味着 AWS 标准化企业的采购、权限、网络边界、审计流程可能更容易接入 OpenAI/Codex。需要重新比较直连 OpenAI API 与 AWS 路径在模型可用性、延迟、日志、权限和成本上的差异。来源：https://openai.com/index/openai-frontier-models-and-codex-are-now-available-on-aws
3. **Coding Agent 继续向“持久、安全、企业化环境”演进**：OpenAI 2026-06-11 宣布计划收购 Ona，用于扩展 Codex 的安全持久云环境；另有 Codex 安全运行文章强调 sandbox、approvals、network policies、agent-native telemetry。这说明代码 Agent 的竞争焦点从单次补全转向任务续跑、隔离、审批与可观测。来源：https://openai.com/index/openai-to-acquire-ona ，https://openai.com/index/running-codex-safely
4. **Agent/RAG 的上下文管理与流式工具调用开始被拆解为可工程化机制**：2026-06-18 arXiv 论文 PACMS 将 Agent 上下文选择建模为可插拔 submodular selection；Streaming RAG 论文指出只有当 tool intent 在用户输入结束前已稳定时，提前检索才有收益。来源：https://arxiv.org/abs/2606.20047v1 ，https://arxiv.org/abs/2606.20113v1
5. **端侧/实时 Agent Serving 需要超越 KV cache 的状态复用**：2026-06-18 arXiv 的 Execution-State Capsules 将复用对象扩展到图绑定执行状态 checkpoint/restore，面向低延迟、小 batch、端侧物理 AI 的分支、重置、中断和重入场景。来源：https://arxiv.org/abs/2606.20537v1
6. **评测从单轮题库继续走向部署仿真、多轮红队、多语言和领域专家任务**：LifeSciBench 面向生命科学专家任务；Multi-LCB 扩展 LiveCodeBench 到多语言；NRT-Bench 用模拟核电站控制室测试安全关键 Agent 的多轮对抗鲁棒性。来源：https://openai.com/index/introducing-life-sci-bench ，https://arxiv.org/abs/2606.20517v1 ，https://arxiv.org/abs/2606.20408v1

### 按时间顺序的今日时间线

- **2026-05-08**：OpenAI 发布 Running Codex safely at OpenAI，描述 Codex 的 sandboxing、approvals、network policies 与 agent-native telemetry。来源：https://openai.com/index/running-codex-safely
- **2026-05-12**：OpenAI 发布 Parameter Golf 复盘，展示 AI-assisted ML research、coding agents、quantization 与受约束模型设计的竞赛式探索。来源：https://openai.com/index/what-parameter-golf-taught-us
- **2026-05-15**：Databricks 将 GPT-5.5 用于 enterprise agent workflows，并提到 OfficeQA Pro benchmark SOTA。来源：https://openai.com/index/databricks
- **2026-05-18**：OpenAI 与 Dell 合作，将 Codex 带到 hybrid/on-premise 企业环境。来源：https://openai.com/index/dell-codex-enterprise-partnership
- **2026-06-01**：OpenAI frontier models 和 Codex 在 AWS 上一般可用。来源：https://openai.com/index/openai-frontier-models-and-codex-are-now-available-on-aws
- **2026-06-03**：OpenAI 介绍 GPT-Rosalind 新能力，覆盖 biological reasoning、medicinal chemistry、genomics analysis 与 experimental workflow。来源：https://openai.com/index/introducing-new-capabilities-to-gpt-rosalind
- **2026-06-11**：OpenAI 宣布计划收购 Ona，用于扩展 Codex 的安全持久云环境和长期运行 AI agents。来源：https://openai.com/index/openai-to-acquire-ona
- **2026-06-16**：OpenAI 发布 Deployment Simulation，用真实会话数据模拟部署场景，在上线前预测模型行为。来源：https://openai.com/index/deployment-simulation
- **2026-06-17**：OpenAI 发布 LifeSciBench，用专家编写与评审任务评估生命科学研究决策能力。来源：https://openai.com/index/introducing-life-sci-bench
- **2026-06-18**：论文侧集中出现 Agent/RAG/Serving/Eval 工程机制：Execution-State Capsules、Probe-and-Refine 仓库指导、Streaming RAG tool-intent stabilization、PACMS、Multi-LCB、NRT-Bench、AutoPass、Contagion Networks。来源：https://arxiv.org/abs/2606.20537v1 ，https://arxiv.org/abs/2606.20512v1 ，https://arxiv.org/abs/2606.20113v1 ，https://arxiv.org/abs/2606.20047v1 ，https://arxiv.org/abs/2606.20517v1 ，https://arxiv.org/abs/2606.20408v1 ，https://arxiv.org/abs/2606.20373v1 ，https://arxiv.org/abs/2606.20493v1
- **2026-06-18**：OpenAI 报道 reasoning model 帮助医生诊断儿童罕见遗传病，在此前未解决病例中识别 18 个新诊断；应视为专家辅助和证据链场景，不应无监督产品化。来源：https://openai.com/index/diagnose-rare-childhood-diseases

### 按主题分组的重点

#### 模型
- GPT-5.5 出现在企业 agent workflow 与 OfficeQA Pro 场景中，说明企业办公任务 benchmark 正在影响模型选型。来源：https://openai.com/index/databricks
- GPT-Rosalind 强化生命科学能力，提示垂直科学模型会与“通用模型 + RAG + 工具链”竞争。来源：https://openai.com/index/introducing-new-capabilities-to-gpt-rosalind
- 固定模型发布文档本次没有新增模型卡/开源权重条目；相关结论仅来自新闻博客入口，模型参数、上下文、许可证与权重状态待后续确认。

#### Agent/RAG
- OpenAI 收购 Ona 与 Codex 安全运行实践共同指向：持久 workspace、凭据隔离、审批链、可恢复任务和遥测会成为 coding agent 基线能力。来源：https://openai.com/index/openai-to-acquire-ona ，https://openai.com/index/running-codex-safely
- Probe-and-Refine 论文把 AGENTS.md/仓库指导从静态 README 变成可测试、可迭代的操作性知识。来源：https://arxiv.org/abs/2606.20512v1
- PACMS 与 Streaming RAG 论文提示：Agent 上下文预算和流式检索触发都需要显式策略，而不是固定 token 截断或盲目提前检索。来源：https://arxiv.org/abs/2606.20047v1 ，https://arxiv.org/abs/2606.20113v1

#### 推理与训练
- Execution-State Capsules 说明端侧/实时 Agent 的 serving 优化不能只看 prefix/KV cache，要考虑图绑定执行状态的 checkpoint/restore。来源：https://arxiv.org/abs/2606.20537v1
- Parameter Golf 展示“人类设约束 + agent 搜索设计空间”的 AI-assisted research 模式，对量化、小模型和架构实验有启发。来源：https://openai.com/index/what-parameter-golf-taught-us
- AutoPass 代表 Agent 进入性能工程闭环：读取 compiler/runtime 证据、提出优化、运行测量、迭代决策。来源：https://arxiv.org/abs/2606.20373v1

#### 多模态
- 今日固定输入中没有可确认的新多模态模型/产品发布；与物理 AI、实时语音/机器人相关的启发主要来自 Execution-State Capsules 的端侧低延迟 serving 设定。来源：https://arxiv.org/abs/2606.20537v1

#### 评测
- Deployment Simulation 是 P0：把真实会话回放引入模型上线前评估。来源：https://openai.com/index/deployment-simulation
- LifeSciBench 强调专家任务与决策质量，适合垂直领域 eval 设计参考。来源：https://openai.com/index/introducing-life-sci-bench
- Multi-LCB、NRT-Bench、Contagion Networks 分别覆盖多语言代码评测、多轮安全关键红队、多 Agent 评价者偏差传播。来源：https://arxiv.org/abs/2606.20517v1 ，https://arxiv.org/abs/2606.20408v1 ，https://arxiv.org/abs/2606.20493v1

#### 工程工具
- OpenAI/Codex on AWS 会影响企业模型接入路径、网络边界、审计与采购流程。来源：https://openai.com/index/openai-frontier-models-and-codex-are-now-available-on-aws
- Dell + Codex 的 hybrid/on-premise 方向值得有内网代码库、数据驻留和合规要求的团队跟踪。来源：https://openai.com/index/dell-codex-enterprise-partnership
- GitHub 固定入口本次没有新增项目巡检内容；开源工具趋势需在下一轮补充。

#### 产品商业化
- OpenAI 在 AWS、Dell、Databricks 三条企业路线同时出现：云市场、混合/本地部署、企业知识工作流。这说明企业 Agent 落地更看重采购与合规路径，而不仅是模型能力。来源：https://openai.com/index/openai-frontier-models-and-codex-are-now-available-on-aws ，https://openai.com/index/dell-codex-enterprise-partnership ，https://openai.com/index/databricks

#### 数据
- Deployment Simulation 需要真实 conversation data 的匿名化、分层与回放；这会把数据治理纳入 eval 基础设施。来源：https://openai.com/index/deployment-simulation
- GPT-Rosalind 和 LifeSciBench 都显示垂直领域数据/专家评审正在成为科学 AI 系统的核心壁垒。来源：https://openai.com/index/introducing-new-capabilities-to-gpt-rosalind ，https://openai.com/index/introducing-life-sci-bench

### 对 LLM 工程师的行动建议

**今天应阅读**
- P0：OpenAI Deployment Simulation，重点看如何把真实会话回放引入上线前准入。https://openai.com/index/deployment-simulation
- P0：Running Codex safely at OpenAI，作为 coding agent 权限、网络、审批和遥测检查清单。https://openai.com/index/running-codex-safely
- P1：PACMS 与 Streaming RAG，两篇合看，用于改造 Agent context budget manager 与流式检索触发策略。https://arxiv.org/abs/2606.20047v1 ，https://arxiv.org/abs/2606.20113v1

**今天应实验**
- 为一个核心产品流程建立 50-200 条匿名化真实会话回放集，记录安全、拒答、工具调用、事实一致性和延迟指标。
- 在一个 coding agent 仓库中试行 Probe-and-Refine：先用失败任务探测 AGENTS.md 缺口，再改写指导，并用回归任务验证是否提升通过率。来源：https://arxiv.org/abs/2606.20512v1
- 对 RAG/Agent 请求离线标注“工具意图稳定点”，比较提前检索、输入结束后检索、混合策略的延迟/成本/错误上下文比例。

**应持续观察**
- OpenAI on AWS 与 Dell hybrid/on-prem Codex 的模型范围、数据边界、日志策略、价格与延迟。
- 多轮 Agent 安全评测是否会从研究 benchmark 进入企业准入流程，尤其是具备工具调用和系统操作权限的 Agent。
- 模型发布与 GitHub 项目入口本轮无新增有效条目，下一轮需补齐开源权重、推理框架、评测工具和工程项目趋势。

### 固定入口

- 论文追踪：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
- 新闻博客追踪：https://my.feishu.cn/docx/P16idvuAgo3u8ixAacXcmfXSn6R
- 模型发布追踪：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb
- GitHub 项目追踪：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g
- 时间索引：https://my.feishu.cn/docx/QZjEdsjnRoDVGixlJTOcjx3Dn8b
- 主题索引：https://my.feishu.cn/docx/OeMPdOXCSoG6JDxWU3qc5fcRn1c

## 原始归档

- [当日 archive index](../../../../archive/2026/06/22/README.md)
