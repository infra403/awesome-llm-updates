## 2026-06-22 15:44 模型发布主题条目

### 模型发布与模型能力

- Multilingual-Multimodal-NLP/LoopCoder-V2（P0）：适合代码生成、代码推理、工具调用式 coding agent、对 looped/parallel-loop transformer 架构做复现或评估；风险：候选信息未给出参数规模、上下文长度和 benchmark，custom_code 需要审计 trust_remote_code；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Multilingual-Multimodal-NLP/LoopCoder-V2
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS（P1）：适合关注低比特多模态/聊天/编码模型在新硬件上的推理适配、chunked-prefill、Blackwell 专用部署链路；风险：uncensored/abliterated 带来安全与合规风险，Qwen3.6、参数、许可证、基准均未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP（P1）：适合比较 XS/非 XS 量化包在显存、速度、输出质量和多模态输入处理上的差异；风险：与 XS 版本关系、许可证、benchmark、上下文长度未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP
- Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16（P1）：适合 Mac/Apple Silicon 本地多模态推理、文档理解、图表理解、OCR 冒烟测试；风险：许可证、上下文长度、性能指标未在候选信息中确认，bf16 对内存要求更高；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16
- Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit（P1）：适合在 Mac 上做低内存多模态推理 PoC，与 bf16/4bit 对比质量和延迟；风险：量化误差、许可证、benchmark 未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit
- Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit（P1）：适合端侧/个人工作站多模态文档问答、图像理解、OCR 的轻量部署探索；风险：4bit 质量损失风险更高，许可证、benchmark 和硬件最低要求未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit
- LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters（P1）：适合研究终端 agent 的后训练/RLVR/GRPO adapter 方案，或对 LiquidAI LFM2.5 系列做可插拔能力实验；风险：仅 adapter，必须依赖基座，pipeline、评测结果、adapter 训练数据和安全边界未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters
- mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF（P2）：适合 CPU/边缘设备上的 Python agentic coding SFT 小模型试验、快速离线基线；风险：许可证、量化位宽、具体 GGUF 文件列表和质量指标未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF

### Agent 与多智能体

- Multilingual-Multimodal-NLP/LoopCoder-V2（P0）：适合代码生成、代码推理、工具调用式 coding agent；风险：custom_code 需要审计 trust_remote_code，参数规模和 benchmark 未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Multilingual-Multimodal-NLP/LoopCoder-V2
- WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit（P1）：适合俄语 agent、多模态/VLM、本地 Apple Silicon 量化部署和 MoE 推理路径观察；风险：下载为 0，成熟度未知，pipeline 缺失；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit
- WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit（P2）：适合更低内存 Apple Silicon 环境下验证俄语 agent/VLM 能力；风险：0 下载且 pipeline 未确认，4bit 质量损失和量化方法细节未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit
- LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters（P1）：适合研究终端 agent 的后训练/RLVR/GRPO adapter 方案；风险：仅 adapter，必须依赖基座，pipeline 和评测结果未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters
- mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF（P2）：适合本地轻量 coding agent 方向观察；风险：许可证、量化位宽、具体 GGUF 文件列表和质量指标未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF

### 推理、训练与后训练

- Multilingual-Multimodal-NLP/LoopCoder-V2（P0）：适合对 looped/parallel-loop transformer 架构做复现或评估；风险：参数规模、上下文长度和 benchmark 未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Multilingual-Multimodal-NLP/LoopCoder-V2
- LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters（P1）：适合研究 RLVR、ECHO、GRPO、LoRA adapter 在终端 agent 上的效果；风险：adapter 训练数据、安全边界和评测结果未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters

### 推理系统与工程工具

- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS（P1）：适合观察 NVFP4/MTP、Blackwell、chunked-prefill 等部署标签；风险：许可证、基准、上下文长度未确认，uncensored/abliterated 有安全风险；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP（P1）：适合比较同系列量化包差异；风险：与 XS 版本关系和许可证未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP
- Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16（P1）：适合 Apple Silicon/MLX 全精度多模态本地推理；风险：许可证、性能指标未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16
- Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit（P1）：适合 Apple Silicon/MLX 8bit 多模态部署对比；风险：量化误差和 benchmark 未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit
- Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit（P1）：适合更低内存 Apple Silicon 多模态部署；风险：4bit 质量损失更高；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit
- WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit（P1）：适合 MLX 8bit 俄语 agent/VLM/MoE 推理观察；风险：成熟度未知且 pipeline 缺失；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit
- WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit（P2）：适合低内存 MLX 4bit 实验；风险：0 下载且量化质量未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit
- mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF（P2）：适合 llama.cpp/CPU/边缘设备本地轻量 coding agent；风险：许可证、量化位宽和质量指标未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/mradermacher/qwen2.5-coder-1.5b-agentic-python-sft-GGUF

### 多模态与生成媒体

- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS（P1）：适合低比特多模态/聊天/编码模型在新硬件上的推理适配；风险：image-text-to-text 标签存在但实际多模态能力未在候选信息中确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP-XS
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP（P1）：适合多模态量化包工程观察；风险：许可证、benchmark、上下文长度未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-NVFP4-MTP
- Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16（P1）：适合文档理解、图表理解、OCR、多模态聊天的 Apple Silicon bf16 本地实验；风险：许可证和性能指标未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-bf16
- Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit（P1）：适合 Apple Silicon 低内存多模态推理 PoC；风险：量化误差和 benchmark 未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-8bit
- Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit（P1）：适合更低内存本地多模态文档问答和 OCR；风险：4bit 质量损失更高；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/Ferox-AI/Phi-4-multimodal-instruct-mlx-4bit
- WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit（P1）：适合俄语 VLM/agent 的 Apple Silicon 8bit 量化观察；风险：pipeline、成熟度、上下文长度未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_8bit
- WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit（P2）：适合更低内存俄语 VLM/agent 实验；风险：4bit 质量损失和量化方法细节未确认；详情：https://my.feishu.cn/docx/MFSbdDfMToLX6MxBUb7ck3y5nJg；原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-mlx_4bit
