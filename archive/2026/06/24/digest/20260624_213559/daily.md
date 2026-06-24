## 2026-06-24 21:35 北京时间 | 每日大模型情报

> 本周期信号判断：P0/P1 候选充足，主线集中在 **Agent 工程化（记忆、代码定位、终端工具）**、**RAG 安全/隐私**、**本地 Agentic 小模型/量化模型** 与 **推理芯片供给链**。以下只纳入巡检窗口内新增、带 quality_score / priority_hint / reason_codes / source URL 的条目；GitHub “updated” 条目仅代表本周期内仓库活跃，不等同于新版本发布。

### 今日最重要（P0/P1）

1. **OpenAI 与 Broadcom 发布 LLM 推理芯片 Jalapeño**：核心变化是 OpenAI News 在 2026-06-24 发布定制 AI 推理芯片消息，候选标记为 P1、quality_score=15，reason_codes 包含 `recent_window`、`source_strong`、`engineering_terms=inference,llm`；工程影响在于如果该芯片进入 OpenAI 自有推理栈，后续可能改变大模型服务的成本、吞吐、功耗与供给弹性，对自建推理团队也有供应链和专用 ASIC 方向的参考价值；建议动作：**今天应阅读**，重点看其披露的是架构能力、量产计划还是战略合作边界；证据边界：候选只确认标题、日期、摘要和 OpenAI 来源，未确认具体性能指标、可用时间、价格或外部采购方式；来源：https://openai.com/index/openai-broadcom-jalapeno-inference-chip

2. **Agent-native memory 从“任务成功率黑盒”转向可拆解的数据管理系统评测**：核心变化是 arXiv 2026-06-23 论文 *Are We Ready For An Agent-Native Memory System?* 被标记为 P0、quality_score=18，提出把 Agent 记忆从简单 RAG/检索组件扩展为支持持久存储、检索、更新、合并与生命周期治理的系统，并指出现有评测多用端到端 F1/BLEU 等黑盒指标；工程影响在于长期 Agent、个人助手、企业知识工作流需要单独评测记忆写入、遗忘、冲突合并、时效性和治理，而不能只看最终任务分；建议动作：**今天应阅读**，可抽取其中评测维度加入现有 Agent memory test plan；证据边界：候选摘要未给出完整 benchmark 名称、数据集规模或代码可用性，需读原文确认；来源：https://arxiv.org/abs/2606.24775v1

3. **SHERLOC 把代码修复 Agent 的“定位”从文件检索推进到结构化诊断**：核心变化是 arXiv 2026-06-23 论文 *SHERLOC: Structured Diagnostic Localization for Code Repair Agents* 被标记为 P0、quality_score=18，指出 repo-level coding agent 会把约一半预算花在 fault localization，提出 training-free 的结构化假设探索/诊断定位框架；工程影响在于 coding agent 的成本和成功率瓶颈可能不在编辑器，而在定位阶段是否能产出可执行诊断上下文，适合改造 SWE-bench 类流水线的 pre-edit 阶段；建议动作：**今天应实验**，优先在一个内部 bugfix benchmark 上比较“文件检索 top-k”与“结构化诊断上下文”对修复成功率和 token 成本的影响；证据边界：候选确认论文方向与摘要，未确认开源实现、具体提升幅度和适配哪些模型；来源：https://arxiv.org/abs/2606.24820v1

4. **RAG 安全今天出现两条互补信号：隐私语义重写与知识投毒**：核心变化是两篇 arXiv 2026-06-23 P0 论文同时进入窗口：*Privacy-Preserving RAG via Multi-Agent Semantic Rewriting*（quality_score=18）关注用多 Agent 对检索内容做隐私抽取、语义分析和重构；*Poisoned Playbooks*（quality_score=18）关注知识投毒对 AI security agents 的影响；工程影响在于企业 RAG 不仅要防 prompt 泄密，还要防知识库被污染后误导安全 Agent，检索前清洗、检索后重写、来源可信度和 playbook 变更审计需要作为一套安全链路设计；建议动作：**今天应阅读**，并把“敏感字段语义保真重写”和“知识库投毒回归测试”加入 RAG 安全 checklist；证据边界：候选摘要未确认生产延迟、召回损失、攻击集规模或防御覆盖率；来源：https://arxiv.org/abs/2606.24623v1 ，https://arxiv.org/abs/2606.24402v1

5. **Hugging Face 本周期集中出现 Agentic / terminal / reasoning 小模型与 GGUF 量化候选**：核心变化是模型巡检在 10 小时窗口内发现多个 P0/P1 模型：`osmapi/osmQwopus3.6-27B-Fable-Agentic`（P0，quality_score=19，2026-06-24T11:26:57Z，Apache-2.0，tool/function-calling/reasoning 标签）、`mradermacher/Fabliq-8B-Agent-Reasoning-GGUF`（P0，quality_score=19，2026-06-24T12:48:30Z，GGUF/agentic/tool-use/terminal 标签）、`LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters`（P0，quality_score=18，2026-06-24T13:11:55Z，terminal-agent/RLVR/GRPO/LoRA 标签）；工程影响在于本地/边缘 Agent 原型可用的模型形态继续向 3B/8B/27B、GGUF、LoRA adapter、tool-use 标签聚集，但下载量和 likes 很低，不能直接视为成熟基座；建议动作：**持续观察**，对 8B GGUF 可做 smoke test（工具调用格式、终端任务、上下文遵循），对 27B/adapter 先等 model card、eval 和社区反馈；证据边界：候选确认时间、标签、license、likes/downloads，未确认真实工具调用准确率、benchmark、训练数据或安全评估；来源：https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic ，https://huggingface.co/mradermacher/Fabliq-8B-Agent-Reasoning-GGUF ，https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters

6. **开源 LLM 工程栈继续围绕评测/观测、低代码 Agent workflow、终端 coding agent 活跃更新**：核心变化是 GitHub 8 小时窗口内 P0 仓库包括 `comet-ml/opik`（quality_score=20，updated 2026-06-24T13:34:31Z，19,755 stars，LLM/RAG/agent tracing 与 eval）、`langgenius/dify`（quality_score=20，updated 2026-06-24T13:34:46Z，146,428 stars，agentic workflow / MCP / RAG）、`can1357/oh-my-pi`（quality_score=20，updated 2026-06-24T13:31:31Z，14,444 stars，terminal coding agent、hash-anchored edits、LSP、browser、subagents）；工程影响在于团队 workflow 的核心差异化正从“能调模型 API”转向“可观测、可评测、可编排、可安全编辑代码”；建议动作：**持续观察**，若团队正在搭 Agent 平台，今天可优先阅读 Opik 的 tracing/eval 能力和 Dify 的 MCP/workflow 更新，oh-my-pi 适合对比终端 coding agent 的编辑保障；证据边界：GitHub 候选只确认本周期 updated/stars/summary/tags，未确认具体 commit 内容、release note 或 breaking change；来源：https://github.com/comet-ml/opik ，https://github.com/langgenius/dify ，https://github.com/can1357/oh-my-pi

### 时间线（北京时间）

- **2026-06-23（日期粒度，论文窗口内）**：Agent-native memory、SHERLOC 代码修复定位、隐私保护 RAG、知识投毒安全 Agent 等 arXiv 论文进入 36 小时窗口，主线偏 Agent/RAG 的评测、安全与系统化设计。
- **2026-06-24（日期粒度，新闻窗口内）**：OpenAI News 发布与 Broadcom 的 LLM 推理芯片 Jalapeño 消息，属于推理成本/供给链方向的 P1 信号。
- **2026-06-24 19:26**：`osmQwopus3.6-27B-Fable-Agentic` 更新，标签集中在 agentic、tool/function calling、reasoning。
- **2026-06-24 20:39–20:48**：Fabliq 8B Agent Reasoning 的 GGUF/FromBase GGUF 候选更新，强化本地量化 Agent 小模型观察线。
- **2026-06-24 21:11**：LFM2.5 8B terminal-agent RLVR/GRPO LoRA adapter 更新，提示 terminal-agent 后训练/适配继续活跃。
- **2026-06-24 21:31–21:35**：GitHub 上 oh-my-pi、Opik、Dify 等 LLM 工程/Agent workflow 仓库被巡检到活跃更新；注意这不是 release 级确认。

### 按主题分组重点

- **模型发布**：HF 出现多条 Agentic/terminal/reasoning/quantized 候选，P0/P1 足够但成熟度证据弱；重点不是立即替换线上模型，而是建立本地 Agent smoke test 队列。
- **Agent / RAG**：Agent memory 论文推动把记忆作为数据管理系统评测；SHERLOC 指向代码 Agent 的诊断定位；隐私 RAG 与知识投毒共同提示 RAG 安全链路需要覆盖“内容清洗 + 来源可信 + 回归攻击”。
- **推理与训练**：OpenAI/Broadcom Jalapeño 是推理芯片供给链 P1 信号；LFM2.5 adapter 的 RLVR/GRPO 标签是后训练方向观察点，但缺少效果数据。
- **多模态**：本周期无足够 P0/P1 多模态主线；`osmQwopus3.6` 标签含 image-text-to-text，但候选未提供多模态能力验证，暂不作为重点。
- **评测**：Opik 的 LLM/RAG/agent observability 与 Agent memory/SHERLOC 论文共同说明，评测正在从单点 benchmark 转向 workflow 级 tracing、定位和记忆子系统指标。
- **工程工具**：Dify、oh-my-pi、Opik 均是工程工具链活跃信号；但 GitHub updated 只代表活跃，今天不应写成“发布重大新功能”。
- **产品商业化**：OpenAI 推理芯片合作可能影响商业 API 成本曲线和供给能力，但候选未确认定价、开放策略或部署节奏。
- **数据**：本周期没有独立数据集/数据工程 P0/P1；RAG 安全论文可作为知识库数据治理的间接信号。

### 对 LLM 工程师的行动建议

- **今天应阅读**：OpenAI/Broadcom Jalapeño 新闻；Agent-native memory 论文；RAG 隐私重写与知识投毒两篇安全论文。
- **今天应实验**：SHERLOC 思路可在内部 repo bugfix 集上做小实验：比较传统 top-k 文件定位 vs. 结构化诊断上下文对修复成功率、token 消耗和工具调用轮次的影响。
- **应持续观察**：Fabliq 8B GGUF、osmQwopus 27B Agentic、LFM2.5 RLVR/GRPO adapter；Opik/Dify/oh-my-pi 的具体 commit/release note。观察原因是候选强但仍缺少实际 benchmark、release note 或生产验证。
- **暂不跟进**：未进入 P0/P1、缺少直接来源 URL、或只是旧来源背景的条目；本周期不为了凑数纳入今日重点。

### 固定入口

- 论文：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
- 新闻/博客：https://my.feishu.cn/docx/P16idvuAgo3u8ixAacXcmfXSn6R
- 模型发布：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb
- GitHub 项目：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g
- 时间索引：https://my.feishu.cn/docx/QZjEdsjnRoDVGixlJTOcjx3Dn8b
- 主题索引：https://my.feishu.cn/docx/OeMPdOXCSoG6JDxWU3qc5fcRn1c
