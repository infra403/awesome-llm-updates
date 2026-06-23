## 2026-06-23 00:26 模型发布主题条目

### 模型发布与模型能力
- jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp（P0）：适合 AMD/ROCm 本地 agentic coding、tool-calling、GGUF/MTP 路线评估；风险是 license、上下文长度、量化影响和来源链路未在候选信息中确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp
- nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill（P0）：适合 Qwen3.6 27B 推理蒸馏、thinking、agentic 与 speculative-decoding 路线对比；风险是 DSV4Pro 含义、训练细节和 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill
- software-mansion/react-native-executorch-gemma-4-multimodal（P0）：适合移动端 Gemma 4 E2B 音频/多模态端侧推理原型；风险是量化方案、端侧资源占用和平台矩阵未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/software-mansion/react-native-executorch-gemma-4-multimodal
- cafonez/Agent-Nemotron-ROCmFP6（P1）：适合 Nemotron 系列 ROCm/llama.cpp agent 量化可行性观察；风险是 license 为 other 且量化精度与模板未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/cafonez/Agent-Nemotron-ROCmFP6
- tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1（P1）：适合 Gemma 4 12B agentic/composer 多模态社区微调观察；风险是来源链路、训练数据和 any-to-any 能力未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1
- tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1（P1）：适合同源 Gemma 4 12B assistant 形态对比；风险是两版本差异、模板和上下文长度未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1
- JeloH/LLM4CodeRE-S2S-V1（P1）：适合代码 RE/S2S 方向 PEFT adapter 线索跟踪；风险是 pipeline、license、任务定义和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/JeloH/LLM4CodeRE-S2S-V1
- xwk123/sft_appdelta_gui_agent（P1）：适合 GUI agent/Qwen3-VL SFT 趋势观察；风险是基座、license、数据来源和评测均未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/xwk123/sft_appdelta_gui_agent
- mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft（P2）：适合轻量生物/RNA 后训练实验观察；风险是任务定义、数据来源和 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft
- mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl（P2）：适合轻量生物/DNA RL 后训练路线观察；风险是奖励设计、数据合规和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl

### Agent 与多智能体
- jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp（P0）：适合 agentic coding、tool-calling 与本地 AMD 推理；风险是 license 与工具调用模板未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp
- nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill（P0）：适合 reasoning/thinking agent 对比；风险是训练来源和实际 agentic 能力未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill
- cafonez/Agent-Nemotron-ROCmFP6（P1）：适合 tool-calling agent 的 ROCmFP6 量化备选；风险是 license other。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/cafonez/Agent-Nemotron-ROCmFP6
- tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1（P1）：适合 terminal/tool-use agentic Gemma 观察；风险是来源与能力边界未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1
- tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1（P1）：适合 assistant 版 agentic Gemma 对比；风险是版本差异未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1
- xwk123/sft_appdelta_gui_agent（P1）：适合 GUI agent 数据与视觉操作模型线索跟踪；风险是信息不足。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/xwk123/sft_appdelta_gui_agent

### 推理系统与工程工具
- jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp（P0）：适合 llama.cpp/GGUF/ROCmFP4/MTP 工程可行性测试；风险是兼容性与 license 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jcbtc/chadrock3.6-27b-pi-agent-rocmfp4-mtp
- software-mansion/react-native-executorch-gemma-4-multimodal（P0）：适合 ExecuTorch + React Native 端侧部署；风险是资源占用和平台兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/software-mansion/react-native-executorch-gemma-4-multimodal
- cafonez/Agent-Nemotron-ROCmFP6（P1）：适合 ROCmFP6/llama.cpp 量化链路观察；风险是 license other 与量化精度未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/cafonez/Agent-Nemotron-ROCmFP6

### 多模态与生成媒体
- software-mansion/react-native-executorch-gemma-4-multimodal（P0）：适合音频文本到文本、移动端多模态推理；风险是音频输入限制未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/software-mansion/react-native-executorch-gemma-4-multimodal
- tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1（P1）：适合 image-text-to-text / any-to-any 能力线索跟踪；风险是多模态能力边界未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-safetensors-yuxinlu1
- tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1（P1）：适合多模态 assistant 版对比；风险是输入格式未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/tepirale/gemma-4-12B-agentic-fable5-composer2.5-v2-3.5x-tau2-assistant-safetensors-yuxinlu1
- xwk123/sft_appdelta_gui_agent（P1）：适合 qwen3_vl GUI agent 方向观察；风险是模型卡关键字段缺失。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/xwk123/sft_appdelta_gui_agent

### 推理、训练与后训练
- nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill（P0）：适合 thinking/distillation/speculative-decoding 路线评估；风险是训练来源和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill
- JeloH/LLM4CodeRE-S2S-V1（P1）：适合代码任务 PEFT adapter 后训练线索；风险是任务定义未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/JeloH/LLM4CodeRE-S2S-V1
- mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft（P2）：适合 RNA SFT 后训练观察；风险是数据和 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft
- mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl（P2）：适合 DNA RL 后训练观察；风险是奖励设计和数据合规未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl

### 数据集与数据工程
- mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft（P2）：适合追踪 RNA 领域数据后训练；风险是数据来源未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-rna-sft
- mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl（P2）：适合追踪 DNA RL 数据/奖励设计；风险是数据合规未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mims-harvard/bio-posttrain-qwen3-1.7b-dna-rl
