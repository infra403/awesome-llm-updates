## 2026-06-24 17:08 北京时间 | 模型发布巡检

本次仅写入候选报告 10 小时巡检窗口内有明确更新时间、来源链接和 P0/P1 工程价值信号的条目；未为凑数量写入低证据或旧模型卡。

### 1. gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF

- 来源：Hugging Face
- 更新时间：2026-06-24T05:09:59.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：2/0
- 重要性：P0
- 主题标签：模型发布与模型能力、Agent 与多智能体、推理系统与工程工具
- 核心变化：Qwen/Qwen-AgentWorld-35B-A3B 的 Q4_K_M GGUF 量化版本在本轮窗口内更新，标签包含 world-model、agent、environment-simulation、llama-cpp、GGUF，并关联数据集 Qwen/AgentWorldBench。
- 适用场景：本地/边缘 Agent 世界模型、环境模拟、llama.cpp 兼容性验证。
- 工程影响：值得进入工程候选池：GGUF + Q4_K_M 直接影响本地推理成本、显存/内存占用和 Agent 子任务离线实验门槛；Apache-2.0 标签降低商用试验阻力。
- 工程风险：下载量为 0、likes 为 2，尚无社区验证；非官方命名空间量化包需核查文件完整性、量化配置和基座一致性。
- 证据边界：参数量仅由模型名暗示为 35B-A3B，未在候选信息中确认；上下文长度、benchmark、训练数据细节、chat template、实际 llama.cpp 版本兼容性未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：今天应实验：优先拉取 GGUF 元数据并用 llama.cpp 做最小 smoke test，验证能否作为低成本 AgentWorld 基线。
- URL：https://huggingface.co/gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF

### 2. Dhptl/Qwen-AgentWorld-35B-A3B-GGUF

- 来源：Hugging Face
- 更新时间：2026-06-24T08:37:26.000Z
- pipeline：image-text-to-text
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、多模态与生成媒体、推理系统与工程工具
- 核心变化：Qwen-AgentWorld 相关 GGUF 包在本轮窗口内更新，pipeline 为 image-text-to-text，标签包含 multimodal、vlm、vision、environment-simulation、quantized，并关联 arxiv:2606.24597。
- 适用场景：多模态 Agent 环境模拟、视觉输入到文本决策链路的本地推理可行性验证。
- 工程影响：可进入候选池但需验证：如果 GGUF 能保留多模态路径，对本地多模态 Agent 原型有价值；同时可比较 text-generation 与 image-text-to-text 包的部署差异。
- 工程风险：0 likes/0 downloads；非官方命名空间；多模态 GGUF 的 projector/视觉塔文件、加载方式和运行时支持最容易缺失。
- 证据边界：参数规模、视觉塔结构、上下文长度、benchmark、chat template、具体推理命令未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：今天应阅读：先看模型卡文件列表与加载说明，确认是否真的具备可运行的多模态 GGUF 组件。
- URL：https://huggingface.co/Dhptl/Qwen-AgentWorld-35B-A3B-GGUF

### 3. lovedheart/Qwen-AgentWorld-35B-A3B-FP8

- 来源：Hugging Face
- 更新时间：2026-06-24T08:55:09.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：模型发布与模型能力、Agent 与多智能体、推理系统与工程工具
- 核心变化：Qwen-AgentWorld-35B-A3B 的 FP8 safetensors 版本在本轮窗口内更新，标签包含 qwen3_5_moe、image-text-to-text、world-model、agent、environment-simulation。
- 适用场景：GPU 侧 FP8 推理/服务化试验，和 GGUF 路径形成成本与吞吐对比。
- 工程影响：可进入候选池：FP8 版本可能影响 vLLM/TGI 等 GPU 推理成本、显存压力和吞吐；适合作为 AgentWorld 权重部署路线的候选之一。
- 工程风险：0 likes/0 downloads；候选信息未显示具体推理框架兼容标签；需防止 FP8 权重格式与目标服务框架不匹配。
- 证据边界：参数规模仅由名称暗示；上下文长度、benchmark、训练数据、chat template、vLLM/TGI/Transformers 版本要求未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：持续观察：等模型卡补齐部署说明后再做完整实验；今天可先记录为 FP8 路线候选。
- URL：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-FP8

### 4. Nexlab/VibeThinker-Fable-Nano-Agentic-3B

- 来源：Hugging Face
- 更新时间：2026-06-24T09:02:20.000Z
- pipeline：text-generation
- license：mit
- likes/downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理、训练与后训练、推理系统与工程工具
- 核心变化：3B agentic/coding/tool-use 模型在本轮窗口内更新，标签包含 qlora、qwen2.5-coder、GGUF、safetensors，基座为 zkxxxx/VibeThinker-3B-heretic。
- 适用场景：小模型工具调用、coding 辅助、低成本 Agent worker 或离线子任务。
- 工程影响：值得进入轻量候选池：3B + tool-use/coding 标签适合做本地 Agent worker、批量代码检索/修补辅助；MIT 标签有利于快速工程试验。
- 工程风险：0 likes/0 downloads，热度尚未形成；base_model 来自第三方，需核查继承许可证和训练数据声明。
- 证据边界：上下文长度、benchmark、工具调用格式、chat template、GGUF 量化文件可用性未在候选信息中确认；license 标签为 mit。
- 建议动作：今天应实验：用少量 tool-use/coding prompts 做 sanity check，重点看输出格式稳定性而非榜单分数。
- URL：https://huggingface.co/Nexlab/VibeThinker-Fable-Nano-Agentic-3B

### 5. mradermacher/Fabliq-8B-Agent-i1-GGUF

- 来源：Hugging Face
- 更新时间：2026-06-24T07:00:10.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：LLM-OS-Models/Fabliq-8B-Agent 的 GGUF 量化版本在本轮窗口内更新，标签包含 Liquid AI/LFM、MoE、agentic、tool-use、terminal、coding-agent、distillation、SFT、imatrix。
- 适用场景：终端/coding-agent 本地推理，尤其适合比较 8B 级工具模型与小模型 agentic 路线。
- 工程影响：可进入候选池：GGUF 和 terminal/coding-agent 标签对本地 Agent CLI、自动化脚本修复、离线 coding worker 有直接工程价值。
- 工程风险：量化发布者为 mradermacher，需核查原始模型卡；0 likes/0 downloads；i1 与非 i1 版本差异未说明。
- 证据边界：pipeline、上下文长度、benchmark、chat template、imatrix 数据来源、具体量化位宽未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：今天应阅读：优先比较 i1 与普通 GGUF 文件列表/量化说明，再决定是否下载测试。
- URL：https://huggingface.co/mradermacher/Fabliq-8B-Agent-i1-GGUF

### 6. LorMolf/Qwen-Embedding-ProcCode-aligned-2k

- 来源：Hugging Face
- 更新时间：2026-06-24T08:48:00.000Z
- pipeline：feature-extraction
- license：未在候选信息中确认
- likes/downloads：0/0
- 重要性：P1
- 主题标签：RAG 与知识工程、数据集与数据工程、推理系统与工程工具
- 核心变化：基于 Qwen/Qwen3-Embedding-0.6B 的 procurement/code aligned 2k 嵌入微调在本轮窗口内更新，标签包含 embeddings、legal-retrieval、procurement、lora-merged、text-embeddings-inference。
- 适用场景：采购/法务代码或流程文档检索、领域 RAG embedding baseline。
- 工程影响：可进入 RAG 候选池：领域对齐 embedding 可能改善采购/合规类语料召回；text-embeddings-inference 标签提示可纳入现有 embedding 服务链路评估。
- 工程风险：0 likes/0 downloads，领域泛化未知；2k 可能是上下文/训练设定但候选信息未确认含义。
- 证据边界：license、benchmark、训练数据、向量维度、最大输入长度、TEI 实际配置未在候选信息中确认；仅确认 base_model 和 lora-merged/feature-extraction 标签。
- 建议动作：今天应实验：用现有采购/法务样例做小规模 recall 对比，确认是否优于通用 Qwen3 embedding。
- URL：https://huggingface.co/LorMolf/Qwen-Embedding-ProcCode-aligned-2k

### 7. ssurface/qwen3-4b-grpo-l5

- 来源：Hugging Face
- 更新时间：2026-06-24T08:35:46.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：推理、训练与后训练、评测与基准、模型发布与模型能力
- 核心变化：基于 Qwen/Qwen3-4B-Instruct-2507 的 GRPO 微调模型在本轮窗口内更新，标签包含 gsm8k、chain-of-thought、cot-compression、level-5。
- 适用场景：小模型后训练、CoT 压缩、GSM8K 类数学推理实验对照。
- 工程影响：可作为研究候选：对工程团队理解 GRPO + CoT 压缩对小模型推理成本/输出长度的影响有参考价值。
- 工程风险：0 likes/0 downloads；同系列 l3/l4/l5 多个 checkpoint，需避免把实验 checkpoint 当稳定发布。
- 证据边界：level-5 含义、benchmark 分数、上下文长度、训练数据、chat template 未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：持续观察：除非正在做 GRPO/CoT 压缩实验，否则先记录同系列最高级别 checkpoint。
- URL：https://huggingface.co/ssurface/qwen3-4b-grpo-l5

### 8. idealab-cs2/reappraisal-4b-grpo

- 来源：Hugging Face
- 更新时间：2026-06-24T09:05:02.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：推理、训练与后训练、模型发布与模型能力、产品与商业化
- 核心变化：基于 Qwen/Qwen3-4B-Thinking-2507 的 GRPO/RLHF 微调在本轮窗口内更新，标签包含 cognitive-reappraisal、emotion-regulation、reasoning。
- 适用场景：心理/情绪调节类垂直助手、对话安全和推理风格控制研究。
- 工程影响：有限进入候选池：对通用 LLM 工程不是核心模型，但对垂直情绪调节产品和 RLHF/GRPO 行为塑形实验有参考。
- 工程风险：垂直医疗/心理场景合规风险高；0 likes/0 downloads；需严格评估安全边界。
- 证据边界：benchmark、临床/安全评测、训练数据、上下文长度、chat template 未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：持续观察：不建议直接上线，只适合研究行为塑形与安全评估样例。
- URL：https://huggingface.co/idealab-cs2/reappraisal-4b-grpo

### 9. LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN

- 来源：Hugging Face
- 更新时间：2026-06-24T08:57:30.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0/0
- 重要性：P1
- 主题标签：推理系统与工程工具、Agent 与多智能体、评测与基准
- 核心变化：Qwen-AgentWorld-35B-A3B 的 AutoRound W4A16 RTN 量化版本在本轮窗口内更新，标签包含 low-bit-open-llm-leaderboard、4-bit、auto-round。
- 适用场景：低比特 GPU/CPU 推理、量化方法对 AgentWorld 任务的退化评估。
- 工程影响：可作为量化路线观察项：W4A16 可能显著降低部署成本，但是否保持 Agent/环境模拟能力必须实测。
- 工程风险：reason_codes 显示 actionability_needs_validation；0 likes/0 downloads；license 未确认；LeaderboardModel1 命名空间需核查可信度。
- 证据边界：license、benchmark、上下文长度、chat template、AutoRound 配置和实际推理框架兼容性未在候选信息中确认。
- 建议动作：持续观察：先不纳入主实验，只在做量化对比时加入。
- URL：https://huggingface.co/LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN

### 10. AgentRen/avro-python-deflate-bomb-poc

- 来源：Hugging Face
- 更新时间：2026-06-24T08:12:31.000Z
- pipeline：未在候选信息中确认
- license：未在候选信息中确认
- likes/downloads：0/0
- 重要性：P1
- 主题标签：推理系统与工程工具、数据集与数据工程
- 核心变化：本轮窗口内出现模型格式漏洞 PoC 条目，标签包含 avro、security、model-format-vulnerability、denial-of-service。
- 适用场景：模型/数据集加载管线安全、CI 安全扫描、Hub artifact 下载治理。
- 工程影响：不作为能力模型进入候选池，但值得工程团队关注：提示模型与数据格式加载可能存在压缩炸弹/拒绝服务风险，影响自动下载、评测和训练数据流水线。
- 工程风险：这是 PoC/安全条目，不是可部署 LLM；若误下载运行可能带来安全风险。
- 证据边界：具体漏洞影响范围、复现代码、license、pipeline、修复版本未在候选信息中确认。
- 建议动作：今天应阅读：安全/平台团队应查看原文，评估是否需要在模型下载与 Avro 解析链路加大小/解压比限制。
- URL：https://huggingface.co/AgentRen/avro-python-deflate-bomb-poc

