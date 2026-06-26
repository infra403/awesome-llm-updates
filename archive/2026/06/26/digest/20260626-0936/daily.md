## 2026-06-26 09:36 北京时间 | 每日大模型情报

本周期信号不低：四路巡检中，论文侧集中出现 Agent/MCP/RAG 安全与评测议题，GitHub 侧有多个人工智能工程栈项目在当前窗口更新，新闻侧有 OpenAI Agent 工作研究与 Hugging Face vLLM Jobs 教程，模型侧有若干面向 Agent/推理的 HF 模型或适配器更新。以下只把带 `quality_score`、`priority_hint=P0/P1`、当前窗口日期和直接来源 URL 的候选纳入重点；对 GitHub“更新”类条目，证据边界明确限定为“仓库在窗口内更新”，不等同于新版本发布。

### 今日最重要（P0/P1）

1. **ShareLock：针对 MCP 的多工具阈值投毒攻击**：核心变化是 arXiv 2026-06-25 新增一篇 MCP 安全论文，指出随着 MCP 成为 Agent 调工具基础设施，攻击者可利用多工具、阈值式投毒绕过人工检查并在 LLM-server 交互中注入恶意提示；工程影响是所有使用 MCP server、工具 marketplace、远程工具注册表的 Agent 架构都需要重新评估工具描述、权限边界和审计策略；建议动作：**今天应阅读**，因为这是当前 Agent 工具链安全的高优先级风险；证据边界：候选确认了论文题名、日期、摘要和 URL，未确认攻击复现代码或影响范围，需阅读原文验证威胁模型；来源：https://arxiv.org/abs/2606.27027v1

2. **OpenRCA 2.0：从结果标签转向因果过程监督的 Agent RCA 评测**：核心变化是 arXiv 2026-06-25 新增 RCA/Agent 评测论文，提出 PAVE step-wise labeling protocol，试图把根因分析从“只猜最终 root cause”推进到“标注故障传播路径”；工程影响是对 SRE/可观测性 Agent、长上下文故障诊断、多步工具调用评测更有参考价值，可用于替代只看最终答案的弱评测；建议动作：**今天应阅读**，并把其评价维度映射到团队内部 incident-agent benchmark；证据边界：候选确认摘要、日期、arXiv URL，未确认数据集可下载状态、许可证和基准结果；来源：https://arxiv.org/abs/2606.27154v1

3. **RAG 安全与隐私综述：把检索索引、查询日志、上下文构造纳入威胁面**：核心变化是 arXiv 2026-06-24 当前窗口候选给出 RAG 安全/隐私系统综述，强调风险不只在生成模型本身，也在检索 pipeline、索引、日志和 context construction；工程影响是企业 RAG 需要补齐数据分级、索引隔离、日志脱敏、检索权限和 prompt/context 泄露测试，而不是只做答案安全过滤；建议动作：**今天应阅读**，适合作为 RAG 安全 checklist 的输入；证据边界：候选确认论文主题和摘要，未确认综述覆盖的防御成熟度或是否有可执行工具；来源：https://arxiv.org/abs/2606.25533v1

4. **Hugging Face：一条命令在 HF Jobs 上运行 vLLM Server**：核心变化是 Hugging Face Blog 2026-06-26 新增 vLLM Jobs 教程，指向把 vLLM server 快速部署到 HF Jobs 的更低门槛路径；工程影响是对临时评测、demo、模型冒烟测试和小规模服务验证有直接价值，可能降低为了试模型而维护自有 GPU 环境的成本；建议动作：**今天应实验**，优先用一个低风险开源模型验证启动时间、并发、成本和日志可观测性；证据边界：候选确认标题、日期、来源和 URL，但摘要未给出具体命令、定价或限制，需按博客实测；来源：https://huggingface.co/blog/vllm-jobs

5. **OpenAI：Agents are transforming work 研究/新闻稿**：核心变化是 OpenAI News 2026-06-25 发布关于 Agent 改变工作的研究文章，强调 Agent 正在承担更长、更复杂任务并扩展多角色生产力；工程影响是对团队 workflow 的启示大于模型选型本身：应把“任务持续时间、可验证中间产物、权限/工具边界、交接审计”作为 Agent 落地指标；建议动作：**持续观察**，作为产品与组织 workflow 设计参考，不宜直接当作工程基准；证据边界：候选确认来源、日期和概要，但未给出可复现实验细节或独立评测；来源：https://openai.com/index/how-agents-are-transforming-work

6. **LLM-OS-Models/LFM2.5-8B-A1B Raw ECHO RLVR GRPO Adapters**：核心变化是 Hugging Face 2026-06-26T01:15:25Z 更新一个基于 LiquidAI/LFM2.5-8B-A1B 的 Agent/terminal-agent/RLVR/GRPO LoRA adapter，标签显示 Apache-2.0；工程影响是可作为小模型 Agent 后训练/适配器路线的观察样本，尤其关注 terminal-agent 和 RLVR/GRPO 在工程任务上的增益；建议动作：**今天应实验**，但只建议 sandbox 冒烟，不建议直接进入生产评测池；证据边界：候选确认 HF 元数据、标签和更新时间，但 likes=1、downloads=0，未确认训练数据、评测结果和真实能力；来源：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters

7. **pmb：面向 AI coding agents 的本地优先持久记忆 MCP**：核心变化是 GitHub 当前窗口更新了 `oleksiijko/pmb`，描述为 Claude Code/Cursor/Codex 可用的 local-first persistent memory over MCP，使用 SQLite，支持 offline/multilingual，并带 BM25、向量检索、知识图谱等标签；工程影响是 Agent 记忆从“云端服务/隐藏状态”转向“可审计、本地文件、MCP 接入”的路线值得关注，直接影响代码 Agent 的长期决策记录、隐私和可迁移性；建议动作：**今天应实验**，用一个小代码仓库验证 memory write/read、冲突处理和隐私边界；证据边界：候选确认仓库元数据、更新时间 2026-06-26T01:32:56Z、stars=85 和摘要，未确认发布版本、协议稳定性或安全审计；来源：https://github.com/oleksiijko/pmb

### 按时间顺序的简短时间线

- **2026-06-24**：RAG 安全与隐私综述进入论文候选，主题覆盖检索架构、威胁、防御和可信系统方向；来源：https://arxiv.org/abs/2606.25533v1
- **2026-06-24**：多模态模型证据顺序敏感性审计论文进入候选，提示相同证据不同排序可能导致不同答案；来源：https://arxiv.org/abs/2606.26079v1
- **2026-06-25**：OpenAI 发布 Agent 改变工作的研究/新闻稿；来源：https://openai.com/index/how-agents-are-transforming-work
- **2026-06-25**：OpenRCA 2.0 和 ShareLock 两篇论文进入候选，分别聚焦 Agent RCA 过程监督评测与 MCP 工具投毒安全；来源：https://arxiv.org/abs/2606.27154v1 、https://arxiv.org/abs/2606.27027v1
- **2026-06-25T20:12:07Z**：`nightmedia/Qwen3.6-35B-A3B-Holo3-Qwopus-AgentWorld-qx64-hi-mlx` 在 HF 更新，标签显示 image-text-to-text、reasoning、long-cot、SFT/LoRA；来源：https://huggingface.co/nightmedia/Qwen3.6-35B-A3B-Holo3-Qwopus-AgentWorld-qx64-hi-mlx
- **2026-06-25T23:47:36Z**：`affaan-m/ECC` 仓库更新，摘要指向 Agent harness performance optimization、skills/instincts/memory/security；来源：https://github.com/affaan-m/ECC
- **2026-06-26T01:15:25Z**：`LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters` 更新；来源：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters
- **2026-06-26T01:30-01:33Z**：RAGFlow、Dify、pmb 等开源 Agent/RAG/Workflow 项目在当前窗口更新；来源：https://github.com/infiniflow/ragflow 、https://github.com/langgenius/dify 、https://github.com/oleksiijko/pmb
- **2026-06-26**：Hugging Face 发布 vLLM Server on HF Jobs 教程；来源：https://huggingface.co/blog/vllm-jobs

### 按主题分组的重点

- **模型发布**：LFM2.5-8B-A1B 的 RLVR/GRPO adapter 和 Qwen3.6/AgentWorld 相关模型更新显示“面向 Agent/terminal/coding/reasoning 的小模型或 MoE 适配”仍在快速试验。工程上应看重可复现训练说明、benchmark 和许可证；本周期候选多数下载/点赞很低，先 sandbox 冒烟，避免进入生产选型。
- **Agent/RAG**：OpenAI Agent 工作研究、pmb 本地记忆 MCP、Dify/RAGFlow 当前窗口更新共同指向 Agent workflow 与 RAG context layer 的工程化；但 GitHub 更新不等于新功能发布，后续需要看 release notes/commit diff。
- **推理与训练**：HF vLLM Jobs 是最直接可实验的推理部署信号；模型侧 RLVR/GRPO/QLoRA 标签说明后训练路线活跃，但证据只到模型卡元数据，能力仍需自测。
- **多模态**：多模态证据顺序敏感性论文提示 MLLM 评测要加入输入顺序/证据排列扰动，不应只测单一 prompt 版本；来源：https://arxiv.org/abs/2606.26079v1
- **评测**：OpenRCA 2.0 的过程监督非常适合 Agent benchmark 升级：从最终答案准确率扩展到路径、工具调用、因果链条。
- **安全**：ShareLock 与 RAG 安全综述是今日安全主线；MCP 工具投毒和 RAG 检索泄露都属于“模型外部上下文层”风险，应进入 Agent/RAG 安全评审。
- **工程工具**：pmb、ECC、trpc-agent-go、Dify/RAGFlow 等项目在窗口内活跃，建议只把 pmb/ECC 作为新方向扫描，其余成熟项目看 changelog 而不是按 stars 排序。
- **产品商业化**：OpenAI 文章偏产品/workflow 叙事，可用于 Agent KPI 和组织流程设计，但不作为模型能力证据。
- **数据**：本周期没有高置信新增数据集主线；RAG 安全综述涉及索引、查询日志、上下文构造的数据治理，应归入持续观察。

### 对 LLM 工程师的行动建议

- **今天应阅读**：ShareLock（MCP 安全）、OpenRCA 2.0（Agent RCA 评测）、RAG 安全与隐私综述。三者都直接影响 Agent/RAG 系统的评测与安全边界。
- **今天应实验**：HF vLLM Jobs 跑一个 vLLM server 冒烟；pmb 用本地仓库验证 MCP memory；LFM2.5 adapter 只做 sandbox 能力/许可证/模型卡完整性检查。
- **应持续观察**：OpenAI Agent work 研究、Dify/RAGFlow/ECC/trpc-agent-go 的实际 changelog、Qwen3.6/AgentWorld 类模型的下载、评测和复现信息。
- **暂不跟进**：缺少来源链接、DROP、非当前窗口或只有标题无质量字段的条目；本周期不要用旧来源填充今日重点。

### 固定入口

- 论文： https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
- 新闻博客： https://my.feishu.cn/docx/P16idvuAgo3u8ixAacXcmfXSn6R
- 模型发布： https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb
- GitHub： https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g
- 时间索引： https://my.feishu.cn/docx/QZjEdsjnRoDVGixlJTOcjx3Dn8b
- 主题索引： https://my.feishu.cn/docx/OeMPdOXCSoG6JDxWU3qc5fcRn1c
