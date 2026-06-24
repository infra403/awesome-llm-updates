## 2026-06-25 01:08 模型发布主题条目

### 模型发布与模型能力
- ivgranite/Qwen-AgentWorld-35B-A3B-GGUF（P0）：适合本地 AgentWorld/环境模拟初测；风险是下载量为 0、量化质量和上下文/benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ivgranite/Qwen-AgentWorld-35B-A3B-GGUF
- mradermacher/Fabliq-8B-Agent-FromBase-GGUF（P0）：适合 8B 级终端 Agent 与本地部署候选；风险是 FromBase 能力边界、工具调用稳定性和上下文长度未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-FromBase-GGUF
- lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4（P1）：适合 Blackwell/NVFP4 低比特推理预研；风险是硬件/框架依赖强、模态能力边界不清。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4
- sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4（P1）：适合日英双语 reasoning 与低比特 vLLM 预研；风险是无热度信号且硬件门槛高。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4
- ermiaazarkhalili/Gemma4-E4B-SFT-Claude-Opus-Reasoning-Unsloth-GGUF（P1）：适合小模型 reasoning 蒸馏和 llama.cpp 本地试跑；风险是蒸馏数据合规和 Gemma license 边界需审查。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ermiaazarkhalili/Gemma4-E4B-SFT-Claude-Opus-Reasoning-Unsloth-GGUF
- leonsarmiento/Nex-N2-mini-5bit-text-mlx（P1）：适合 Mac/MLX 轻量 agentic 对话预研；风险是 license 未确认，暂不宜进入商业候选。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/leonsarmiento/Nex-N2-mini-5bit-text-mlx
- micymike/CodeMate-Qwen-1.5B-32K-Distilled-on-Claude-Fable-5（P1）：适合低成本 coding 辅助和代码摘要；风险是 license、真实 32K、benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/micymike/CodeMate-Qwen-1.5B-32K-Distilled-on-Claude-Fable-5
- HaimingW/qwen2.5-1.5b-faithful-summarization（P1）：适合 RAG 摘要和忠实性摘要链路预研；风险是 license 与忠实性评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/HaimingW/qwen2.5-1.5b-faithful-summarization

### Agent 与多智能体
- ivgranite/Qwen-AgentWorld-35B-A3B-GGUF（P0）：适合 Agent 环境模拟、本地 GGUF smoke test；风险是量化和工具调用兼容性需实测。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ivgranite/Qwen-AgentWorld-35B-A3B-GGUF
- mradermacher/Fabliq-8B-Agent-FromBase-GGUF（P0）：适合终端 Agent、小模型 Agent baseline；风险是 FromBase 能力可能弱于 reasoning 版本。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-FromBase-GGUF
- mradermacher/Fabliq-8B-Agent-Reasoning-i1-GGUF（P1）：适合工具使用和终端推理 A/B；风险是下载/点赞为 0，i1 量化效果未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-Reasoning-i1-GGUF
- jedisct1/Qwen-AgentWorld-35B-A3B-oQ8-MLX（P1）：适合 Apple Silicon/LM Studio AgentWorld 试用；风险是 MLX 与 tool-calling template 兼容性需实测。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jedisct1/Qwen-AgentWorld-35B-A3B-oQ8-MLX
- lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4（P1）：适合 AgentWorldBench 相关低比特推理预研；风险是 NVFP4 部署门槛和模态标签不一致。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4
- leonsarmiento/Nex-N2-mini-5bit-text-mlx（P1）：适合 Mac 本地 agentic 子任务；风险是 license 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/leonsarmiento/Nex-N2-mini-5bit-text-mlx

### RAG 与知识工程
- HaimingW/qwen2.5-1.5b-faithful-summarization（P1）：适合 RAG 文档压缩、忠实摘要后处理；风险是 faithfulness 不能只凭模型名确认，需要内部摘要评测。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/HaimingW/qwen2.5-1.5b-faithful-summarization

### 推理、训练与后训练
- mradermacher/Fabliq-8B-Agent-FromBase-GGUF（P0）：适合观察 distillation/SFT/ablation 后的 8B Agent baseline；风险是训练数据与指标未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-FromBase-GGUF
- mradermacher/Fabliq-8B-Agent-Reasoning-i1-GGUF（P1）：适合 reasoning SFT 与 FromBase 对照；风险是 reasoning 提升没有 benchmark 支撑。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-Reasoning-i1-GGUF
- sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4（P1）：适合 thinking/reasoning 低比特量化链路；风险是上下文和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4
- ermiaazarkhalili/Gemma4-E4B-SFT-Claude-Opus-Reasoning-Unsloth-GGUF（P1）：适合 reasoning 蒸馏小模型对照；风险是数据来源和 license 需审。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ermiaazarkhalili/Gemma4-E4B-SFT-Claude-Opus-Reasoning-Unsloth-GGUF
- micymike/CodeMate-Qwen-1.5B-32K-Distilled-on-Claude-Fable-5（P1）：适合 coding 蒸馏模型观察；风险是 distillation 来源、license 和代码 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/micymike/CodeMate-Qwen-1.5B-32K-Distilled-on-Claude-Fable-5
- HaimingW/qwen2.5-1.5b-faithful-summarization（P1）：适合 summarization fine-tune 对照；风险是训练数据和评测方法未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/HaimingW/qwen2.5-1.5b-faithful-summarization

### 推理系统与工程工具
- ivgranite/Qwen-AgentWorld-35B-A3B-GGUF（P0）：适合 llama.cpp/GGUF 本地部署；风险是具体量化档位和资源需求未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ivgranite/Qwen-AgentWorld-35B-A3B-GGUF
- jedisct1/Qwen-AgentWorld-35B-A3B-oQ8-MLX（P1）：适合 MLX/LM Studio 试跑；风险是无社区验证。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jedisct1/Qwen-AgentWorld-35B-A3B-oQ8-MLX
- lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4（P1）：适合 compressed-tensors/NVFP4 部署预研；风险是框架版本和硬件要求未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4
- sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4（P1）：适合 vLLM + W4A4/NVFP4 预研；风险是 Blackwell 依赖强。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4
- leonsarmiento/Nex-N2-mini-5bit-text-mlx（P1）：适合 mlx-lm 5-bit 本地运行；风险是 license 与量化质量未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/leonsarmiento/Nex-N2-mini-5bit-text-mlx

### 评测与基准
- lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4（P1）：标签关联 Qwen/AgentWorldBench，适合跟踪 AgentWorldBench 相关复现；风险是候选信息未给出任何 benchmark 数值。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4
