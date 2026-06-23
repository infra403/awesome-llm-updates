## 2026-06-23 00:26 北京时间 | 模型发布巡检

### 1. jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp
- 来源：Hugging Face
- 更新时间：2026-06-22T15:01:43.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：2 / 638
- 重要性：P0
- 主题标签：模型发布与模型能力、Agent 与多智能体、推理系统与工程工具
- 适用场景：面向本地 agentic coding、tool-calling、no-thinking 推理路径，以及 AMD/ROCm、Ryzen AI Max 395 / Strix Halo 等本地部署评估；标签显示包含 llama.cpp、GGUF、ROCmFP4、MTP/speculative 相关线索。
- 工程风险：候选信息未确认原始模型卡细节、许可证、上下文长度、基准成绩和量化精度影响；“qwen3.6 / qwen35 / 27b”等仅来自标签，需核验来源权重与转换链路。
- 建议动作：优先下载模型卡与文件清单，核对 license、GGUF 分片、llama.cpp 加载参数、MTP 支持方式；在 AMD ROCm 目标机器上做短链路工具调用和代码任务 smoke test。
- URL：https://huggingface.co/jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp

### 2. nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill
- 来源：Hugging Face
- 更新时间：2026-06-22T16:16:35.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：1 / 0
- 重要性：P0
- 主题标签：模型发布与模型能力、推理、训练与后训练、Agent 与多智能体
- 适用场景：候选标签指向 Qwen/Qwen3.6-27B 的 reasoning/thinking/distillation/agentic/MTP/speculative-decoding 微调模型，可用于推理蒸馏、思维链风格、Agent 推理路径对比。
- 工程风险：候选信息未确认模型卡中的训练数据、蒸馏来源 DSV4Pro 含义、上下文长度、评测结果与实际 speculative decoding 接口；0 downloads 表明尚未有使用热度信号。
- 建议动作：核验模型卡和权重格式，检查是否提供 chat template / thinking 控制开关；用内部 reasoning 与 tool-use 小集对比基座 Qwen/Qwen3.6-27B。
- URL：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill

### 3. software-mansion/react-native-executorch-gemma-4-multimodal
- 来源：Hugging Face
- 更新时间：2026-06-22T08:39:30.000Z
- pipeline：audio-text-to-text
- license：apache-2.0
- likes/downloads：0 / 936
- 重要性：P0
- 主题标签：多模态与生成媒体、推理系统与工程工具、模型发布与模型能力
- 适用场景：面向 React Native + ExecuTorch 的 Gemma 4 E2B 量化多模态/音频文本到文本端侧推理，适合移动端多模态原型、离线语音/音频理解链路验证。
- 工程风险：候选信息未确认量化方案、端侧内存/延迟、支持平台矩阵、音频输入限制和模型卡完整部署步骤；下载量较高但 likes 为 0，需确认是否来自自动化依赖下载。
- 建议动作：优先评估 React Native 集成示例、ExecuTorch 版本锁定、Android/iOS 包体与内存峰值；验证 apache-2.0 与 google/gemma-4-E2B 基座条款是否一致。
- URL：https://huggingface.co/software-mansion/react-native-executorch-gemma-4-multimodal

### 4. cafonez/Agent-Nemotron-ROCmFP6
- 来源：Hugging Face
- 更新时间：2026-06-22T12:18:29.000Z
- pipeline：text-generation
- license：other
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 适用场景：候选标签显示为 NVIDIA Nemotron-3 Nano 30B-A3B BF16 的 GGUF/quantized/ROCmFP6 版本，面向 agentic、tool-calling、llama.cpp 与 ROCm 本地推理。
- 工程风险：license 为 other，商业/再分发风险需要重点核验；候选信息未确认量化精度、文件兼容性、上下文长度、工具调用模板和 Nemotron 原始条款。
- 建议动作：作为 ROCm 本地 agent 模型备选纳入观察，不进入生产前必须完成 license 审查和 llama.cpp 加载验证。
- URL：https://huggingface.co/cafonez/Agent-Nemotron-ROCmFP6

### 5. tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1
- 来源：Hugging Face
- 更新时间：2026-06-22T15:32:01.000Z
- pipeline：any-to-any
- license：apache-2.0
- likes/downloads：1 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、多模态与生成媒体、模型发布与模型能力
- 适用场景：标签包含 gemma4_unified、image-text-to-text、coding、agentic、terminal、tool-use、reasoning、thinking、local-llm，适合观察 Gemma 4 12B 多模态/工具使用社区微调路线。
- 工程风险：模型命名链路较长且基座标记为 yuxinlu1/...-GGUF 的 finetune，候选信息未确认权重来源、训练方法、上下文长度、benchmark 和真实 any-to-any 能力边界。
- 建议动作：先核对模型卡是否解释从 GGUF 到 safetensors 的来源与合法性；仅做离线实验，暂不用于面向用户的多模态能力承诺。
- URL：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1

### 6. tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1
- 来源：Hugging Face
- 更新时间：2026-06-22T15:31:58.000Z
- pipeline：any-to-any
- license：apache-2.0
- likes/downloads：1 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、多模态与生成媒体、模型发布与模型能力
- 适用场景：与上一条同源但标签为 gemma4_unified_assistant / text-generation，可能更偏 assistant 对话形态；适合比较 agentic Gemma 4 的 assistant 与 composer 版本差异。
- 工程风险：候选信息未确认两版本差异、训练数据、模型卡质量、基座合法性、上下文长度与多模态输入格式；0 downloads 说明还缺少社区验证。
- 建议动作：如果要评估 Gemma 4 agentic 微调，建议与第 5 条成对拉取模型卡，只保留文档更完整、模板更清晰的一支进入实验队列。
- URL：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1

### 7. JeloH/LLM4CodeRE-S2S-V1
- 来源：Hugging Face
- 更新时间：2026-06-22T12:54:03.000Z
- pipeline：未在候选信息中确认
- license：未在候选信息中确认
- likes/downloads：1 / 56
- 重要性：P1
- 主题标签：模型发布与模型能力、推理、训练与后训练
- 适用场景：标签显示为 PEFT adapter，基于 JeloH/xGenq-qwen2.5-coder-7b-instruct-OKI；模型名 LLM4CodeRE-S2S 暗示面向代码相关序列到序列任务，可作为代码理解/逆向工程类微调观察项。
- 工程风险：候选信息未确认 pipeline、license、任务定义、训练数据、评测指标和 adapter 加载方式；需要明确是否依赖私有/同名基座 adapter。
- 建议动作：读取模型卡确认 CodeRE 的任务含义与示例；若用于代码工程评估，先验证 adapter 与 base_model 可复现实例。
- URL：https://huggingface.co/JeloH/LLM4CodeRE-S2S-V1

### 8. xwk123/sft_appdelta_gui_agent
- 来源：Hugging Face
- 更新时间：2026-06-22T12:10:04.000Z
- pipeline：未在候选信息中确认
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、多模态与生成媒体、模型发布与模型能力
- 适用场景：标签包含 safetensors、qwen3_vl，模型名指向 GUI agent SFT，可用于观察视觉语言模型在应用界面操作/GUI agent 数据上的微调趋势。
- 工程风险：候选信息缺少 pipeline、license、基座、上下文长度、输入图像分辨率、GUI 数据来源与评测；0 downloads/0 likes 表明热度和可靠性都未验证。
- 建议动作：先作为情报线索记录；只有在模型卡提供数据来源和可运行 demo 后再进入 GUI agent benchmark。
- URL：https://huggingface.co/xwk123/sft_appdelta_gui_agent

### 9. mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft
- 来源：Hugging Face
- 更新时间：2026-06-22T15:48:11.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P2
- 主题标签：模型发布与模型能力、推理、训练与后训练、数据集与数据工程
- 适用场景：基于 Qwen/Qwen3-1.7B 的 biology / bio-posttrain / RNA SFT 小模型，适合作为生物序列后训练方向的轻量实验候选。
- 工程风险：候选信息未确认训练数据来源、RNA 任务定义、评测、上下文长度和生物安全边界；小模型能力上限需谨慎。
- 建议动作：关注模型卡是否补充数据与 benchmark；如团队有生物信息检索/生成需求，可纳入小规模离线评测。
- URL：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft

### 10. mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl
- 来源：Hugging Face
- 更新时间：2026-06-22T15:47:19.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P2
- 主题标签：模型发布与模型能力、推理、训练与后训练、数据集与数据工程
- 适用场景：基于 Qwen/Qwen3-1.7B 的 biology / bio-posttrain / DNA RL 小模型，适合观察生物序列 RL 后训练路线。
- 工程风险：候选信息未确认 RL 奖励设计、DNA 任务边界、评测和数据合规；不应直接用于高风险生物设计场景。
- 建议动作：与 RNA SFT 条目成对跟踪，等待模型卡补充 benchmark 后再决定是否进入内部 bio LLM 实验。
- URL：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl
