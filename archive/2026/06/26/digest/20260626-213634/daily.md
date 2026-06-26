## 2026-06-26 21:36 北京时间 | 每日大模型情报

> 本周期整体信号来自四路巡检：论文 36h、新闻/博客 8h、模型 10h、GitHub 8h。新闻博客本周期低信号，仅 1 条 P1；今日主线主要来自 Agent/RAG 评测论文、Agent/RAG 开源项目更新、HF 模型发布与推理部署博客。以下只纳入带有 priority\_hint=P0/P1、quality\_score、reason\_codes、当前窗口日期和直接来源 URL 的候选。

### 今日最重要的 P0/P1

1. **Temporal Validity in Retrieval Memory：RAG 记忆需要显式时间有效性**：核心变化是论文指出传统 embedding 相似度无法可靠区分“重复事实”和“已过期/被推翻事实”，候选摘要给出 contradicted vs duplicated fact 的 AUROC 0.59（接近随机）；工程影响是长期记忆、代码知识库、API 文档 RAG 和 Agent workflow 需要把 valid\_from/valid\_to、版本和冲突消解纳入检索排序，而不是只依赖向量相似度；建议动作：**今天应阅读**，优先检查自家 RAG 是否会把旧 API、旧配置和旧决策与新事实混检；证据边界：已确认来源为 2026-06-25 arXiv 候选摘要，未确认完整实验设置和数据集细节；来源：https://arxiv.org/abs/2606.26511v1
2. **MIRROR：面向 Agentic RAG 的跨模态/跨攻击面红队框架**：核心变化是用 novelty-constrained memory-guided MCTS 生成更少重复的攻击样本，覆盖文本投毒、图像注入、direct-query attack 和 orchestrator-level tool manipulation；工程影响是多模态 Agentic RAG 的安全评测不能只做 prompt injection，应把检索层、工具编排层、图文输入层纳入统一红队；建议动作：**今天应阅读**，安全/评测负责人应抽取其攻击面分类转成内部 eval checklist；证据边界：已确认候选摘要声称现有文本投毒 benchmark 有 73-84% exact duplication，未确认 MIRROR 的开源状态与复现实验成本；来源：https://arxiv.org/abs/2606.26793v1
3. **OpenRCA 2.0 / PAVE：从结果标签转向因果过程监督的 RCA Agent 评测**：核心变化是候选摘要指出现有 RCA 数据集只标 root cause，容易退化成模式匹配；新协议强调 fault propagation path 的逐步标签；工程影响是 AIOps/可观测性 Agent、日志分析 Agent 和工具调用 Agent 的评测应考察“定位路径”而非只看最终答案；建议动作：**今天应阅读**，可把因果路径标签作为内部 incident replay eval 的评分维度；证据边界：已确认 2026-06-25 arXiv 摘要与 P0 评分，未确认数据规模、标注成本和是否提供代码；来源：https://arxiv.org/abs/2606.27154v1
4. **Qwen-AgentWorld-35B-A3B GGUF 量化版本出现 NVFP4/MXFP4-MOE 分支**：核心变化是 HF 上新增/更新 FreedomAISVR 的 Qwen-AgentWorld-35B-A3B-NVFP4-GGUF 与 MXFP4-MOE-GGUF，标签包含 agent、world-model、vision、multimodal、GGUF、Apache-2.0，更新时间分别为 2026-06-26 13:30:14/13:30:21 UTC；工程影响是本地/边缘 Agent、多模态 Agent 原型可以评估更低精度 GGUF 路线，但需要验证实际上下文、视觉能力、工具调用与量化精度损失；建议动作：**今天应实验**，只在隔离环境跑 smoke test 和小型 agent task，不直接进入生产模型池；证据边界：已确认 HF 元数据、下载量和标签，未确认官方来源、模型卡质量、benchmark 与安全评测；来源：https://huggingface.co/FreedomAISVR/Qwen-AgentWorld-35B-A3B-NVFP4-GGUF ，https://huggingface.co/FreedomAISVR/Qwen-AgentWorld-35B-A3B-MXFP4-MOE-GGUF
5. **GitHub Agent/RAG 工程栈集中活跃：Dify、RAGFlow、Neo.mjs、OpenLoomi**：核心变化是 2026-06-26 20:51-21:34 北京时间窗口内，多条高星/明确工程元数据项目更新，覆盖 production-ready agentic workflow、Agentic RAG、GraphRAG/long-term memory、proactive AI mates；工程影响是 Agent 平台从单点框架转向“workflow + memory/RAG + MCP + 多 Agent 编排”的集成栈，团队选型需要关注上下文工程、权限、安全和可观测性；建议动作：**持续观察**，只对正在选型的团队建立对比表，不因单次更新时间迁移平台；证据边界：已确认 GitHub 更新时间、stars、summary 和 tags，未确认本次提交具体变更内容；来源：https://github.com/langgenius/dify ，https://github.com/infiniflow/ragflow ，https://github.com/neomjs/neo ，https://github.com/melandlabs/openloomi
6. **HF Jobs 一行命令运行 vLLM Server**：核心变化是 Hugging Face Blog 发布 “Run a vLLM Server on HF Jobs in One Command”，把 vLLM server 与 HF Jobs 的启动流程包装为更短路径；工程影响是临时 benchmark、演示、短期推理服务和模型 smoke test 的环境准备成本下降，但长期生产仍要评估稳定性、配额、冷启动和观测；建议动作：**今天应实验**，用一个非敏感小模型跑 OpenAI-compatible endpoint smoke test；证据边界：已确认 2026-06-26 HF Blog P1 候选，未确认价格、区域配额、GPU 可用性和生产 SLA；来源：https://huggingface.co/blog/vllm-jobs

### 按时间顺序的简短时间线

- **2026-06-25（论文窗口）**：OpenRCA 2.0、MIRROR、Temporal Validity in Retrieval Memory 等 Agent/RAG 评测与安全论文进入 P0，说明今日论文主线集中在“长期记忆可靠性、Agentic RAG 安全、过程监督评测”。
- **2026-06-26 20:51 北京时间左右**：RAGFlow 更新，候选显示其定位为融合 RAG 与 Agent capabilities 的 context layer（GitHub stars 83,682；来源更新时间 2026-06-26T12:51:10Z）。
- **2026-06-26 21:16-21:30 北京时间**：HF 模型流出现 LFM2.5 RLVR/GRPO adapters、Qwen-AgentWorld 35B A3B GGUF 量化分支等 P0 候选，模型主线偏 Agent/terminal-agent/多模态本地推理。
- **2026-06-26 21:32-21:34 北京时间**：OpenLoomi、Neo.mjs、Dify 等 Agent/RAG/MCP 工程项目在 GitHub 候选流中集中更新，但本周期只确认仓库元数据与更新时间，未确认具体 commit 内容。
- **2026-06-26（新闻博客日期级）**：HF Blog 发布 vLLM on HF Jobs 教程，是新闻/博客流唯一 P1；Anthropic、Mistral、The Batch RSS 抓取失败，新闻面需要后续修复源。

### 按主题分组的重点

#### 模型
- **Qwen-AgentWorld-35B-A3B GGUF NVFP4/MXFP4-MOE**：可作为 Agent/world-model/vision 方向的本地推理候选，但先验证模型卡、推理兼容性、量化损失和多模态输入链路。来源：https://huggingface.co/FreedomAISVR/Qwen-AgentWorld-35B-A3B-NVFP4-GGUF
- **LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters**：候选标签包含 terminal-agent、rlvr、grpo、lora、adapter，适合作为“后训练/终端 Agent 行为适配”的观察对象；证据边界是 downloads=0 且候选只给 HF 元数据。来源：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters

#### Agent/RAG
- 今日最强主线是 Agentic RAG 的记忆、检索安全和过程评测：Temporal Validity 解决 stale-fact；MIRROR 覆盖跨攻击面红队；OpenRCA 2.0 强调因果过程监督。
- 工程判断：Agent/RAG 系统的下一阶段质量门槛应从“能答对”提升到“检索事实不过期、攻击面可枚举、推理路径可审计”。

#### 推理与训练
- HF Jobs + vLLM 是低摩擦推理部署信号，适合 demo、临时评测和 smoke test；不要把博客教程等同于生产 SLA。
- RLVR/GRPO adapter 候选说明 terminal-agent/工具使用后训练仍在持续出现，但需等模型卡和复现实验补齐。

#### 多模态
- Qwen-AgentWorld GGUF 候选带 vision/multimodal 标签，MIRROR 把图像注入纳入 Agentic RAG 攻击面；多模态 Agent 的安全和评测需要同步跟进。

#### 评测
- OpenRCA 2.0 与 Temporal Validity 都指向“过程/时效性”维度；建议内部 eval 加入时间冲突、版本迁移、因果路径评分。

#### 安全
- MIRROR 是今日安全主线：从 prompt injection 扩到 text poisoning、image injection、direct query、orchestrator/tool manipulation。

#### 工程工具 / 开源项目
- Dify、RAGFlow、Neo.mjs、OpenLoomi 的共同信号是 Agentic workflow + MCP + memory/RAG 的平台化；今日只建议观察和对比，不建议基于更新时间做迁移决策。

#### 产品商业化
- 本周期无足够 P0/P1 产品商业化信号；暂不补旧闻。

#### 数据
- Temporal Validity 暗示 RAG 数据工程必须记录事实生命周期和版本；OpenRCA 2.0 暗示 Agent eval 数据需要标注过程路径。

### 对 LLM 工程师的行动建议

- **今天应阅读**：Temporal Validity、MIRROR、OpenRCA 2.0 三篇论文；原因是它们直接影响 Agent/RAG 的评测、安全和长期记忆设计。
- **今天应实验**：HF Jobs 一行命令运行 vLLM；原因是可快速验证是否适合临时评测/演示环境。另可对 Qwen-AgentWorld GGUF 做最小 smoke test，但仅限隔离环境。
- **应持续观察**：Dify/RAGFlow/Neo.mjs/OpenLoomi 的具体 commit/release 内容，以及 LFM2.5 RLVR/GRPO adapters 的模型卡与复现实验。
- **暂不跟进**：缺少直接来源、DROP、非当前窗口或只靠旧来源的条目；本次未纳入。

### 固定入口

- 论文入口：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
- 新闻博客入口：https://my.feishu.cn/docx/P16idvuAgo3u8ixAacXcmfXSn6R
- 模型发布入口：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb
- GitHub 项目入口：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g
- 时间索引：https://my.feishu.cn/docx/QZjEdsjnRoDVGixlJTOcjx3Dn8b
- 主题索引：https://my.feishu.cn/docx/OeMPdOXCSoG6JDxWU3qc5fcRn1c
