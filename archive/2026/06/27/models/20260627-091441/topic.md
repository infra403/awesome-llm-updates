## 2026-06-27 09:14 模型发布主题条目

### 模型发布与模型能力

- `InternScience/Agents-A1`（P0）：适合 Agent 子任务、工具调用前的对话/规划模型候选。风险：likes/downloads 仍低，参数量、上下文长度、benchmark、训练数据、chat template 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/InternScience/Agents-A1
- `Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2`（P1）：适合 Qwen3.5-9B GGUF 本地推理、coding/math/reasoning smoke test。风险：模型名中的 Claude/Opus 关系未在候选信息中确认，benchmark 与量化位宽未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2
- `ansulev/NRS_QWEN_MYTHOS_1M`（P1）：适合长上下文工具调用、代码 Agent、多步推理任务的离线评估。风险：1m-context 仅为候选标签，license 与实际上下文未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/ansulev/NRS_QWEN_MYTHOS_1M
- `havok2/Qwen-AgentWorld-35B-A3B-VL36`（P1）：适合视觉问答 Agent、UI/网页截图理解、多模态工具链观察。风险：merge/vision-graft 的 processor、投影层与模板兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/havok2/Qwen-AgentWorld-35B-A3B-VL36
- `shatu/Qwen3-8B-Reasoning-Fix`（P1）：适合小参数推理提示词回归和 TGI smoke test。风险：具体 fix 内容和 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/shatu/Qwen3-8B-Reasoning-Fix
- `issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf`（P1）：适合本地 coding Agent worker 初筛。风险：pipeline、license、base_model、量化等级均未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf
- `maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx`（P1）：适合 AgentWorld 量化与 Blackwell/DGX 推理栈观察。风险：NVFP4 运行框架、显存、吞吐未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx
- `olka-fi/Ornith-1.0-397B-MXFP4`（P1）：适合 vLLM 超大模型量化服务路径观察。风险：actionability_needs_validation，硬件需求、vLLM 版本和真实可运行性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/olka-fi/Ornith-1.0-397B-MXFP4
- `migtissera/GLM-5.2`（P1）：适合 GLM 系模型卡和 eval-results 核验。风险：第三方上传者与同名重复条目并存，官方关系与评测可信度未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/migtissera/GLM-5.2
- `somosnlp-hackathon-2026/mombeu-LFM2.5-350M`（P1）：适合低资源语言、文化对齐与小模型后训练观察。风险：350M 级能力边界较小，benchmark 与实际 Guarani 能力未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/somosnlp-hackathon-2026/mombeu-LFM2.5-350M

### Agent 与多智能体

- `InternScience/Agents-A1`（P0）：适合 Agent 对话/规划模型候选；风险是 chat template、上下文和显存需求未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/InternScience/Agents-A1
- `ansulev/NRS_QWEN_MYTHOS_1M`（P1）：适合长上下文工具调用与 coding-agent 验证；风险是 1M 上下文与工具格式未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/ansulev/NRS_QWEN_MYTHOS_1M
- `havok2/Qwen-AgentWorld-35B-A3B-VL36`（P1）：适合多模态 Agent 观察；风险是 vision-graft 可用性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/havok2/Qwen-AgentWorld-35B-A3B-VL36
- `issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf`（P1）：适合本地 coding-agent smoke test；风险是 license 和 base_model 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf
- `maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx`（P1）：适合 AgentWorld 高端 GPU 量化部署观察；风险是 NVFP4 生态依赖强。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx

### RAG 与知识工程

- `somosnlp-hackathon-2026/mombeu-LFM2.5-350M`（P1）：适合低资源语言/文化对齐 RAG 答案风格观察；风险是能力、上下文长度和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/somosnlp-hackathon-2026/mombeu-LFM2.5-350M

### 推理、训练与后训练

- `Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2`（P1）：适合本地推理与 coding/reasoning 基线实验；风险是蒸馏来源、benchmark、量化位宽未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2
- `ansulev/NRS_QWEN_MYTHOS_1M`（P1）：适合 SFT/工具调用/长上下文后训练观察；风险是 license、训练细节和真实上下文未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/ansulev/NRS_QWEN_MYTHOS_1M
- `shatu/Qwen3-8B-Reasoning-Fix`（P1）：适合 reasoning 微调效果对比；风险是修复目标与评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/shatu/Qwen3-8B-Reasoning-Fix
- `olka-fi/Ornith-1.0-397B-MXFP4`（P1）：适合 MXFP4/compressed-tensors 量化路径观察；风险是硬件与部署要求未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/olka-fi/Ornith-1.0-397B-MXFP4
- `migtissera/GLM-5.2`（P1）：适合 GLM MoE/DSA 与 eval-results 跟踪；风险是官方关系和评测可信度未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/migtissera/GLM-5.2

### 推理系统与工程工具

- `InternScience/Agents-A1`（P0）：适合端点兼容与 Agent 模型部署候选跟踪；风险是推理配置未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/InternScience/Agents-A1
- `Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2`（P1）：适合 llama.cpp/local-llm 实验；风险是 GGUF 量化等级与实际兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2
- `issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf`（P1）：适合本地 coding Agent 推理格式验证；风险是 license 与基础模型未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf
- `maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx`（P1）：适合 Blackwell/DGX NVFP4 推理栈验证；风险是硬件依赖强。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx
- `olka-fi/Ornith-1.0-397B-MXFP4`（P1）：适合 vLLM 超大模型量化加载验证；风险是 actionability_needs_validation 与高资源门槛。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/olka-fi/Ornith-1.0-397B-MXFP4

### 多模态与生成媒体

- `havok2/Qwen-AgentWorld-35B-A3B-VL36`（P1）：适合 image-text-to-text Agent/UI 截图理解方向观察；风险是视觉编码器来源、输入分辨率和 processor 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/havok2/Qwen-AgentWorld-35B-A3B-VL36

### 评测与基准

- `shatu/Qwen3-8B-Reasoning-Fix`（P1）：适合推理修复前后自建 benchmark 对比；风险是候选信息未给出分数。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/shatu/Qwen3-8B-Reasoning-Fix
- `migtissera/GLM-5.2`（P1）：适合 eval-results 可信度核验；风险是官方关系、评测集和分数未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/migtissera/GLM-5.2

### 数据集与数据工程

- `somosnlp-hackathon-2026/mombeu-LFM2.5-350M`（P1）：适合公开文化对齐数据集、DPO/SFT 流程观察；风险是训练细节与实际效果未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/somosnlp-hackathon-2026/mombeu-LFM2.5-350M
