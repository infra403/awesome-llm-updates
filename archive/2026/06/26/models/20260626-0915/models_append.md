## 2026-06-26 09:15 北京时间 | 模型发布巡检

巡检窗口：候选报告标注的最近 10 小时；本次仅选入有 Hugging Face 来源链接且更新时间在窗口内、priority_hint=P1 的条目。P0 未发现。

### 1. `sinonchum/Qwen3-4B-Feiyue-v1-bf16`

- 来源：Hugging Face
- 更新时间：2026-06-26T00:06:52Z
- Pipeline：text-generation
- License：apache-2.0
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：模型发布与模型能力、Agent 与多智能体、推理、训练与后训练
- 核心变化：基于 Qwen/Qwen3-4B-Instruct-2507 的 LoRA/adapter 微调版本，标签指向 agent、tool-calling、code-review、prd-generation，bf16 权重形态。
- 适用场景：Agent 工具调用、代码审查、PRD 生成等轻量中文/英文任务的候选适配器。
- 工程影响：对本地小模型 Agent 子任务有潜在工程价值：4B 级底座若可复用，可能降低工具调用/文档生成链路成本。
- 工程风险：当前 likes/downloads 均为 0，只有模型卡标签层面的工程信号；需要确认 adapter 加载方式和实际指令跟随质量。
- 证据边界：参数量来自底座名 4B；上下文长度、benchmark、训练数据、chat template、推理框架兼容性未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：今天应阅读：优先查看模型卡与 adapter 配置，判断是否能快速接入现有 Qwen3 推理栈。
- URL：https://huggingface.co/sinonchum/Qwen3-4B-Feiyue-v1-bf16

### 2. `Walid692/agentforge-mistral-7b-qlora`

- 来源：Hugging Face
- 更新时间：2026-06-25T22:21:35Z
- Pipeline：未在候选信息中确认
- License：apache-2.0
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理、训练与后训练、模型发布与模型能力
- 核心变化：基于 mistralai/Mistral-7B-Instruct-v0.2 的 QLoRA/adapter 微调版本，标签包含 agentforge、fine-tuning、conversational。
- 适用场景：Mistral 7B Instruct 系生态中的 AgentForge 类 agent 实验或再微调基线。
- 工程影响：适合作为低成本 agent 微调配方参考，尤其是已有 Mistral 7B 部署路径的团队。
- 工程风险：未给出 pipeline_tag，热度为 0；需要验证 adapter 是否完整、是否有可复现实验说明。
- 证据边界：参数量来自底座名 7B；上下文长度、benchmark、训练数据、chat template、推理框架兼容性未在候选信息中确认；license 标签为 apache-2.0。
- 建议动作：持续观察：先看模型卡/文件结构，除非正在维护 Mistral AgentForge 方向，否则不急于实验。
- URL：https://huggingface.co/Walid692/agentforge-mistral-7b-qlora

### 3. `humanailabs/calendar-agent-fp16`

- 来源：Hugging Face
- 更新时间：2026-06-25T17:55:30Z
- Pipeline：text-generation
- License：mit
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、模型发布与模型能力、推理系统与工程工具
- 核心变化：基于 unsloth/Phi-4-mini-instruct 的日历 agent SFT/fp16 微调版本，标签含 calendar、sft、unsloth、trl、custom_code、TGI/endpoints_compatible。
- 适用场景：日程/日历垂直 Agent、小型任务助手、工具调用前的意图解析候选。
- 工程影响：对垂直工作流 agent 有参考意义；TGI/endpoints_compatible 标签暗示可能较容易接入服务化推理。
- 工程风险：custom_code 增加安全与部署审查成本；likes/downloads 为 0，实际日历任务能力未验证。
- 证据边界：底座、fp16、MIT、TGI/endpoints_compatible 来自候选标签；参数量、上下文长度、benchmark、训练数据、chat template 未在候选信息中确认。
- 建议动作：今天应阅读：重点核查 custom_code、模型卡任务定义和是否有日历工具调用格式。
- URL：https://huggingface.co/humanailabs/calendar-agent-fp16

### 4. `sahilchachra/Qwen-AgentWorld-35B-A3B-AWQ`

- 来源：Hugging Face
- 更新时间：2026-06-25T19:31:29Z
- Pipeline：text-generation
- License：apache-2.0
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：Qwen/Qwen-AgentWorld-35B-A3B 的 AWQ 量化版本，标签含 qwen3_5_moe、int4、w4a16、compressed-tensors、llm-compressor。
- 适用场景：AgentWorld 系模型的低比特本地/自托管推理候选，适合评估 MoE Agent 模型部署成本。
- 工程影响：若基座能力满足需求，AWQ/W4A16 可显著影响显存预算和吞吐测试计划。
- 工程风险：未提供下载/关注度信号；量化质量、兼容后端、实际显存占用需实测。
- 证据边界：35B-A3B、AWQ、int4/W4A16、apache-2.0 来自候选信息；上下文长度、benchmark、训练数据、chat template、精度损失未在候选信息中确认。
- 建议动作：今天应实验：如果已有 AWQ 推理栈，可做最小加载和长短样本 smoke test。
- URL：https://huggingface.co/sahilchachra/Qwen-AgentWorld-35B-A3B-AWQ

### 5. `meshllm/Qwen-AgentWorld-35B-A3B-UD-Q4_K_XL-layers`

- 来源：Hugging Face
- 更新时间：2026-06-25T19:29:49Z
- Pipeline：未在候选信息中确认
- License：未在候选信息中确认
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具
- 核心变化：Qwen-AgentWorld-35B-A3B 的 GGUF/UD-Q4_K_XL-layers 形态，标签含 gguf、imatrix、endpoints_compatible、conversational。
- 适用场景：llama.cpp/GGUF 本地推理用户评估 AgentWorld 35B-A3B 的低比特可运行性。
- 工程影响：对 CPU/消费级 GPU 本地试跑和边缘部署成本评估有直接价值。
- 工程风险：license 未确认；分层/量化包是否完整、tokenizer/chat template 是否匹配需验证。
- 证据边界：GGUF、Q4_K_XL、imatrix 来自候选标签；参数量来自模型名；上下文长度、benchmark、license、训练数据、chat template 未在候选信息中确认。
- 建议动作：今天应实验：GGUF 栈用户可先下载元数据或小范围加载验证，不建议直接进入生产候选。
- URL：https://huggingface.co/meshllm/Qwen-AgentWorld-35B-A3B-UD-Q4_K_XL-layers

### 6. `LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-Tuning`

- 来源：Hugging Face
- 更新时间：2026-06-25T17:52:58Z
- Pipeline：text-generation
- License：未在候选信息中确认
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、评测与基准
- 核心变化：Qwen-AgentWorld-35B-A3B 的 AutoRound W4A16 量化/调优版本，标签含 low-bit-open-llm-leaderboard、4-bit、auto-round。
- 适用场景：比较 AWQ、AutoRound 等不同低比特路径对 AgentWorld 系模型的兼容性与质量影响。
- 工程影响：可作为低比特量化方案横评样本，帮助选择服务端推理压缩路线。
- 工程风险：leaderboard 标签不等于已验证榜单成绩；license 未确认，实际精度和后端兼容性需实测。
- 证据边界：W4A16/4-bit/AutoRound 来自候选标签；上下文长度、benchmark、license、训练数据、chat template 未在候选信息中确认。
- 建议动作：持续观察：纳入量化方案对比清单，等待模型卡/下载信号更完整后实验。
- URL：https://huggingface.co/LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-Tuning

### 7. `nightmedia/Qwen-AgentWorld-35B-A3B-qx64-hi-mlx`

- 来源：Hugging Face
- 更新时间：2026-06-25T22:59:44Z
- Pipeline：未在候选信息中确认
- License：未在候选信息中确认
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具
- 核心变化：Qwen-AgentWorld-35B-A3B 的 MLX/6-bit 相关打包版本，标签含 qwen3_5_moe、6-bit。
- 适用场景：Apple Silicon/MLX 本地推理方向评估 AgentWorld 系模型。
- 工程影响：如果文件格式可用，可能扩展 AgentWorld 到 Mac 本地实验路径，影响个人开发者和端侧验证成本。
- 工程风险：候选标签缺少 license、pipeline、base_model、量化方法细节；工程可用性证据不足。
- 证据边界：MLX 来自模型名，6-bit 来自标签；参数量来自模型名；上下文长度、benchmark、license、训练数据、chat template、MLX 兼容细节未在候选信息中确认。
- 建议动作：持续观察：仅对 MLX 用户有跟进价值，先不进入通用候选池。
- URL：https://huggingface.co/nightmedia/Qwen-AgentWorld-35B-A3B-qx64-hi-mlx

### 8. `ASTRAI-labs/pluto-nano-0.5`

- 来源：Hugging Face
- 更新时间：2026-06-26T00:21:21Z
- Pipeline：text-generation
- License：other
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：模型发布与模型能力、推理、训练与后训练
- 核心变化：ASTRAI pluto-nano 系微调版本，标签含 mixture-of-experts、moe、reasoning、custom_code，多语言 en/pt/es/zh/hi。
- 适用场景：小型 MoE/reasoning 模型研究、低成本多语言推理实验。
- 工程影响：对小模型 MoE 架构和 reasoning 微调路线有观察价值，但需先过许可证与 custom_code 审查。
- 工程风险：license:other 与 custom_code 都会提高工程接入风险；实际参数量、激活参数、能力未确认。
- 证据边界：MoE、reasoning、custom_code、多语言标签来自候选信息；参数量、上下文长度、benchmark、训练数据、chat template、具体 license 条款未在候选信息中确认。
- 建议动作：今天应阅读：先确认 license:other 的条款和 custom_code 内容，未确认前不实验。
- URL：https://huggingface.co/ASTRAI-labs/pluto-nano-0.5

### 9. `MKSHRESTHA/Gemma-3-270m_Newari_autocomplete`

- 来源：Hugging Face
- 更新时间：2026-06-26T00:29:38Z
- Pipeline：text-generation
- License：未在候选信息中确认
- Likes/Downloads：0/0
- 重要性：P1
- 主题标签：模型发布与模型能力、数据集与数据工程、推理、训练与后训练
- 核心变化：基于 google/gemma-3-270m 的 Newari/Nepal Bhasa 低资源语言 autocomplete LoRA/SFT 版本，候选信息包含数据集标签 prageshshrestha/literature-scraped-text-corpus-for-newari-language。
- 适用场景：低资源语言补全、数据集/微调流程参考、小模型本地实验。
- 工程影响：对多语言覆盖和低资源语言数据工程有参考意义；270m 级底座可能适合轻量端侧实验。
- 工程风险：license 未确认；任务偏 autocomplete，通用 LLM/Agent 工程影响有限。
- 证据边界：270m 来自底座名；数据集标签、LoRA/SFT 来自候选信息；上下文长度、benchmark、license、训练数据细节、chat template 未在候选信息中确认。
- 建议动作：持续观察：有低资源语言需求时阅读，否则暂不进入通用工程候选池。
- URL：https://huggingface.co/MKSHRESTHA/Gemma-3-270m_Newari_autocomplete
