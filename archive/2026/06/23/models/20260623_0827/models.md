## 2026-06-23 08:27 北京时间 | 模型发布巡检

本次基于预运行候选列表筛选 10 条。所有参数规模、benchmark、license、pipeline 仅采用候选信息；未出现的字段标为“未在候选信息中确认”。

### 1. `reecdev/VibeThinker-3B-LQ8-GGUF`（P0）
- 模型名：`reecdev/VibeThinker-3B-LQ8-GGUF`
- 来源：Hugging Face
- 更新时间：2026-06-23T00:03:13.000Z
- pipeline：text-generation
- license：mit
- likes/downloads：0/0
- 重要性：P0
- 主题标签：模型发布与模型能力、推理、训练与后训练、评测与基准、推理系统与工程工具
- 适用场景：GGUF/LQ8 量化推理试用；关注 math、code、reasoning、gpqa、instruction-following 标签；可用于本地 reasoning/code 小模型候选。
- 工程风险：候选信息只确认其为 WeiboAI/VibeThinker-3B 的量化版本与 MIT 许可证；具体上下文长度、量化质量、GPQA 或代码基准分数未在候选信息中确认。
- 建议动作：优先拉取模型卡与 GGUF 文件清单，验证 llama.cpp 兼容性、提示模板和本地推理速度；如用于生产需自行做数学/代码回归评测。
- URL：https://huggingface.co/reecdev/VibeThinker-3B-LQ8-GGUF

### 2. `PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c`（P0）
- 模型名：`PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c`
- 来源：Hugging Face
- 更新时间：2026-06-22T21:05:33.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P0
- 主题标签：Agent 与多智能体、推理、训练与后训练、模型发布与模型能力
- 适用场景：基于 Qwen/Qwen3-32B 的 finetune，标签包含 qwen3、megatron；适合关注代码/AgenticRL 黑盒训练路线的工程团队跟踪。
- 工程风险：候选信息未确认训练数据、Agent 任务定义、上下文长度、评测结果和推理部署要求；模型名时间戳异常，需核对模型卡。
- 建议动作：进入观察名单；下载前先核验权重完整性、模型卡说明和 Qwen3-32B 基座兼容配置，重点做工具调用/代码任务离线评测。
- URL：https://huggingface.co/PGCodeLLM/AgenticRL-blackbox-260401_231502_cd7fb81c

### 3. `WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess`（P1）
- 模型名：`WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess`
- 来源：Hugging Face
- 更新时间：2026-06-22T17:04:41.000Z
- pipeline：未在候选信息中确认
- license：未在候选信息中确认
- likes/downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 适用场景：GGUF、llama.cpp、MoE、mixed-precision、ru-agent 标签，适合关注俄语 Agent 和本地量化部署的人跟踪。
- 工程风险：license、pipeline、参数细节和基座模型条款未在候选信息中确认；“Qwen3.6-35B-A3B”与 REAM/MTPLess 含义需以模型卡为准。
- 建议动作：暂不进入生产选型；先核对许可证、GGUF 量化配置、tokenizer/chat template 与 llama.cpp 加载情况。
- URL：https://huggingface.co/WaveCut/Qwen3.6-35B-A3B-REAM-160-ru-agent-GGUF-MTPLess

### 4. `yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit`（P1）
- 模型名：`yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit`
- 来源：Hugging Face
- 更新时间：2026-06-22T23:44:36.000Z
- pipeline：text-generation
- license：llama3.1
- likes/downloads：0/0
- 重要性：P1
- 主题标签：推理系统与工程工具、模型发布与模型能力
- 适用场景：Llama-3.1-8B-Instruct 的 AWQ 4-bit/compressed-tensors 量化，适合低显存推理、TGI 兼容性验证和部署基线对比。
- 工程风险：候选信息未确认量化校准集、精度损失、吞吐和上下文长度；Llama 3.1 许可证需按业务场景复核。
- 建议动作：作为 8B 级英文/通用指令模型量化部署候选；优先跑内部 prompt regression 与 AWQ/TGI 加载测试。
- URL：https://huggingface.co/yw223/Meta-Llama-3.1-8B-Instruct-AWQ-4bit

### 5. `RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO`（P1）
- 模型名：`RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO`
- 来源：Hugging Face
- 更新时间：2026-06-22T17:41:02.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理、训练与后训练、评测与基准
- 适用场景：Qwen3 4B、GRPO、unsloth、Minesweeper agent 标签，适合跟踪小模型通过 RL 学习游戏/环境策略的实验。
- 工程风险：候选信息未确认任务环境、奖励设计、训练集、评测指标和泛化表现；Minesweeper 代理能力不能外推到通用 Agent。
- 建议动作：作为 RL/GRPO 小模型案例观察；若复现需先查模型卡和训练脚本，再以固定局面集做策略评测。
- URL：https://huggingface.co/RealPirate786/Minesweeper_agent_Qwen3_4B_GRPO

### 6. `yw223/Qwen3-8B-AWQ-4bit`（P1）
- 模型名：`yw223/Qwen3-8B-AWQ-4bit`
- 来源：Hugging Face
- 更新时间：2026-06-22T23:48:26.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0/0
- 重要性：P1
- 主题标签：推理系统与工程工具、模型发布与模型能力
- 适用场景：Qwen/Qwen3-8B 的 AWQ 4-bit/compressed-tensors 量化，适合中文/多语 8B 模型低显存推理基线。
- 工程风险：候选信息未确认量化校准、困惑度/基准损失、上下文长度和实际吞吐；需要确认 chat template 与 TGI/vLLM/AWQ 兼容。
- 建议动作：建议纳入 8B 量化服务候选；与原始 Qwen3-8B、2-bit/3-bit 变体做准确率-显存-吞吐对比。
- URL：https://huggingface.co/yw223/Qwen3-8B-AWQ-4bit

### 7. `heterodoxin/fastcontext-1.0-4b-sft-apostate`（P1）
- 模型名：`heterodoxin/fastcontext-1.0-4b-sft-apostate`
- 来源：Hugging Face
- 更新时间：2026-06-22T23:47:35.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0/0
- 重要性：P1
- 主题标签：RAG 与知识工程、模型发布与模型能力、产品与商业化
- 适用场景：基于 microsoft/FastContext-1.0-4B-SFT 的 finetune，名称和标签指向 fast context、apostate、uncensored、abliteration；适合长上下文/RAG 工程关注但需谨慎。
- 工程风险：license 未确认；候选标签含 uncensored/abliteration，安全对齐、合规和输出风险较高；上下文长度和长文评测未在候选信息中确认。
- 建议动作：仅建议在隔离环境做研究评估；严禁直接接入面向用户的生产 RAG/Agent 服务，先补安全评测和许可证核验。
- URL：https://huggingface.co/heterodoxin/fastcontext-1.0-4b-sft-apostate

### 8. `yw223/Gemma-2-9B-it-AWQ-4bit`（P2）
- 模型名：`yw223/Gemma-2-9B-it-AWQ-4bit`
- 来源：Hugging Face
- 更新时间：2026-06-22T23:51:07.000Z
- pipeline：text-generation
- license：gemma
- likes/downloads：0/0
- 重要性：P2
- 主题标签：推理系统与工程工具、模型发布与模型能力
- 适用场景：Gemma-2-9B-it 的 AWQ 4-bit/compressed-tensors 量化，适合作为 Gemma 系列低显存推理补充候选。
- 工程风险：候选信息未确认量化质量、校准集、上下文长度、推理吞吐；Gemma 许可证需按业务用途复核。
- 建议动作：优先级低于更新基座或强能力模型；如已有 Gemma 9B 需求，可与 2-bit/3-bit 版本做部署对照。
- URL：https://huggingface.co/yw223/Gemma-2-9B-it-AWQ-4bit

### 9. `a3ilab-llm-uncertainty/gptoss_20b_all_zhtw_lr5e-7_ep5_64_128_256_base_cot_v6data_only_answer_loss_B_method`（P2）
- 模型名：`a3ilab-llm-uncertainty/gptoss_20b_all_zhtw_lr5e-7_ep5_64_128_256_base_cot_v6data_only_answer_loss_B_method`
- 来源：Hugging Face
- 更新时间：2026-06-22T18:52:31.000Z
- pipeline：text-generation
- license：other
- likes/downloads：0/0
- 重要性：P2
- 主题标签：推理、训练与后训练、模型发布与模型能力
- 适用场景：openai/gpt-oss-20b 的 LoRA/PEFT adapter，标签显示 zhtw、llama-factory、base_cot、only_answer_loss，适合关注繁中后训练与不确定性实验的人跟踪。
- 工程风险：license 为 other；训练数据、任务、评测、基座条款和 adapter 使用方式未在候选信息中确认；模型名包含大量实验超参但语义需核验。
- 建议动作：仅研究性跟踪；如用于繁中任务，先核验模型卡、adapter 加载方式与基座授权，再做繁中 QA/CoT 行为评测。
- URL：https://huggingface.co/a3ilab-llm-uncertainty/gptoss_20b_all_zhtw_lr5e-7_ep5_64_128_256_base_cot_v6data_only_answer_loss_B_method

### 10. `multimodalart/Boogu-Image-0.1-Edit-aoti-ds`（P2）
- 模型名：`multimodalart/Boogu-Image-0.1-Edit-aoti-ds`
- 来源：Hugging Face
- 更新时间：2026-06-22T19:37:49.000Z
- pipeline：未在候选信息中确认
- license：未在候选信息中确认
- likes/downloads：0/0
- 重要性：P2
- 主题标签：多模态与生成媒体、数据集与数据工程
- 适用场景：名称指向 Boogu Image 编辑相关数据/模型条目，适合关注图像编辑数据集或多模态生成媒体流水线的人后续核验。
- 工程风险：候选信息只有 region 与候选分数，未确认其是模型还是数据集、license、文件类型、pipeline、任务定义和评测。
- 建议动作：低优先级记录；仅在多模态巡检中打开模型卡确认类型与许可证后再决定是否纳入数据/模型资产库。
- URL：https://huggingface.co/multimodalart/Boogu-Image-0.1-Edit-aoti-ds
