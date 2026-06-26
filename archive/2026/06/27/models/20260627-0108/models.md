## 2026-06-27 01:08 北京时间 | 模型发布巡检

本次筛选基于预运行脚本的 10 小时 Recency window；仅纳入候选信息中带有 Hugging Face 来源、URL、更新时间且 priority_hint=P1 的条目。未在候选中确认的参数规模、上下文长度、benchmark、训练数据、chat template 或框架兼容性均不补写。

### 1. s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF
- 来源：Hugging Face
- 更新时间：2026-06-26T16:35:02.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；推理系统与工程工具；Agent 与多智能体；推理、训练与后训练
- 核心变化：近期更新的 GGUF / NVFP4 / MTP 量化版本，标签显示面向 llama.cpp、speculative-decoding、agentic-coding、reasoning、Blackwell sm_120/sm_121。
- 适用场景：本地推理、低比特部署、投机解码实验、Agent coding 子任务候选池预研。
- 工程影响：如果模型卡与权重完整，可用于评估 NVFP4 + MTP 在 Blackwell GPU 或 llama.cpp 路径上的吞吐、显存与延迟收益；对需要本地部署推理模型的工程团队有验证价值。
- 工程风险：likes/downloads 均为 0，尚无使用反馈；license 未确认；NVFP4 / MTP 对运行栈和硬件支持要求较高。
- 证据边界：参数规模由名称暗示但未在候选信息中独立确认；上下文长度、benchmark、训练数据、chat template、具体推理命令、权重文件完整性和 license 未在候选信息中确认。
- 建议动作：今天应实验 —— 仅做小规模加载与吞吐 smoke test，优先验证 GGUF 文件、llama.cpp 兼容性和 NVFP4/MTP 是否真的可用。
- URL：https://huggingface.co/s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF

### 2. renaudb1999/le-harnais-ft-agentworld-8b
- 来源：Hugging Face
- 更新时间：2026-06-26T13:27:37.000Z
- pipeline：text-generation
- license：llama3.1
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体；模型发布与模型能力；推理系统与工程工具
- 核心变化：基于 meta-llama/Llama-3.1-8B-Instruct 的 AgentWorld 方向微调/量化候选，标签包含 transformers、safetensors、gguf、text-generation-inference、endpoints_compatible。
- 适用场景：Agent 工具调用/对话任务的 8B 级本地或端点部署评估。
- 工程影响：8B 规模通常更接近可部署候选池，可与 1B/3B 同系列进行成本、延迟、Agent 成功率和响应质量对比；TGI/endpoints_compatible 标签降低端点实验门槛。
- 工程风险：热度为 0，AgentWorld 微调效果未由候选信息给出；Llama 3.1 许可证约束需要纳入产品合规审查。
- 证据边界：benchmark、上下文长度、训练数据细节、chat template、AgentWorld 数据集/任务定义、GGUF 量化精度和实际推理兼容性未在候选信息中确认。
- 建议动作：今天应阅读 —— 先读模型卡确认微调目标、许可证与推理示例，再决定是否进入 Agent eval。
- URL：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-8b

### 3. renaudb1999/le-harnais-ft-agentworld-3b
- 来源：Hugging Face
- 更新时间：2026-06-26T13:18:59.000Z
- pipeline：text-generation
- license：llama3.2
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体；模型发布与模型能力；推理系统与工程工具
- 核心变化：基于 meta-llama/Llama-3.2-3B-Instruct 的 AgentWorld 方向微调/量化候选，标签包含 transformers、safetensors、gguf、TGI/endpoints_compatible。
- 适用场景：轻量 Agent、边缘/单卡推理、低成本对话流程。
- 工程影响：可作为 8B 版本的轻量对照，评估 Agent 子任务在 3B 级是否能保持足够指令遵循与工具使用能力。
- 工程风险：likes/downloads 为 0；微调收益未确认；Llama 3.2 许可证与部署范围需复核。
- 证据边界：benchmark、上下文长度、训练数据细节、chat template、量化参数和实际 GGUF/TGI 可用性未在候选信息中确认。
- 建议动作：持续观察 —— 与 8B 同系列合并跟踪，若模型卡给出 Agent eval 或下载增长再实验。
- URL：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-3b

### 4. renaudb1999/le-harnais-ft-agentworld-1b
- 来源：Hugging Face
- 更新时间：2026-06-26T13:14:07.000Z
- pipeline：text-generation
- license：llama3.2
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体；模型发布与模型能力；推理系统与工程工具
- 核心变化：基于 meta-llama/Llama-3.2-1B-Instruct 的 AgentWorld 方向微调/量化候选，标签包含 transformers、safetensors、gguf、TGI/endpoints_compatible。
- 适用场景：极低成本 Agent 分类、路由、简单指令执行或离线小模型 baseline。
- 工程影响：可用于判断 1B 级模型是否足以承担 Agent pipeline 中的低风险子任务，从而节省主模型调用成本。
- 工程风险：likes/downloads 为 0；1B 级模型可能在多步推理和工具调用上不稳定；许可证与实际商用限制需确认。
- 证据边界：benchmark、上下文长度、训练数据细节、chat template、GGUF 量化细节和部署兼容性未在候选信息中确认。
- 建议动作：持续观察 —— 作为同系列低成本候选记录，暂不优先投入实验资源。
- URL：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-1b

### 5. Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000
- 来源：Hugging Face
- 更新时间：2026-06-26T15:07:29.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体；推理系统与工程工具；模型发布与模型能力
- 核心变化：近期更新的 qwen3 / dflash / speculative-decoding / agent / longctx 相关 checkpoint，名称显示 step38000。
- 适用场景：长上下文 Agent、投机解码、Qwen3 系列衍生 checkpoint 预研。
- 工程影响：若 longctx 与 dflash 标签属实，可能影响长上下文 Agent 任务的吞吐、上下文窗口和成本评估；Apache-2.0 标签对工程试验较友好。
- 工程风险：checkpoint 性质可能不适合直接生产；pipeline 未确认；没有 likes/downloads 反馈。
- 证据边界：具体上下文长度、dflash 实现要求、benchmark、训练/后训练数据、chat template、base model 细节和推理框架兼容性未在候选信息中确认。
- 建议动作：今天应阅读 —— 重点确认 longctx 的真实窗口、加载方式和是否只是中间 checkpoint。
- URL：https://huggingface.co/Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000

### 6. Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF
- 来源：Hugging Face
- 更新时间：2026-06-26T16:41:08.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：5 / 0
- 重要性：P1
- 主题标签：多模态与生成媒体；模型发布与模型能力；推理系统与工程工具
- 核心变化：近期更新的 GGUF 量化版本，标签显示 vision、image-text-to-text、reasoning、long-context、1M-context、uncensored、abliterated、llama.cpp。
- 适用场景：本地多模态/长上下文 GGUF 可用性验证，特别是 image-text-to-text 与 1M context 宣称的边界测试。
- 工程影响：若模型卡与权重支持属实，可为本地多模态、超长上下文和 llama.cpp 路径提供新候选；5 likes 表明相对本批次有少量关注。
- 工程风险：uncensored/abliterated 标签带来安全与合规风险；downloads 为 0；1M context 和 vision 能力需实测，不宜直接进入生产。
- 证据边界：1M 上下文长度、视觉输入链路、benchmark、训练数据、chat template、GGUF 量化类型和实际 llama.cpp 兼容性未在候选信息中确认。
- 建议动作：今天应实验 —— 仅在隔离环境做加载、上下文长度和图文输入 smoke test，同时记录安全风险。
- URL：https://huggingface.co/Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF

### 7. srmty/smolLM2-360M-instruct-math-v1
- 来源：Hugging Face
- 更新时间：2026-06-26T16:25:36.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；推理、训练与后训练；评测与基准
- 核心变化：基于 HuggingFaceTB/SmolLM2-360M 的 math/reasoning 指令微调版本，标签包含 supervised-fine-tuning、alpaca、gpteacher、metamath、small-language-models。
- 适用场景：小模型数学推理 baseline、端侧/低资源推理、蒸馏或评测脚手架。
- 工程影响：360M 级别若能在基础数学任务上稳定，可作为低成本路由器、答案校验器或教学数据评测 baseline。
- 工程风险：模型很小，复杂推理能力预期有限；无下载/点赞反馈；数据混合和评测结果未确认。
- 证据边界：benchmark、训练样本规模、具体数据配比、上下文长度、chat template 和部署兼容性未在候选信息中确认。
- 建议动作：持续观察 —— 适合作为轻量 baseline 记录，等模型卡给出 math eval 后再加入系统评测。
- URL：https://huggingface.co/srmty/smolLM2-360M-instruct-math-v1

### 8. jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-8B
- 来源：Hugging Face
- 更新时间：2026-06-26T14:21:56.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；数据集与数据工程；推理系统与工程工具
- 核心变化：基于 Qwen/Qwen3-8B-Base 的粤语 chat/vector merged 微调版本，标签包含 arxiv:2309.00071、arxiv:2505.09388、TGI/endpoints_compatible。
- 适用场景：粤语对话、区域语言 RAG/客服、中文方言评测集构建。
- 工程影响：为粤语场景提供 Qwen3-8B 衍生候选，可用于比较通用中文模型在粤语输入、繁简混杂和本地表达上的差异。
- 工程风险：无下载/点赞反馈；“vector_merged” 方法和数据来源需审查；方言能力必须用自有粤语测试集验证。
- 证据边界：benchmark、训练数据许可、上下文长度、chat template、合并方法细节和实际 TGI 兼容性未在候选信息中确认。
- 建议动作：今天应阅读 —— 若业务涉及粤语客服/RAG，应先确认模型卡的数据与许可，再安排小评测。
- URL：https://huggingface.co/jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-8B

### 9. nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4
- 来源：Hugging Face
- 更新时间：2026-06-26T16:59:04.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：推理、训练与后训练；模型发布与模型能力；推理系统与工程工具
- 核心变化：Qwen/Qwen3.6-27B 的 thinking/distill/NVFP4 量化候选，标签包含 reasoning、nvfp4、w4a16、quantized、distilled、modelopt。
- 适用场景：推理型模型蒸馏、NVFP4/W4A16 量化部署、27B 级本地推理实验。
- 工程影响：对关注推理模型部署成本的团队有价值，可验证 distill + NVFP4/W4A16 对质量、延迟、显存的折中。
- 工程风险：Qwen3.6-27B 与 DSV4Pro 命名信息需核验；downloads/likes 为 0；量化和推理能力宣称需要实测。
- 证据边界：benchmark、上下文长度、原始模型卡、蒸馏数据、chat template、modelopt 配置和硬件兼容性未在候选信息中确认。
- 建议动作：今天应阅读 —— 先核验模型卡与权重来源；若链路可信，再做量化加载测试。
- URL：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4

### 10. jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507
- 来源：Hugging Face
- 更新时间：2026-06-26T14:25:15.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；推理、训练与后训练；数据集与数据工程
- 核心变化：基于 Qwen/Qwen3-30B-A3B-Base 的粤语 chat/vector merged 思考型版本，标签包含 qwen3_moe、conversational、TGI/endpoints_compatible。
- 适用场景：粤语复杂问答、区域语言推理任务、MoE 模型在方言场景的对照实验。
- 工程影响：可与同作者 Qwen3-8B 粤语版本组成大小模型对照，评估 MoE/Think 版本在方言理解和推理任务上的边际收益。
- 工程风险：0 likes/downloads；模型名中的 2507 和 Think 含义需查模型卡；MoE 部署成本与 serving 兼容性需验证。
- 证据边界：benchmark、上下文长度、训练数据许可、chat template、MoE active parameters、TGI 实际兼容性和推理开销未在候选信息中确认。
- 建议动作：持续观察 —— 先与 8B 版本合并跟踪，待模型卡补足数据或业务需要粤语推理时再实验。
- URL：https://huggingface.co/jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507
