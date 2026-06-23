## 2026-06-23 17:08 北京时间 | 模型发布巡检

> 巡检窗口：候选报告标注的最近 10 小时；本次只纳入候选中带有更新时间、来源链接且 priority_hint 为 P0/P1 的条目。时间索引：https://my.feishu.cn/docx/QZjEdsjnRoDVGixlJTOcjx3Dn8b；主题索引：https://my.feishu.cn/docx/OeMPdOXCSoG6JDxWU3qc5fcRn1c。

### [P0] osmapi/osmQwopus3.6-27B-Fable-Agentic

- 模型名：osmapi/osmQwopus3.6-27B-Fable-Agentic
- 来源：Hugging Face
- 更新时间：2026-06-23T04:25:33.000Z
- pipeline：text-generation
- license：agpl-3.0
- likes/downloads：1 / 0
- 重要性：P0
- 主题标签：Agent 与多智能体、推理、训练与后训练、模型发布与模型能力
- 核心变化：基于 Jackrong/Qwopus3.6-27B-v2 的全量微调版本，标签显示面向 agentic、tool-use、function-calling、reasoning / chain-of-thought，并使用 Glint-Research/Fable-5-traces 数据集。
- 适用场景：Agent 子任务、工具调用/函数调用 SFT 候选、推理轨迹数据蒸馏对比。
- 工程影响：对需要开源权重做工具调用策略微调或 agent 评测回放的团队有参考价值；但 AGPL-3.0 会直接影响商用/服务端集成合规评估。
- 工程风险：下载为 0、likes 仅 1，尚无社区验证；AGPL-3.0 需要法务确认；模型名称和 base_model 均非主流官方发布。
- 证据边界：参数量仅能从名称推断为 27B，候选元数据未独立确认；上下文长度、benchmark、chat template、推理显存、函数调用格式兼容性未在候选信息中确认。
- 建议动作：今天应阅读：P0 且 agent/tool-use 标签明确，先读模型卡确认训练目标与许可证义务。
- URL：https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic

### [P0] parth-1/metaguard-policy-agent-v1

- 模型名：parth-1/metaguard-policy-agent-v1
- 来源：Hugging Face
- 更新时间：2026-06-23T08:44:46.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 260
- 重要性：P0
- 主题标签：Agent 与多智能体、模型发布与模型能力、产品与商业化
- 核心变化：Llama 架构文本生成微调模型，标签包含 text-generation-inference、unsloth、policy-agent，候选窗口内下载量 260。
- 适用场景：策略/安全策略 Agent、轻量 guard/policy routing、TGI 部署候选。
- 工程影响：Apache-2.0 与 TGI 标签使其更容易进入工程 PoC；下载量在本批低热度候选中突出，值得检查是否适合做策略判断或 agent policy 节点。
- 工程风险：模型用途从名称推断为 policy-agent，但任务定义、输入输出 schema、误判率未确认；base_model 元数据指向自身，需核验真实基座。
- 证据边界：参数规模、上下文长度、benchmark、训练数据、chat template、真实 base model、推理资源需求未在候选信息中确认。
- 建议动作：今天应实验：Apache-2.0 + TGI + 下载量信号较强，可用小样本 policy prompts 做 smoke test。
- URL：https://huggingface.co/parth-1/metaguard-policy-agent-v1

### [P0] voidful/gemma-4-e4b-it-agent-sft-tw

- 模型名：voidful/gemma-4-e4b-it-agent-sft-tw
- 来源：Hugging Face
- 更新时间：2026-06-23T04:24:38.000Z
- pipeline：未在候选信息中确认
- license：gemma
- likes/downloads：0 / 2
- 重要性：P0
- 主题标签：Agent 与多智能体、评测与基准、模型发布与模型能力
- 核心变化：基于 google/gemma-4-E4B-it 的繁体中文 agent-sft 全量微调，标签含 traditional-chinese、claw-eval-zh。
- 适用场景：繁中 Agent 指令跟随、中文评测集对齐、低下载早期模型观察。
- 工程影响：如果团队需要繁体中文 agent 能力或中文评测适配，这是一个可读模型卡的早期候选；Gemma license 对再分发/商用边界需要单独核验。
- 工程风险：下载仅 2，工程成熟度不足；pipeline 未给出；Gemma 许可证不是 Apache/MIT，需确认使用条款。
- 证据边界：参数规模 E4B 含义、上下文长度、benchmark/CLAW-eval-ZH 分数、训练数据细节、chat template、推理框架兼容性未在候选信息中确认。
- 建议动作：今天应阅读：P0 且覆盖繁中 Agent/评测方向，先核验模型卡和许可证。
- URL：https://huggingface.co/voidful/gemma-4-e4b-it-agent-sft-tw

### [P1] autotrust/gemma4-31B-Fable-5-Distilled

- 模型名：autotrust/gemma4-31B-Fable-5-Distilled
- 来源：Hugging Face
- 更新时间：2026-06-23T08:34:51.000Z
- pipeline：text-generation
- license：gemma
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：多模态与生成媒体、Agent 与多智能体、推理、训练与后训练
- 核心变化：基于 google/gemma-4-31B-it 的 QLoRA 微调/蒸馏版本，标签含 fable-5、tool-use、code-generation、multimodal、reasoning。
- 适用场景：多模态 + tool-use/coding 复合能力探索、Fable-5 蒸馏数据对比。
- 工程影响：如果模型卡证实多模态和工具调用格式，可能用于大模型 Agent 的多模态子任务；31B 级别对本地推理成本较高，需量化或服务化评估。
- 工程风险：likes/downloads 均为 0，尚无采用信号；license 为 gemma；“multimodal”标签与 pipeline text-generation 之间需要模型卡核验。
- 证据边界：参数规模仅从名称/基座推断，候选信息未确认；上下文长度、benchmark、训练数据授权、chat template、视觉输入处理方式、推理框架兼容性未在候选信息中确认。
- 建议动作：今天应阅读：能力标签覆盖面广但证据弱，优先核验模型卡而非立即集成。
- URL：https://huggingface.co/autotrust/gemma4-31B-Fable-5-Distilled

### [P1] arizal/qwen2.5-1.5b-legal-sft

- 模型名：arizal/qwen2.5-1.5b-legal-sft
- 来源：Hugging Face
- 更新时间：2026-06-23T08:53:03.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：RAG 与知识工程、推理、训练与后训练、模型发布与模型能力
- 核心变化：基于 unsloth/Qwen2.5-1.5B-Instruct-bnb-4bit 的法律领域 SFT，标签含 text-generation-inference、unsloth。
- 适用场景：法律 RAG 的答案风格微调、小模型边缘部署、领域 SFT 基线。
- 工程影响：1.5B 级别若模型卡可靠，可作为低成本法律问答 rerank/草拟节点实验；Apache-2.0 对工程试验友好。
- 工程风险：无下载/点赞信号；法律领域数据、覆盖法域、幻觉控制未知，不适合直接生产。
- 证据边界：上下文长度、benchmark、训练数据来源/法域、chat template、量化兼容、法律可靠性评测未在候选信息中确认。
- 建议动作：持续观察：可记录为法律小模型候选，待模型卡和样例完善后再实验。
- URL：https://huggingface.co/arizal/qwen2.5-1.5b-legal-sft

### [P1] waynehwang/multimodal_sport_gemma3

- 模型名：waynehwang/multimodal_sport_gemma3
- 来源：Hugging Face
- 更新时间：2026-06-23T06:16:44.000Z
- pipeline：image-text-to-text
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：多模态与生成媒体、数据集与数据工程、模型发布与模型能力
- 核心变化：基于 google/gemma-3-4b-it 的韩语体育多模态微调，数据集标签为 hyokwan/multi_modal_sample，pipeline 为 image-text-to-text。
- 适用场景：体育图文理解、韩语多模态问答、垂直数据集微调样例。
- 工程影响：Apache-2.0 与 4B 级别基座适合做多模态小模型 PoC；对垂直体育数据集构建有参考意义。
- 工程风险：下载/点赞为 0，数据集 sample 性质可能较弱；适用语言为 ko，跨语言泛化未知。
- 证据边界：训练数据规模、图像分辨率/视觉塔、benchmark、上下文长度、chat template、推理框架兼容性未在候选信息中确认。
- 建议动作：持续观察：垂直多模态方向有参考性，但需等待模型卡和样例验证。
- URL：https://huggingface.co/waynehwang/multimodal_sport_gemma3

### [P1] AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4

- 模型名：AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4
- 来源：Hugging Face
- 更新时间：2026-06-23T07:37:34.000Z
- pipeline：image-text-to-text
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：多模态与生成媒体、推理系统与工程工具、模型发布与模型能力
- 核心变化：面向 Apple Silicon/MLX-VLM 的 FP4 量化多模态版本，标签含 mlx、apple-silicon、metal、quantized、vision、speculative-decoding。
- 适用场景：Mac 本地多模态推理、MLX-VLM 量化部署、FP4 低内存实验。
- 工程影响：如果文件和模型卡可用，可帮助评估 27B 级多模态模型在 Apple Silicon 上的本地推理成本；speculative-decoding 标签值得推理系统团队关注。
- 工程风险：名称含 uncensored，安全/合规风险高；license 未确认；下载为 0；多个架构标签如 mamba/ssm/linear-attention 需高度核验。
- 证据边界：参数规模、基座真实性、许可证、上下文长度、benchmark、实际 MLX 加载命令、量化精度损失未在候选信息中确认。
- 建议动作：持续观察：仅作为 MLX 量化信号跟踪，未经许可和安全核验不进入生产候选池。
- URL：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4

### [P1] AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit

- 模型名：AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit
- 来源：Hugging Face
- 更新时间：2026-06-23T07:37:33.000Z
- pipeline：image-text-to-text
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：多模态与生成媒体、推理系统与工程工具、模型发布与模型能力
- 核心变化：同系列 Apple Silicon/MLX-VLM 8bit 量化多模态版本，更新时间与 FP4 版本几乎同步。
- 适用场景：Mac 本地多模态推理、8bit 与 FP4 质量/速度对比、量化回归测试。
- 工程影响：可作为 FP4 版本的对照组，帮助判断极低比特量化的质量损失；对 MLX 部署链路有工程参考。
- 工程风险：license 未确认且名称含 uncensored；下载为 0；模型卡证据不足时不宜进入工程候选池。
- 证据边界：参数规模、许可证、上下文长度、benchmark、chat template、视觉输入格式、MLX 版本要求和显存/内存占用未在候选信息中确认。
- 建议动作：持续观察：仅在需要 Apple Silicon 多模态量化对照时读卡验证。
- URL：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit

### [P1] waynehwang/multimodal_sport_gemma3_gguf

- 模型名：waynehwang/multimodal_sport_gemma3_gguf
- 来源：Hugging Face
- 更新时间：2026-06-23T06:07:18.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：多模态与生成媒体、推理系统与工程工具、模型发布与模型能力
- 核心变化：waynehwang/multimodal_sport_gemma3 的 GGUF 相关发布，标签含 gguf、conversational、apache-2.0。
- 适用场景：llama.cpp/GGUF 本地部署、多模态体育模型的边缘推理尝试。
- 工程影响：若 GGUF 文件完整且支持对应视觉组件，可降低本地部署门槛；适合推理工程团队检查多模态 GGUF 支持链路。
- 工程风险：pipeline、量化类型、文件清单和视觉适配器未确认；多模态 GGUF 经常依赖额外 mmproj/视觉投影文件，需要核验。
- 证据边界：GGUF 量化等级、是否包含/需要 mmproj、上下文长度、benchmark、chat template、llama.cpp 兼容版本未在候选信息中确认。
- 建议动作：今天应阅读：GGUF 形态对部署影响直接，先核验文件列表和加载说明。
- URL：https://huggingface.co/waynehwang/multimodal_sport_gemma3_gguf

### [P1] INCModel2/GLM-5.2-MXFP4-Mixed-LLMC

- 模型名：INCModel2/GLM-5.2-MXFP4-Mixed-LLMC
- 来源：Hugging Face
- 更新时间：2026-06-23T03:22:35.000Z
- pipeline：text-generation
- license：other
- likes/downloads：0 / 12
- 重要性：P1
- 主题标签：推理系统与工程工具、模型发布与模型能力、推理、训练与后训练
- 核心变化：基于 zai-org/GLM-5.2 的量化版本，标签含 auto-round、8-bit、compressed-tensors、glm_moe_dsa。
- 适用场景：GLM-5.2 低比特/压缩张量推理、AutoRound 量化效果跟踪、MoE/DSA 架构部署观察。
- 工程影响：对关注 GLM 系列本地推理和压缩张量格式的团队有参考价值；下载 12 高于本批多数 0 下载模型。
- 工程风险：license 为 other，需要明确授权；量化格式与常用推理后端兼容性未确认；非官方发布可能存在权重来源风险。
- 证据边界：参数规模、上下文长度、benchmark、量化校准集、精度损失、chat template、vLLM/Transformers/llama.cpp 兼容性未在候选信息中确认。
- 建议动作：今天应阅读：量化与部署格式影响工程选型，但必须先核验许可证和后端兼容。
- URL：https://huggingface.co/INCModel2/GLM-5.2-MXFP4-Mixed-LLMC
