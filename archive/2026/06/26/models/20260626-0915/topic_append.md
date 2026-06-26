## 2026-06-26 09:15 模型发布主题条目

### 模型发布与模型能力

- `sinonchum/Qwen3-4B-Feiyue-v1-bf16`（P1）：适合场景：Agent 工具调用、代码审查、PRD 生成等轻量中文/英文任务的候选适配器；风险：当前 likes/downloads 均为 0，只有模型卡标签层面的工程信号；需要确认 adapter 加载方式和实际指令跟随质量；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/sinonchum/Qwen3-4B-Feiyue-v1-bf16
- `ASTRAI-labs/pluto-nano-0.5`（P1）：适合场景：小型 MoE/reasoning 模型研究、低成本多语言推理实验；风险：license:other 与 custom_code 都会提高工程接入风险；实际参数量、激活参数、能力未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ASTRAI-labs/pluto-nano-0.5
- `MKSHRESTHA/Gemma-3-270m_Newari_autocomplete`（P1）：适合场景：低资源语言补全、数据集/微调流程参考、小模型本地实验；风险：license 未确认；任务偏 autocomplete，通用 LLM/Agent 工程影响有限；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/MKSHRESTHA/Gemma-3-270m_Newari_autocomplete

### Agent 与多智能体

- `Walid692/agentforge-mistral-7b-qlora`（P1）：适合场景：Mistral 7B Instruct 系生态中的 AgentForge 类 agent 实验或再微调基线；风险：未给出 pipeline_tag，热度为 0；需要验证 adapter 是否完整、是否有可复现实验说明；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Walid692/agentforge-mistral-7b-qlora
- `humanailabs/calendar-agent-fp16`（P1）：适合场景：日程/日历垂直 Agent、小型任务助手、工具调用前的意图解析候选；风险：custom_code 增加安全与部署审查成本；likes/downloads 为 0，实际日历任务能力未验证；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/humanailabs/calendar-agent-fp16
- `sahilchachra/Qwen-AgentWorld-35B-A3B-AWQ`（P1）：适合场景：AgentWorld 系模型的低比特本地/自托管推理候选，适合评估 MoE Agent 模型部署成本；风险：未提供下载/关注度信号；量化质量、兼容后端、实际显存占用需实测；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/sahilchachra/Qwen-AgentWorld-35B-A3B-AWQ
- `meshllm/Qwen-AgentWorld-35B-A3B-UD-Q4_K_XL-layers`（P1）：适合场景：llama.cpp/GGUF 本地推理用户评估 AgentWorld 35B-A3B 的低比特可运行性；风险：license 未确认；分层/量化包是否完整、tokenizer/chat template 是否匹配需验证；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/meshllm/Qwen-AgentWorld-35B-A3B-UD-Q4_K_XL-layers
- `LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-Tuning`（P1）：适合场景：比较 AWQ、AutoRound 等不同低比特路径对 AgentWorld 系模型的兼容性与质量影响；风险：leaderboard 标签不等于已验证榜单成绩；license 未确认，实际精度和后端兼容性需实测；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-Tuning
- `nightmedia/Qwen-AgentWorld-35B-A3B-qx64-hi-mlx`（P1）：适合场景：Apple Silicon/MLX 本地推理方向评估 AgentWorld 系模型；风险：候选标签缺少 license、pipeline、base_model、量化方法细节；工程可用性证据不足；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/nightmedia/Qwen-AgentWorld-35B-A3B-qx64-hi-mlx
