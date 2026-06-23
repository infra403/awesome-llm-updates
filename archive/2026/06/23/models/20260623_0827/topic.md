## 2026-06-23 08:27 模型发布主题条目

### 模型发布与模型能力

- `reecdev/VibeThinker-3B-LQ8-GGUF`（P0）：适合场景：GGUF/LQ8 量化推理试用；关注 math、code、reasoning、gpqa、instruction-following 标签；可用于本地 reasoning/code 小模型候选。 风险：候选信息只确认其为 WeiboAI/VibeThinker-3B 的量化版本与 MIT 许可证；具体上下文长度、量化质量、GPQA 或代码基准分数未在候选信息中确认。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/reecdev/VibeThinker-3B-LQ8-GGUF
- `PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c`（P0）：适合场景：基于 Qwen/Qwen3-32B 的 finetune，标签包含 qwen3、megatron；适合关注代码/AgenticRL 黑盒训练路线的工程团队跟踪。 风险：候选信息未确认训练数据、Agent 任务定义、上下文长度、评测结果和推理部署要求；模型名时间戳异常，需核对模型卡。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c
- `WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess`（P1）：适合场景：GGUF、llama.cpp、MoE、mixed-precision、ru-agent 标签，适合关注俄语 Agent 和本地量化部署的人跟踪。 风险：license、pipeline、参数细节和基座模型条款未在候选信息中确认；“Qwen3.6-35B-A3B”与 REAM/MTPLess 含义需以模型卡为准。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess
- `yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit`（P1）：适合场景：Llama-3.1-8B-Instruct 的 AWQ 4-bit/compressed-tensors 量化，适合低显存推理、TGI 兼容性验证和部署基线对比。 风险：候选信息未确认量化校准集、精度损失、吞吐和上下文长度；Llama 3.1 许可证需按业务场景复核。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit
- `yw223/Qwen3-8B-AWQ-4bit`（P1）：适合场景：Qwen/Qwen3-8B 的 AWQ 4-bit/compressed-tensors 量化，适合中文/多语 8B 模型低显存推理基线。 风险：候选信息未确认量化校准、困惑度/基准损失、上下文长度和实际吞吐；需要确认 chat template 与 TGI/vLLM/AWQ 兼容。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/yw223/Qwen3-8B-AWQ-4bit
- `heterodoxin/fastcontext-1.0-4b-sft-apostate`（P1）：适合场景：基于 microsoft/FastContext-1.0-4B-SFT 的 finetune，名称和标签指向 fast context、apostate、uncensored、abliteration；适合长上下文/RAG 工程关注但需谨慎。 风险：license 未确认；候选标签含 uncensored/abliteration，安全对齐、合规和输出风险较高；上下文长度和长文评测未在候选信息中确认。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/heterodoxin/fastcontext-1.0-4b-sft-apostate
- `yw223/Gemma-2-9B-it-AWQ-4bit`（P2）：适合场景：Gemma-2-9B-it 的 AWQ 4-bit/compressed-tensors 量化，适合作为 Gemma 系列低显存推理补充候选。 风险：候选信息未确认量化质量、校准集、上下文长度、推理吞吐；Gemma 许可证需按业务用途复核。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/yw223/Gemma-2-9B-it-AWQ-4bit
- `a3ilab-llm-uncertainty/gptoss_20b_all_zhtw_lr5e-7_ep5_64_128_256_base_cot_v6data_only_answer_loss_B_method`（P2）：适合场景：openai/gpt-oss-20b 的 LoRA/PEFT adapter，标签显示 zhtw、llama-factory、base_cot、only_answer_loss，适合关注繁中后训练与不确定性实验的人跟踪。 风险：license 为 other；训练数据、任务、评测、基座条款和 adapter 使用方式未在候选信息中确认；模型名包含大量实验超参但语义需核验。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/a3ilab-llm-uncertainty/gptoss_20b_all_zhtw_lr5e-7_ep5_64_128_256_base_cot_v6data_only_answer_loss_B_method

### Agent 与多智能体

- `PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c`（P0）：适合场景：基于 Qwen/Qwen3-32B 的 finetune，标签包含 qwen3、megatron；适合关注代码/AgenticRL 黑盒训练路线的工程团队跟踪。 风险：候选信息未确认训练数据、Agent 任务定义、上下文长度、评测结果和推理部署要求；模型名时间戳异常，需核对模型卡。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c
- `WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess`（P1）：适合场景：GGUF、llama.cpp、MoE、mixed-precision、ru-agent 标签，适合关注俄语 Agent 和本地量化部署的人跟踪。 风险：license、pipeline、参数细节和基座模型条款未在候选信息中确认；“Qwen3.6-35B-A3B”与 REAM/MTPLess 含义需以模型卡为准。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess
- `RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO`（P1）：适合场景：Qwen3 4B、GRPO、unsloth、Minesweeper agent 标签，适合跟踪小模型通过 RL 学习游戏/环境策略的实验。 风险：候选信息未确认任务环境、奖励设计、训练集、评测指标和泛化表现；Minesweeper 代理能力不能外推到通用 Agent。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO

### RAG 与知识工程

- `heterodoxin/fastcontext-1.0-4b-sft-apostate`（P1）：适合场景：基于 microsoft/FastContext-1.0-4B-SFT 的 finetune，名称和标签指向 fast context、apostate、uncensored、abliteration；适合长上下文/RAG 工程关注但需谨慎。 风险：license 未确认；候选标签含 uncensored/abliteration，安全对齐、合规和输出风险较高；上下文长度和长文评测未在候选信息中确认。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/heterodoxin/fastcontext-1.0-4b-sft-apostate

### 推理、训练与后训练

- `reecdev/VibeThinker-3B-LQ8-GGUF`（P0）：适合场景：GGUF/LQ8 量化推理试用；关注 math、code、reasoning、gpqa、instruction-following 标签；可用于本地 reasoning/code 小模型候选。 风险：候选信息只确认其为 WeiboAI/VibeThinker-3B 的量化版本与 MIT 许可证；具体上下文长度、量化质量、GPQA 或代码基准分数未在候选信息中确认。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/reecdev/VibeThinker-3B-LQ8-GGUF
- `PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c`（P0）：适合场景：基于 Qwen/Qwen3-32B 的 finetune，标签包含 qwen3、megatron；适合关注代码/AgenticRL 黑盒训练路线的工程团队跟踪。 风险：候选信息未确认训练数据、Agent 任务定义、上下文长度、评测结果和推理部署要求；模型名时间戳异常，需核对模型卡。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c
- `RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO`（P1）：适合场景：Qwen3 4B、GRPO、unsloth、Minesweeper agent 标签，适合跟踪小模型通过 RL 学习游戏/环境策略的实验。 风险：候选信息未确认任务环境、奖励设计、训练集、评测指标和泛化表现；Minesweeper 代理能力不能外推到通用 Agent。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO
- `a3ilab-llm-uncertainty/gptoss_20b_all_zhtw_lr5e-7_ep5_64_128_256_base_cot_v6data_only_answer_loss_B_method`（P2）：适合场景：openai/gpt-oss-20b 的 LoRA/PEFT adapter，标签显示 zhtw、llama-factory、base_cot、only_answer_loss，适合关注繁中后训练与不确定性实验的人跟踪。 风险：license 为 other；训练数据、任务、评测、基座条款和 adapter 使用方式未在候选信息中确认；模型名包含大量实验超参但语义需核验。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/a3ilab-llm-uncertainty/gptoss_20b_all_zhtw_lr5e-7_ep5_64_128_256_base_cot_v6data_only_answer_loss_B_method

### 推理系统与工程工具

- `reecdev/VibeThinker-3B-LQ8-GGUF`（P0）：适合场景：GGUF/LQ8 量化推理试用；关注 math、code、reasoning、gpqa、instruction-following 标签；可用于本地 reasoning/code 小模型候选。 风险：候选信息只确认其为 WeiboAI/VibeThinker-3B 的量化版本与 MIT 许可证；具体上下文长度、量化质量、GPQA 或代码基准分数未在候选信息中确认。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/reecdev/VibeThinker-3B-LQ8-GGUF
- `WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess`（P1）：适合场景：GGUF、llama.cpp、MoE、mixed-precision、ru-agent 标签，适合关注俄语 Agent 和本地量化部署的人跟踪。 风险：license、pipeline、参数细节和基座模型条款未在候选信息中确认；“Qwen3.6-35B-A3B”与 REAM/MTPLess 含义需以模型卡为准。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess
- `yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit`（P1）：适合场景：Llama-3.1-8B-Instruct 的 AWQ 4-bit/compressed-tensors 量化，适合低显存推理、TGI 兼容性验证和部署基线对比。 风险：候选信息未确认量化校准集、精度损失、吞吐和上下文长度；Llama 3.1 许可证需按业务场景复核。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit
- `yw223/Qwen3-8B-AWQ-4bit`（P1）：适合场景：Qwen/Qwen3-8B 的 AWQ 4-bit/compressed-tensors 量化，适合中文/多语 8B 模型低显存推理基线。 风险：候选信息未确认量化校准、困惑度/基准损失、上下文长度和实际吞吐；需要确认 chat template 与 TGI/vLLM/AWQ 兼容。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/yw223/Qwen3-8B-AWQ-4bit
- `yw223/Gemma-2-9B-it-AWQ-4bit`（P2）：适合场景：Gemma-2-9B-it 的 AWQ 4-bit/compressed-tensors 量化，适合作为 Gemma 系列低显存推理补充候选。 风险：候选信息未确认量化质量、校准集、上下文长度、推理吞吐；Gemma 许可证需按业务用途复核。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/yw223/Gemma-2-9B-it-AWQ-4bit

### 多模态与生成媒体

- `multimodalart/Boogu-Image-0.1-Edit-aoti-ds`（P2）：适合场景：名称指向 Boogu Image 编辑相关数据/模型条目，适合关注图像编辑数据集或多模态生成媒体流水线的人后续核验。 风险：候选信息只有 region 与候选分数，未确认其是模型还是数据集、license、文件类型、pipeline、任务定义和评测。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/multimodalart/Boogu-Image-0.1-Edit-aoti-ds

### 评测与基准

- `reecdev/VibeThinker-3B-LQ8-GGUF`（P0）：适合场景：GGUF/LQ8 量化推理试用；关注 math、code、reasoning、gpqa、instruction-following 标签；可用于本地 reasoning/code 小模型候选。 风险：候选信息只确认其为 WeiboAI/VibeThinker-3B 的量化版本与 MIT 许可证；具体上下文长度、量化质量、GPQA 或代码基准分数未在候选信息中确认。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/reecdev/VibeThinker-3B-LQ8-GGUF
- `RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO`（P1）：适合场景：Qwen3 4B、GRPO、unsloth、Minesweeper agent 标签，适合跟踪小模型通过 RL 学习游戏/环境策略的实验。 风险：候选信息未确认任务环境、奖励设计、训练集、评测指标和泛化表现；Minesweeper 代理能力不能外推到通用 Agent。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO

### 产品与商业化

- `heterodoxin/fastcontext-1.0-4b-sft-apostate`（P1）：适合场景：基于 microsoft/FastContext-1.0-4B-SFT 的 finetune，名称和标签指向 fast context、apostate、uncensored、abliteration；适合长上下文/RAG 工程关注但需谨慎。 风险：license 未确认；候选标签含 uncensored/abliteration，安全对齐、合规和输出风险较高；上下文长度和长文评测未在候选信息中确认。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/heterodoxin/fastcontext-1.0-4b-sft-apostate

### 数据集与数据工程

- `multimodalart/Boogu-Image-0.1-Edit-aoti-ds`（P2）：适合场景：名称指向 Boogu Image 编辑相关数据/模型条目，适合关注图像编辑数据集或多模态生成媒体流水线的人后续核验。 风险：候选信息只有 region 与候选分数，未确认其是模型还是数据集、license、文件类型、pipeline、任务定义和评测。 详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/multimodalart/Boogu-Image-0.1-Edit-aoti-ds
