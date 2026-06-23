## 2026-06-24 01:09 北京时间 | 模型发布巡检

本轮依据候选报告的 10 小时 Recency window 筛选，仅写入有 Hugging Face 来源链接、更新时间在窗口内且 priority_hint=P1 的条目；未确认字段均显式标注。

### 1. `wahidmounir/Agents-K1-Q8_0-GGUF`
- 模型名：`wahidmounir/Agents-K1-Q8_0-GGUF`
- 来源：Hugging Face
- 更新时间：2026-06-23T16:01:26Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：InternScience/Agents-K1 的 GGUF Q8_0 量化版本在本轮窗口内更新，标签显示面向 information-extraction、named-entity-recognition、relation-extraction、GRPO/RL、scientific-text/biomedical，并标注 llama-cpp、endpoints_compatible。
- 适用场景：本地/边缘端 Agent 信息抽取、科研/生物医学文本结构化、低运维成本离线推理候选。
- 工程影响：Q8_0 GGUF 对 llama.cpp 路线有直接工程价值，可用于快速验证 Agents-K1 在本地 CPU/GPU 混合部署中的实体/关系抽取能力；Apache-2.0 标签降低二次集成门槛。
- 工程风险：likes/downloads 均为 0，尚无社区验证；量化来源为第三方仓库，需要核对量化质量与上游权重一致性。
- 证据边界：参数量、上下文长度、benchmark、训练数据、chat template、具体推理显存/内存需求未在候选信息中确认；仅候选标签确认 GGUF、llama-cpp、license:apache-2.0。
- 建议动作：今天应实验：若团队已有 llama.cpp/GGUF 评测脚本，可用 5-10 条内部 IE/NER/RE 样例做冒烟测试。
- URL：https://huggingface.co/wahidmounir/Agents-K1-Q8_0-GGUF

### 2. `voidful/barbet-1b-base-agent-sft-tw-fullft`
- 模型名：`voidful/barbet-1b-base-agent-sft-tw-fullft`
- 来源：Hugging Face
- 更新时间：2026-06-23T15:48:56Z
- pipeline：text-generation
- license：other
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理、训练与后训练、模型发布与模型能力
- 核心变化：OpenFormosa/barbet-1b-base 的完整微调 Agent SFT 版本在本轮窗口内更新，标签包含 agent、tool-use、zh-tw、taiwan、custom-code、dataset:voidful/agent-sft。
- 适用场景：繁体中文/台湾语境工具调用、轻量 Agent SFT 对照、中文多轮工具使用数据格式参考。
- 工程影响：1B 级别基础模型的 full-finetune 方向适合低成本 Agent 子任务实验，特别是工具调用格式与繁中语料适配；但 custom-code 标签提示部署时需更严格审查。
- 工程风险：license 标为 other，商用/再分发边界不清；custom-code 需要审计远程代码；likes/downloads 均为 0。
- 证据边界：具体参数量由模型名暗示 1B，但候选字段未单独确认；上下文长度、benchmark、训练细节、chat template、工具调用协议未在候选信息中确认。
- 建议动作：今天应阅读：先读模型卡和 license 说明，未确认授权前不要进入生产候选池。
- URL：https://huggingface.co/voidful/barbet-1b-base-agent-sft-tw-fullft

### 3. `npario/SIQ-1-35B-Q4_K_M-GGUF`
- 模型名：`npario/SIQ-1-35B-Q4_K_M-GGUF`
- 来源：Hugging Face
- 更新时间：2026-06-23T15:36:45Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：AlexWortega/SIQ-1-35B 的 Q4_K_M GGUF 版本在本轮窗口内更新，标签显示 autoresearch、distillation、agentic、coding、agent、moe、tiny、llama-cpp。
- 适用场景：Agentic coding/自动研究子任务、本地 GGUF 评测、蒸馏/MoE 路线观察。
- 工程影响：Q4_K_M GGUF 可能降低 35B 级模型本地试跑成本，适合作为 coding/agentic 小样本 benchmark 的候选；Apache-2.0 标签利于工程 PoC。
- 工程风险：第三方量化仓库且 likes/downloads 为 0；“35B”“MoE/tiny”等标签组合需要核对上游模型定义，避免误判实际激活参数或部署需求。
- 证据边界：参数量仅从模型名/标签推断，未在候选信息中结构化确认；上下文长度、benchmark、量化校准方式、chat template、内存需求未确认。
- 建议动作：今天应实验：可加入本地 GGUF smoke test，但先核对上游 AlexWortega/SIQ-1-35B 模型卡。
- URL：https://huggingface.co/npario/SIQ-1-35B-Q4_K_M-GGUF

### 4. `Lance1573/acrouter-qwen35-08b-router-lora`
- 模型名：`Lance1573/acrouter-qwen35-08b-router-lora`
- 来源：Hugging Face
- 更新时间：2026-06-23T16:12:02Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、评测与基准
- 核心变化：Qwen/Qwen3.5-0.8B 的 router LoRA/PEFT adapter 在本轮窗口内更新，标签包含 model-routing、agent-as-a-router、CodeRouterBench、arxiv:2606.22902。
- 适用场景：多模型路由、Agent 子任务分发、coding 请求分类/路由策略实验。
- 工程影响：路由器 LoRA 比直接部署大模型更适合接入推理网关或 Agent 编排层，可用于“低成本模型选择器”PoC；CodeRouterBench 标签提示其与代码路由评测相关。
- 工程风险：adapter 依赖 Qwen/Qwen3.5-0.8B 基座；候选信息未确认论文内容和评测结果；likes/downloads 为 0，社区信号弱。
- 证据边界：上下文长度、benchmark 数值、训练数据、实际路由标签空间、chat template、与 vLLM/TGI/llama.cpp 的兼容方式未在候选信息中确认。
- 建议动作：今天应阅读：优先读模型卡、arXiv 链接和 CodeRouterBench 数据格式，判断是否能接入现有网关路由评测。
- URL：https://huggingface.co/Lance1573/acrouter-qwen35-08b-router-lora

### 5. `invosmartplay/legal-chatbot-indonesia-qwen-0.5b`
- 模型名：`invosmartplay/legal-chatbot-indonesia-qwen-0.5b`
- 来源：Hugging Face
- 更新时间：2026-06-23T15:40:40Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：RAG 与知识工程、模型发布与模型能力、推理系统与工程工具
- 核心变化：基于 unsloth/Qwen2.5-0.5B-Instruct-bnb-4bit 的印尼法律聊天微调模型在本轮窗口内更新，标签包含 text-generation-inference、unsloth、conversational。
- 适用场景：低成本垂直法律问答、印尼语/法律 RAG 辅助模型、边缘部署可行性观察。
- 工程影响：0.5B 级别低成本模型可用于 RAG pipeline 中的轻量对话层或分类/摘要子任务，TGI/endpoints_compatible 标签对快速服务化有帮助。
- 工程风险：垂直法律场景有高合规/幻觉风险；训练数据和评测未确认；0 likes/downloads 缺少实际采用信号。
- 证据边界：参数量由基座标签/模型名指向 0.5B，但候选未提供独立参数字段；上下文长度、法律数据来源、benchmark、chat template、适用法域边界未确认。
- 建议动作：持续观察：除非有印尼法律场景需求，否则先记录，不进入通用候选池。
- URL：https://huggingface.co/invosmartplay/legal-chatbot-indonesia-qwen-0.5b

### 6. `Xy2509413/Llama-3.3-70B-Instruct-abliterated`
- 模型名：`Xy2509413/Llama-3.3-70B-Instruct-abliterated`
- 来源：Hugging Face
- 更新时间：2026-06-23T16:03:31Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力、推理系统与工程工具
- 核心变化：meta-llama/Llama-3.3-70B-Instruct 的 abliterated/uncensored 派生模型在本轮窗口内更新，标签包含 llama-3、facebook、meta、pytorch、conversational、多语言。
- 适用场景：安全对齐差异分析、拒答机制/安全评测红队对照，不建议作为业务模型直接候选。
- 工程影响：可作为安全评测对照样本，帮助工程团队验证 guardrail、策略层和内容安全网关是否依赖模型自身拒答。
- 工程风险：abliterated/uncensored 明确提示安全约束弱化；license 未在候选信息中确认；70B 部署成本高且无下载/点赞信号。
- 证据边界：license、上下文长度、benchmark、移除/弱化对齐的具体方法、chat template、部署要求未在候选信息中确认。
- 建议动作：暂不跟进：除安全红队/评测用途外，不建议进入工程候选池。
- URL：https://huggingface.co/Xy2509413/Llama-3.3-70B-Instruct-abliterated

### 7. `Fallow21/glasswing-health-assistant-v1`
- 模型名：`Fallow21/glasswing-health-assistant-v1`
- 来源：Hugging Face
- 更新时间：2026-06-23T15:47:52Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：RAG 与知识工程、模型发布与模型能力、推理系统与工程工具
- 核心变化：基于 unsloth/Qwen2.5-1.5B-Instruct-bnb-4bit 的 health assistant 微调模型在本轮窗口内更新，标签包含 text-generation-inference、unsloth、conversational。
- 适用场景：医疗/健康问答原型、RAG 后处理/摘要子任务、低成本垂直助手实验。
- 工程影响：1.5B 级别模型适合做低成本健康问答 PoC 或本地隐私场景的辅助层；TGI/endpoints_compatible 标签有利于快速部署验证。
- 工程风险：医疗健康领域风险高，缺少训练数据/评测/安全边界；likes/downloads 为 0；不能据候选信息判断临床可靠性。
- 证据边界：上下文长度、benchmark、训练数据、医疗免责声明、安全评测、chat template 未在候选信息中确认。
- 建议动作：持续观察：只有在补齐模型卡证据和医学安全评测后才考虑实验。
- URL：https://huggingface.co/Fallow21/glasswing-health-assistant-v1

### 8. `NullVoider/Nex-N2-Pro`
- 模型名：`NullVoider/Nex-N2-Pro`
- 来源：Hugging Face
- 更新时间：2026-06-23T16:57:25Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：多模态与生成媒体、评测与基准、模型发布与模型能力
- 核心变化：带 qwen3_5_moe、image-text-to-text、eval-results 标签的模型在本轮窗口内更新，pipeline 标为 text-generation，并标注 endpoints_compatible。
- 适用场景：多模态/图文到文本能力巡检、MoE 结构观察、评测结果字段核对。
- 工程影响：如果模型卡确认 image-text-to-text 能力，可进入多模态助手和视觉理解 pipeline 的候选；eval-results 标签值得核对是否有可复现实验。
- 工程风险：候选中 pipeline 与 image-text-to-text 标签存在表达不一致；likes/downloads 为 0；模型架构、输入格式和评测细节不明。
- 证据边界：参数量、上下文长度、视觉编码器/输入分辨率、benchmark 数值、chat template、部署框架兼容性未在候选信息中确认。
- 建议动作：今天应阅读：优先核对模型卡中的多模态输入格式和 eval-results 是否真实可用。
- URL：https://huggingface.co/NullVoider/Nex-N2-Pro
