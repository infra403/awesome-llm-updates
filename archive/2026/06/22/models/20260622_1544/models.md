## 2026-06-22 15:44 北京时间 | 模型发布巡检

本次基于预运行脚本注入的 Hugging Face 候选列表筛选；未在候选信息中出现的参数规模、上下文长度、benchmark、license 均不补写。

### 1. Multilingual-Multimodal-NLP/LoopCoder-V2
- 来源：Hugging Face
- 更新时间：2026-06-18T04:43:31.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：32/445
- 重要性：P0
- 主题标签：模型发布与模型能力、Agent 与多智能体、推理、训练与后训练
- 适用场景：代码生成、代码推理、工具调用式 coding agent、对 looped/parallel-loop transformer 架构做复现或评估。
- 工程风险：候选信息未给出参数规模、上下文长度和 benchmark；custom_code 需要审计 trust_remote_code；真实多语言/多模态能力未在候选信息中确认。
- 建议动作：优先拉取模型卡和论文核对架构、依赖与 eval；在隔离环境做小样本 HumanEval/MBPP/真实仓库修复任务冒烟测试。
- URL：https://huggingface.co/Multilingual-Multimodal-NLP/LoopCoder-V2

### 2. AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS
- 来源：Hugging Face
- 更新时间：2026-06-21T02:26:41.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：47/41791
- 重要性：P1
- 主题标签：模型发布与模型能力、多模态与生成媒体、推理系统与工程工具
- 适用场景：关注低比特多模态/聊天/编码模型在新硬件上的推理适配、chunked-prefill、Blackwell 专用部署链路。
- 工程风险：“uncensored/abliterated”带来安全与合规风险；Qwen3.6、参数/许可证/基准均未在候选信息中确认；XS 与非 XS 差异未确认。
- 建议动作：仅作为部署工程观察项；先核验模型卡、license、基座来源与权重格式，再决定是否进入内测。
- URL：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS

### 3. AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP
- 来源：Hugging Face
- 更新时间：2026-06-21T02:26:39.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：19/35515
- 重要性：P1
- 主题标签：模型发布与模型能力、多模态与生成媒体、推理系统与工程工具
- 适用场景：比较 XS/非 XS 量化包在显存、速度、输出质量和多模态输入处理上的差异。
- 工程风险：与 XS 版本关系、许可证、benchmark、上下文长度未在候选信息中确认；安全策略可能因 abliterated/uncensored 发生变化。
- 建议动作：若团队跟踪 NVFP4/MTP，可加入候选对照；否则暂不进入生产候选。
- URL：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP

### 4. Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16
- 来源：Hugging Face
- 更新时间：2026-06-19T20:44:11.000Z
- pipeline：image-text-to-text
- license：未在候选信息中确认
- likes/downloads：0/24
- 重要性：P1
- 主题标签：多模态与生成媒体、推理系统与工程工具、模型发布与模型能力
- 适用场景：Mac/Apple Silicon 本地多模态推理、文档理解、图表理解、OCR 冒烟测试。
- 工程风险：候选信息未确认许可证、上下文长度、性能指标；bf16 对内存要求更高；需确认与官方 Phi-4 multimodal 权重许可一致性。
- 建议动作：Apple Silicon 用户可优先验证安装和样例；工程侧记录 MLX 环境、显存/内存占用和推理吞吐。
- URL：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16

### 5. Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit
- 来源：Hugging Face
- 更新时间：2026-06-19T20:44:05.000Z
- pipeline：image-text-to-text
- license：未在候选信息中确认
- likes/downloads：0/20
- 重要性：P1
- 主题标签：多模态与生成媒体、推理系统与工程工具、模型发布与模型能力
- 适用场景：在 Mac 上做低内存多模态推理 PoC，与 bf16/4bit 对比质量和延迟。
- 工程风险：量化误差、许可证、benchmark 未在候选信息中确认；需检查 DocVQA/MMMU/ChartQA 等标签是否只是训练/评测数据引用。
- 建议动作：与 bf16 版本做相同输入集对比，记录 hallucination 和 OCR 准确率差异。
- URL：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit

### 6. Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit
- 来源：Hugging Face
- 更新时间：2026-06-19T20:42:36.000Z
- pipeline：image-text-to-text
- license：未在候选信息中确认
- likes/downloads：0/20
- 重要性：P1
- 主题标签：多模态与生成媒体、推理系统与工程工具、模型发布与模型能力
- 适用场景：端侧/个人工作站多模态文档问答、图像理解、OCR 的轻量部署探索。
- 工程风险：4bit 质量损失风险更高；许可证、benchmark 和硬件最低要求未在候选信息中确认。
- 建议动作：只建议作为本地推理实验；上线前必须与 bf16/8bit 做质量回归。
- URL：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit

### 7. WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit
- 来源：Hugging Face
- 更新时间：2026-06-22T07:15:35.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、多模态与生成媒体、推理系统与工程工具
- 适用场景：俄语 agent、多模态/VLM、本地 Apple Silicon 量化部署和 MoE 推理路径观察。
- 工程风险：下载为 0，成熟度未知；Qwen3.6、35B-A3B、REAM-160 含义和上下文长度未在候选信息中确认；pipeline 缺失。
- 建议动作：作为 P1 观察项保留；先核验 base_model 与模型卡，再决定是否测试俄语 agent 任务。
- URL：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit

### 8. WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit
- 来源：Hugging Face
- 更新时间：2026-06-22T06:51:24.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P2
- 主题标签：Agent 与多智能体、多模态与生成媒体、推理系统与工程工具
- 适用场景：更低内存 Apple Silicon 环境下验证俄语 agent/VLM 能力。
- 工程风险：0 下载且 pipeline 未确认；4bit 质量损失和量化方法细节未在候选信息中确认。
- 建议动作：若 8bit 版本通过冒烟，再用 4bit 做质量/内存折中评估。
- URL：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit

### 9. LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters
- 来源：Hugging Face
- 更新时间：2026-06-22T07:38:00.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：1/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理、训练与后训练、模型发布与模型能力
- 适用场景：研究终端 agent 的后训练/RLVR/GRPO adapter 方案，或对 LiquidAI LFM2.5 系列做可插拔能力实验。
- 工程风险：仅 adapter，必须依赖基座；pipeline、评测结果、adapter 训练数据和安全边界未在候选信息中确认。
- 建议动作：先核对基座许可与 adapter 加载方式；可用标准 terminal-agent 任务集做 AB 测试。
- URL：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters

### 10. mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF
- 来源：Hugging Face
- 更新时间：2026-06-22T05:13:59.000Z
- pipeline：未在候选信息中确认
- license：未在候选信息中确认
- likes/downloads：0/0
- 重要性：P2
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 适用场景：CPU/边缘设备上的 Python agentic coding SFT 小模型试验、快速离线基线。
- 工程风险：许可证、量化位宽、具体 GGUF 文件列表和质量指标未在候选信息中确认；0 下载说明热度暂低。
- 建议动作：如需要本地小模型基线，下载前先检查 GGUF quant 列表和 base_model 许可。
- URL：https://huggingface.co/mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF
