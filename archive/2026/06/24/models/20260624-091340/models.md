## 2026-06-24 09:13 北京时间 | 模型发布巡检

本次依据候选报告的 10 小时窗口筛选；只写入候选中确认有更新时间、来源链接且具备工程跟进价值的 P0/P1 条目。未在候选信息中出现的参数规模、上下文长度、benchmark、训练细节或 license 均显式标注为未确认。

### 1. rodin-llm/rodin-1b

- **来源**：Hugging Face
- **更新时间**：2026-06-23T19:42:14.000Z
- **pipeline**：text-generation
- **license**：apache-2.0（来自候选标签）
- **likes/downloads**：1 / 0
- **重要性**：P0
- **主题标签**：模型发布与模型能力；推理系统与工程工具；数据集与数据工程
- **核心变化**：候选显示为 French、from-scratch、Llama 架构风格的 1B 级基础模型，并带有 safetensors、GGUF、text-generation-inference 标签；训练数据标签包括 HPLT、cc100、wikipedia、wikisource、PleIAs/common_corpus。
- **适用场景**：法语本地推理、低成本基座实验、法语 RAG/分类/抽取任务的轻量候选。
- **工程影响**：apache-2.0 与 GGUF/TGI 标签降低本地评估和服务化试验门槛；若团队有法语垂直任务，可作为“小模型是否足够”的成本基线。
- **工程风险**：likes/downloads 仍很低，候选未显示真实评测结果或社区验证；从 scratch 模型需要重点看 tokenizer、chat/instruct 适配与法语任务覆盖。
- **证据边界**：参数量从模型名推断为 1B，但候选未给出精确参数；上下文长度、benchmark、chat template、推理显存需求未在候选信息中确认；训练数据只确认候选标签列出的数据集名。
- **建议动作**：今天应阅读。理由：P0 且 license/GGUF/TGI/法语 from-scratch 信息对开源选型有直接工程影响。
- **URL**：https://huggingface.co/rodin-llm/rodin-1b

### 2. rodin-llm/rodin-1b-instruct

- **来源**：Hugging Face
- **更新时间**：2026-06-23T19:47:32.000Z
- **pipeline**：text-generation
- **license**：未在候选信息中确认
- **likes/downloads**：0 / 0
- **重要性**：P1
- **主题标签**：模型发布与模型能力；Agent 与多智能体；推理系统与工程工具
- **核心变化**：rodin-1b 的 instruct/chat 版本，候选标签显示 conversational、chatml、GGUF、safetensors，并标注 base_model:rodin-llm/rodin-1b。
- **适用场景**：法语对话、轻量 Agent 子任务、离线/边缘设备的指令跟随实验。
- **工程影响**：与基础版配套出现，便于比较 base vs instruct 在法语指令跟随、工具前后处理、RAG 问答中的收益；GGUF 标签意味着可优先用 llama.cpp 类本地栈做冒烟测试。
- **工程风险**：候选未给出 license，不能直接进入商用或再分发流程；没有 benchmark、上下文长度和模板细节，ChatML 标签仍需下载 tokenizer/config 后验证。
- **证据边界**：参数量、上下文长度、benchmark、license、量化文件明细、chat template 未在候选信息中确认；只确认候选标签中的 base_model、chatml、GGUF、safetensors。
- **建议动作**：今天应实验。理由：如果 rodin base 进入候选池，instruct 版应同步做最小指令跟随与本地推理验证。
- **URL**：https://huggingface.co/rodin-llm/rodin-1b-instruct

### 3. wilsonramos/qwen3-4b-2507-agentic-questionnaire-gguf

- **来源**：Hugging Face
- **更新时间**：2026-06-23T18:22:03.000Z
- **pipeline**：未在候选信息中确认
- **license**：未在候选信息中确认
- **likes/downloads**：0 / 0
- **重要性**：P1
- **主题标签**：Agent 与多智能体；推理系统与工程工具；模型发布与模型能力
- **核心变化**：Qwen/Qwen3-4B-Instruct-2507 的 GGUF 量化候选，标签显示 llama.cpp、tool-calling、agentic、endpoints_compatible、conversational。
- **适用场景**：本地 Agent 工具调用、小型问卷/结构化任务、低成本离线推理验证。
- **工程影响**：GGUF + llama.cpp + tool-calling 标签使它适合快速纳入本地 Agent runtime 的兼容性测试，尤其是函数调用格式、停止词和上下文管理。
- **工程风险**：非官方量化仓库且候选无下载/点赞；license 未确认，量化参数、校准方式、量化精度与工具调用模板均未确认。
- **证据边界**：参数量由 base_model 名称提示为 4B，但候选未给出精确配置；上下文长度、benchmark、license、量化位宽、chat/tool template 未在候选信息中确认。
- **建议动作**：今天应实验。理由：Agent/tool-calling GGUF 对本地 Agent 栈有直接兼容性价值，但必须先做模板和许可证核验。
- **URL**：https://huggingface.co/wilsonramos/qwen3-4b-2507-agentic-questionnaire-gguf

### 4. CMU-AIRe/MRT-online

- **来源**：Hugging Face
- **更新时间**：2026-06-23T23:34:04.000Z
- **pipeline**：text-generation
- **license**：mit（来自候选标签）
- **likes/downloads**：0 / 0
- **重要性**：P1
- **主题标签**：推理、训练与后训练；评测与基准；模型发布与模型能力
- **核心变化**：基于 deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B 的推理/数学后训练候选，标签包含 reinforcement-learning、reasoning、math、test-time-compute、mrt、grpo，并关联 arxiv:2503.07572。
- **适用场景**：小模型推理、数学题、test-time compute 策略、RL/GRPO 后训练复现实验。
- **工程影响**：对关注“更小推理模型 + 在线/测试时计算”的团队，可作为低成本评测对象；MIT 标签降低研究复现和内部评测摩擦。
- **工程风险**：候选无点赞/下载，实际效果未验证；基于蒸馏 R1 1.5B，能力上限和稳定性需要用内部 math/reasoning 集合重新评估。
- **证据边界**：上下文长度、benchmark 分数、训练配方细节、推理时计算开销、chat template 未在候选信息中确认；只确认候选标签中的 base_model、MIT、RL/GRPO/MRT 方向。
- **建议动作**：今天应阅读。理由：推理后训练与 test-time-compute 对评测/成本策略有方法论价值，先读模型卡和论文链接再决定是否跑实验。
- **URL**：https://huggingface.co/CMU-AIRe/MRT-online

### 5. voidful/gemma-4-12b-it-agent-sft-tw-fullft

- **来源**：Hugging Face
- **更新时间**：2026-06-23T23:15:24.000Z
- **pipeline**：text-generation
- **license**：gemma（来自候选标签）
- **likes/downloads**：0 / 0
- **重要性**：P1
- **主题标签**：Agent 与多智能体；多模态与生成媒体；模型发布与模型能力
- **核心变化**：google/gemma-4-12B-it 的 full-finetune Agent SFT 繁中候选，标签包含 traditional-chinese、agent-sft、claw-eval-zh、multimodal-preserved、dataset:voidful/agent-sft。
- **适用场景**：繁体中文 Agent 指令跟随、中文评测、需要保留多模态能力的 Gemma 系列微调对比。
- **工程影响**：如果团队在繁中 Agent 或中文工具调用场景做模型路由，可作为 Gemma 4 12B IT 的专项微调候选；“multimodal-preserved”标签提示需要验证微调后图文能力是否退化。
- **工程风险**：Gemma license 对使用场景有约束，需要单独审查；full-finetune 可能改变原模型安全/多模态行为；候选无社区热度。
- **证据边界**：上下文长度、benchmark 结果、具体 CLAW eval 分数、多模态评测、训练超参、chat/tool template 未在候选信息中确认。
- **建议动作**：持续观察。理由：方向对繁中 Agent 有价值，但当前候选证据不足，先等模型卡/评测补充或小样本验证。
- **URL**：https://huggingface.co/voidful/gemma-4-12b-it-agent-sft-tw-fullft

### 6. arlarena/if_step200

- **来源**：Hugging Face
- **更新时间**：2026-06-23T23:42:41.000Z
- **pipeline**：reinforcement-learning
- **license**：apache-2.0（来自候选标签）
- **likes/downloads**：0 / 0
- **重要性**：P1
- **主题标签**：推理、训练与后训练；评测与基准；模型发布与模型能力
- **核心变化**：基于 Qwen/Qwen3-8B-Base 的 GRPO/instruction-following 训练候选，标签包含 ifbench、slime、text-generation-inference、endpoints_compatible。
- **适用场景**：指令跟随训练复现、IFBench 对齐评测、Qwen3 8B Base 后训练流程参考。
- **工程影响**：Apache-2.0 与 TGI/endpoints_compatible 标签便于内部服务化测试；对后训练团队可用于观察 step200 早期 checkpoint 的 IF 能力变化。
- **工程风险**：pipeline 标为 reinforcement-learning，不一定是可直接上线的聊天模型；step200 可能只是中间 checkpoint，稳定性和对齐程度未知。
- **证据边界**：benchmark 分数、上下文长度、chat template、训练数据、step200 含义、推理资源需求未在候选信息中确认。
- **建议动作**：持续观察。理由：对后训练/评测有参考价值，但工程候选池应等更多 checkpoint 或模型卡细节。
- **URL**：https://huggingface.co/arlarena/if_step200

### 7. hyokwan/gemma3_multimodal_test

- **来源**：Hugging Face
- **更新时间**：2026-06-24T00:46:59.000Z
- **pipeline**：image-text-to-text
- **license**：未在候选信息中确认
- **likes/downloads**：0 / 0
- **重要性**：P1（弱证据，actionability_needs_validation）
- **主题标签**：多模态与生成媒体；模型发布与模型能力；推理系统与工程工具
- **核心变化**：Gemma3 图文到文本候选，标签显示 transformers、safetensors、image-text-to-text、conversational、TGI/endpoints_compatible。
- **适用场景**：Gemma3 多模态加载链路、图文问答 smoke test、TGI 兼容性验证。
- **工程影响**：若团队维护多模态推理服务，可作为近期 Gemma3 多模态模型卡/权重变更的观察点；但“test”命名提示不要直接纳入生产候选。
- **工程风险**：模型名包含 test 且无热度；license、base_model、评测、输入分辨率/视觉塔信息均缺失，工程可用性不明。
- **证据边界**：参数量、base_model、license、上下文长度、图像输入规格、benchmark、多模态保真度未在候选信息中确认。
- **建议动作**：暂不跟进。理由：只保留为多模态信号，当前证据不足以进入工程候选池。
- **URL**：https://huggingface.co/hyokwan/gemma3_multimodal_test

### 8. LLM-OS-Models/Fabliq-1.2B-Agent-JP-GGUF

- **来源**：Hugging Face
- **更新时间**：2026-06-23T17:54:33.000Z
- **pipeline**：未在候选信息中确认
- **license**：未在候选信息中确认
- **likes/downloads**：0 / 0
- **重要性**：P1（弱证据，actionability_needs_validation）
- **主题标签**：Agent 与多智能体；推理系统与工程工具；模型发布与模型能力
- **核心变化**：Fabliq-1.2B-Agent-JP 的 GGUF 版本，标签包含 gguf、conversational、endpoints_compatible；同批还出现 safetensors 版本和 Base/Base-GGUF 版本。
- **适用场景**：日语轻量 Agent、本地 GGUF 推理、Base vs Agent 变体对比。
- **工程影响**：1.2B 级 Agent JP 命名与 GGUF 标签对低成本日语 Agent 子任务有潜在价值，可用于本地 runtime 的语言覆盖测试。
- **工程风险**：候选信息很少且无 license；base_model/tag 仅显示 lfm2 出现在非 GGUF 版本候选中，本条未确认；无 benchmark 和下载热度。
- **证据边界**：参数量仅由模型名提示，未在候选元数据中确认；license、上下文长度、benchmark、chat/tool template、GGUF 量化位宽、训练数据未在候选信息中确认。
- **建议动作**：持续观察。理由：日语轻量 Agent 方向值得留意，但当前证据只够登记观察，不宜投入评测资源。
- **URL**：https://huggingface.co/LLM-OS-Models/Fabliq-1.2B-Agent-JP-GGUF
