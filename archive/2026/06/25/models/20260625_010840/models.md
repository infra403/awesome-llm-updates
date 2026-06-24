## 2026-06-25 01:08 北京时间 | 模型发布巡检

本次仅纳入候选报告标记为 10 小时巡检窗口内更新、且具备 Hugging Face 来源链接与工程相关 reason_codes 的 P0/P1 条目；未用低证据条目补数。

### 1. ivgranite/Qwen-AgentWorld-35B-A3B-GGUF
- 来源：Hugging Face
- 更新时间：2026-06-24T16:49:24.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：1 / 0
- 重要性：P0
- 主题标签：模型发布与模型能力；Agent 与多智能体；推理系统与工程工具
- 核心变化：Qwen/Qwen-AgentWorld-35B-A3B 的 GGUF 量化版本进入本窗口；标签显示 world-model、agent、environment-simulation、conversational，并关联 arxiv:2606.24597。
- 适用场景：本地 llama.cpp/GGUF 评估 Agent 环境模拟、工具调用前的子任务规划、低成本离线实验。
- 工程影响：如果基座 AgentWorld 能力成立，GGUF 版本可降低本地推理门槛，便于工程团队在不部署完整 Transformers 服务的情况下做 Agent 行为回放和环境模拟 sanity check。
- 工程风险：下载量为 0，社区验证不足；量化质量、具体量化档位、chat template 与 function/tool calling 兼容性需实测。
- 证据边界：参数量从模型名可见为 35B-A3B，但候选信息未确认激活参数、上下文长度、benchmark、训练数据、具体 GGUF 文件列表、推理速度与显存/内存需求；license 仅按候选标签记录为 apache-2.0。
- 建议动作：今天应实验——优先拉取一个小体积量化档位，用既有 AgentWorldBench/内部 Agent 回放任务做 smoke test。
- URL：https://huggingface.co/ivgranite/Qwen-AgentWorld-35B-A3B-GGUF

### 2. mradermacher/Fabliq-8B-Agent-FromBase-GGUF
- 来源：Hugging Face
- 更新时间：2026-06-24T16:02:55.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0 / 12
- 重要性：P0
- 主题标签：模型发布与模型能力；Agent 与多智能体；推理、训练与后训练；推理系统与工程工具
- 核心变化：LLM-OS-Models/Fabliq-8B-Agent-FromBase 的 GGUF 量化版本；标签显示 liquid-ai、moe、agentic、terminal、fable-5、distillation、sft、ablation。
- 适用场景：终端 Agent、脚本执行助手、8B 级本地 agentic 模型候选，以及 FromBase/SFT 路线的消融对照。
- 工程影响：相较 35B 级 AgentWorld，8B GGUF 更适合快速部署到开发机或边缘节点，12 downloads 在本窗口内说明已有少量实际拉取。
- 工程风险：无 likes，热度证据弱；“FromBase”暗示可能不是最终 reasoning 版本，真实工具调用稳定性、终端安全边界与幻觉率需评测。
- 证据边界：参数量仅从名称推断为 8B；上下文长度、benchmark、训练数据细节、chat template、具体 GGUF 量化档位和 Liquid/MoE 推理兼容要求未在候选信息中确认；license 仅按候选标签记录为 apache-2.0。
- 建议动作：今天应实验——用本地 terminal-agent 任务集跑最小回归，重点看命令生成可控性与失败恢复能力。
- URL：https://huggingface.co/mradermacher/Fabliq-8B-Agent-FromBase-GGUF

### 3. mradermacher/Fabliq-8B-Agent-Reasoning-i1-GGUF
- 来源：Hugging Face
- 更新时间：2026-06-24T15:40:11.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体；推理、训练与后训练；推理系统与工程工具
- 核心变化：Fabliq-8B-Agent-Reasoning 的 i1/GGUF 量化版本；标签包含 tool-use、terminal、reasoning、distillation、sft。
- 适用场景：Agent reasoning 子任务、工具使用链路、终端操作的推理型小模型备选。
- 工程影响：可与 FromBase-GGUF 做 A/B，对比 reasoning SFT 是否改善多步命令规划、工具选择和错误解释。
- 工程风险：当前 likes/downloads 均为 0，缺少外部验证；i1 量化/校准含义、性能损失与 prompt 格式需确认。
- 证据边界：上下文长度、benchmark、训练数据、tool schema 支持方式、chat template、推理框架版本要求未在候选信息中确认；license 仅按候选标签记录为 apache-2.0。
- 建议动作：今天应实验——如果已有 Fabliq FromBase 测试脚本，应同步纳入 reasoning 版本做同题对照；否则持续观察。
- URL：https://huggingface.co/mradermacher/Fabliq-8B-Agent-Reasoning-i1-GGUF

### 4. jedisct1/Qwen-AgentWorld-35B-A3B-oQ8-MLX
- 来源：Hugging Face
- 更新时间：2026-06-24T14:01:20.000Z
- pipeline：未在候选信息中确认
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；Agent 与多智能体；推理系统与工程工具
- 核心变化：Qwen-AgentWorld-35B-A3B 的 MLX 8-bit 量化版本；标签包含 mlx、omlx、lm-studio、qwen、tool-calling。
- 适用场景：Apple Silicon/MLX 本地评测、LM Studio 桌面环境验证 AgentWorld tool-calling 行为。
- 工程影响：为 Mac 开发者提供比 GGUF 路线更贴近 MLX 的测试路径，可能降低 AgentWorld 在个人开发机上的试用成本。
- 工程风险：社区使用信号为 0；oQ8 的量化质量、MLX 版本兼容性和 tool-calling template 需要实际加载确认。
- 证据边界：上下文长度、benchmark、显存/统一内存需求、训练数据、chat template、工具调用格式未在候选信息中确认；license 仅按候选标签记录为 apache-2.0。
- 建议动作：持续观察——Mac/MLX 栈用户可列入候选池，但在出现下载或模型卡细节前不宜默认采用。
- URL：https://huggingface.co/jedisct1/Qwen-AgentWorld-35B-A3B-oQ8-MLX

### 5. lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4
- 来源：Hugging Face
- 更新时间：2026-06-24T16:28:25.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；Agent 与多智能体；推理系统与工程工具；评测与基准
- 核心变化：Qwen-AgentWorld-35B-A3B 的 NVFP4/compressed-tensors 版本；标签显示 dataset:Qwen/AgentWorldBench、arxiv:2606.24597、world-model、environment-simulation。
- 适用场景：Blackwell/NVFP4 或支持 compressed-tensors 的推理栈预研，AgentWorldBench 相关评测复现。
- 工程影响：若部署栈支持 NVFP4，可显著影响 35B-A3B 类 Agent 模型的显存成本和吞吐评估，是比通用 GGUF 更偏数据中心推理优化的候选。
- 工程风险：候选标签同时出现 image-text-to-text 与 text-generation，模态能力边界不清；NVFP4 依赖硬件/框架支持，当前 likes/downloads 为 0。
- 证据边界：上下文长度、benchmark、实际多模态能力、训练数据、chat template、vLLM/Transformers 精确版本要求未在候选信息中确认；license 仅按候选标签记录为 apache-2.0。
- 建议动作：今天应阅读——先核对模型卡的 compressed-tensors 加载方式和硬件要求，再决定是否进入实验队列。
- URL：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-NVFP4

### 6. sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4
- 来源：Hugging Face
- 更新时间：2026-06-24T14:26:44.000Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；推理、训练与后训练；推理系统与工程工具
- 核心变化：llm-jp/llm-jp-4-32b-a3b-thinking 的 NVFP4/W4A4 compressed-tensors 量化版本；标签包含 qwen3_moe、vllm、moe、reasoning、thinking、japanese、blackwell。
- 适用场景：日英双语 reasoning、日语 Agent/RAG 子任务、Blackwell 上的 W4A4/vLLM 推理预研。
- 工程影响：对需要日语推理能力和低比特数据中心部署的团队有候选价值，尤其适合验证 vLLM + compressed-tensors 路线。
- 工程风险：无下载/点赞；NVFP4/Blackwell 适配门槛高，非目标硬件上可用性有限。
- 证据边界：参数量从名称可见 32b-a3b，但候选信息未确认上下文长度、benchmark、训练数据、chat template、实际 vLLM 版本和显存需求；license 仅按候选标签记录为 apache-2.0。
- 建议动作：持续观察——有日语/Blackwell 需求的团队可建卡跟踪，否则暂不投入实验资源。
- URL：https://huggingface.co/sakamakismile/llm-jp-4-32b-a3b-thinking-NVFP4

### 7. ermiaazarkhalili/Gemma4-E4B-SFT-Claude-Opus-Reasoning-Unsloth-GGUF
- 来源：Hugging Face
- 更新时间：2026-06-24T16:52:05.000Z
- pipeline：text-generation
- license：gemma
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；推理、训练与后训练；推理系统与工程工具
- 核心变化：Gemma4-E4B-SFT-Claude-Opus-Reasoning-Unsloth 的 GGUF/llama.cpp 量化版本；标签包含 reasoning、unsloth、dataset:ermiaazarkhalili/claude-reasoning-distillation。
- 适用场景：小模型 reasoning 蒸馏效果验证、本地 llama.cpp 快速试跑、Gemma license 下的实验候选。
- 工程影响：E4B 级别如可用，可能成为低成本 reasoning 子任务模型；GGUF 版本便于本地评估而无需完整训练框架。
- 工程风险：蒸馏自 Claude Opus reasoning 的合规/数据来源需额外审查；Gemma license 对商业使用边界需法务确认。
- 证据边界：候选信息未确认上下文长度、benchmark、训练样本质量、chat template、具体 GGUF 量化档位和推理资源需求；license 仅按候选标签记录为 gemma。
- 建议动作：今天应阅读——先审模型卡和数据集说明，确认数据/许可证风险后再实验。
- URL：https://huggingface.co/ermiaazarkhalili/Gemma4-E4B-SFT-Claude-Opus-Reasoning-Unsloth-GGUF

### 8. leonsarmiento/Nex-N2-mini-5bit-text-mlx
- 来源：Hugging Face
- 更新时间：2026-06-24T16:53:36.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；Agent 与多智能体；推理系统与工程工具
- 核心变化：nex-agi/Nex-N2-mini 的 MLX 5-bit text 量化版本；标签包含 qwen3_5_moe、mlx-lm、moe、agentic、conversational。
- 适用场景：Apple Silicon 上的轻量 agentic/对话模型试用，Nex-N2-mini 系列本地开发机验证。
- 工程影响：5-bit MLX 版本可能降低 Mac 本地推理成本，适合做 Agent 子任务、对话路由或提示词回归的轻量候选。
- 工程风险：license 未确认，无法直接进入商业候选；无下载/点赞，模型卡信息需补齐。
- 证据边界：候选信息未确认 license、参数量、上下文长度、benchmark、训练数据、chat template、量化误差和 MLX 版本要求。
- 建议动作：持续观察——在 license 明确前仅可作为技术预研条目，不建议进入生产候选池。
- URL：https://huggingface.co/leonsarmiento/Nex-N2-mini-5bit-text-mlx

### 9. micymike/CodeMate-Qwen-1.5B-32K-Distilled-on-Claude-Fable-5
- 来源：Hugging Face
- 更新时间：2026-06-24T16:43:26.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；推理、训练与后训练；推理系统与工程工具
- 核心变化：Qwen2 系列 1.5B、32K、面向 CodeMate 的蒸馏模型；标签包含 text-generation-inference、conversational、Distilled-on-Claude-Fable-5。
- 适用场景：低成本 coding assistant、长上下文代码摘要/补全前处理、TGI 部署烟测。
- 工程影响：如果 32K 上下文属实，小参数模型可用于代码检索后压缩、CI 日志摘要和 coding agent 的廉价辅助环节。
- 工程风险：license 未确认，蒸馏来源与代码能力 benchmark 未给出；1.5B 模型在复杂 coding 任务上可能能力不足。
- 证据边界：32K 来自模型名而非候选结构化字段；候选信息未确认 license、benchmark、训练数据、真实上下文长度、chat template 与 TGI 版本要求。
- 建议动作：持续观察——等 license/模型卡补全后，可用内部代码摘要集做小规模验证。
- URL：https://huggingface.co/micymike/CodeMate-Qwen-1.5B-32K-Distilled-on-Claude-Fable-5

### 10. HaimingW/qwen2.5-1.5b-faithful-summarization
- 来源：Hugging Face
- 更新时间：2026-06-24T16:43:10.000Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：模型发布与模型能力；RAG 与知识工程；推理、训练与后训练
- 核心变化：基于 Qwen/Qwen2.5-1.5B 的 faithful summarization 微调版本；标签包含 base_model:finetune、text-generation-inference、conversational。
- 适用场景：RAG 摘要、文档压缩、答案忠实性对照、小模型 summarization pipeline。
- 工程影响：面向“faithful summarization”的 1.5B 微调模型可能降低 RAG 后处理成本，适合作为长文档摘要链路的候选 rerun 模型。
- 工程风险：无社区热度；faithfulness 需要任务内评测，不能仅凭名称进入生产；license 未确认。
- 证据边界：候选信息未确认 license、上下文长度、benchmark、训练数据、忠实性评测方法、chat template 与 TGI 版本要求。
- 建议动作：持续观察——先等待模型卡补齐，若有摘要评测集可做离线对照实验。
- URL：https://huggingface.co/HaimingW/qwen2.5-1.5b-faithful-summarization
