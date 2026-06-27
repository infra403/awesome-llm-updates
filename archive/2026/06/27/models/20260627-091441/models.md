## 2026-06-27 09:14 北京时间 | 模型发布巡检

本次巡检窗口：候选报告标注的最近 10 小时；仅纳入候选列表中带有明确更新时间与来源链接的 P0/P1 条目。未确认字段均按“未在候选信息中确认”处理。

### 1. `InternScience/Agents-A1`

- 来源：Hugging Face
- 更新时间：2026-06-26T22:18:39Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：6 / 3
- 重要性：P0：候选信息显示为 Qwen3.5 MoE 相关、Apache-2.0、text-generation/conversational，并带 image-text-to-text 与 endpoints_compatible 标签，且是本轮唯一 P0。
- 主题标签：模型发布与模型能力、Agent 与多智能体、推理系统与工程工具
- 核心变化：本周期窗口内更新的 Agent 方向模型卡/权重条目；核心变化更接近“Agent 能力模型进入巡检池”，不是热度驱动。
- 适用场景：Agent 子任务、工具调用前的对话/规划模型候选；也可作为 Qwen3.5 MoE 系 Agent 模型卡跟踪对象。
- 工程影响：若权重与模板完整，可能影响 Agent 编排层的开源模型候选、端点部署兼容性和本地/托管推理选型。
- 工程风险：当前 likes/downloads 仍低，工程成熟度未由下载量验证；需要确认模型卡是否给出 chat template、依赖 transformers 版本、显存需求和推理样例。
- 证据边界：参数量、上下文长度、benchmark、训练数据、精确多模态输入格式、chat template 与部署显存未在候选信息中确认；license 仅依据候选标签 license:apache-2.0。
- 建议动作：今天应阅读：P0 且与 Agent 工程选型直接相关，先核验模型卡和最小推理脚本。
- URL：https://huggingface.co/InternScience/Agents-A1

### 2. `Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2`

- 来源：Hugging Face
- 更新时间：2026-06-27T00:25:36Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1：GGUF、llama.cpp、local-llm、coding/math/reasoning/cybersecurity 标签明确指向本地推理与代码任务实验。
- 主题标签：推理系统与工程工具、推理、训练与后训练、模型发布与模型能力
- 核心变化：本周期更新的 Qwen3.5-9B 量化/本地推理条目；候选标签显示 base_model 与 quantized base_model 均为 Qwen/Qwen3.5-9B。
- 适用场景：llama.cpp 本地试跑、代码/数学/安全类提示词回归、小显存或 NPU/边缘推理可行性摸底。
- 工程影响：可能降低 coding/reasoning 类任务的本地实验成本；但需核验 GGUF 文件、量化等级和实际兼容性。
- 工程风险：模型名包含 Claude/Opus 字样但候选证据只确认 Qwen3.5-9B base/quantized 标签，不能据此推断蒸馏来源或能力。
- 证据边界：benchmark、训练/蒸馏数据、NPU2 含义、上下文长度、GGUF 量化位宽与 license 以外的使用限制未在候选信息中确认。
- 建议动作：今天应实验：若团队维护 llama.cpp coding 基线，可先下载小样本跑通；否则持续观察。
- URL：https://huggingface.co/Atomic-Germ/Qwen3.5-9B-Claude-4.8-Opus-NPU2

### 3. `ansulev/NRS_QWEN_MYTHOS_1M`

- 来源：Hugging Face
- 更新时间：2026-06-27T00:58:27Z
- pipeline：text-generation
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1：标签包含 1m-context、tool-use、coding-agent、reasoning、sft，并声明数据集 SKT-NRS/SKT-OMNI-CORPUS-2T，适合长上下文 Agent 候选跟踪。
- 主题标签：Agent 与多智能体、推理、训练与后训练、模型发布与模型能力
- 核心变化：本周期更新的 Qwen3.5-9B 微调条目；候选信息显示 base_model:Qwen/Qwen3.5-9B 与 finetune 标签。
- 适用场景：长上下文工具调用、代码 Agent、多步推理任务的离线评估候选。
- 工程影响：若 1M 上下文与工具调用模板真实可用，可能影响长文档 Agent/RAG 替代链路；但需要强验证。
- 工程风险：0 likes/0 downloads，且 1m-context 属候选标签，未见实际上下文测试证据；“uncensored”等标签也提示需做安全策略评估。
- 证据边界：license、实际最大上下文、RoPE/推理配置、benchmark、chat template、工具调用格式、训练数据细节未在候选信息中确认。
- 建议动作：今天应阅读：优先核验模型卡是否提供 1M 上下文配置和 tool-use 样例；未确认前不要进入生产候选池。
- URL：https://huggingface.co/ansulev/NRS_QWEN_MYTHOS_1M

### 4. `havok2/Qwen-AgentWorld-35B-A3B-VL36`

- 来源：Hugging Face
- 更新时间：2026-06-26T20:35:04Z
- pipeline：image-text-to-text
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1：标签显示 Qwen-AgentWorld-35B-A3B 与 Qwen3.6-35B-A3B merge/vision-graft，pipeline 为 image-text-to-text，指向多模态 Agent 实验。
- 主题标签：Agent 与多智能体、多模态与生成媒体、模型发布与模型能力
- 核心变化：本周期更新的多模态/视觉嫁接合并模型条目；更像 merge/vision-graft 版本而非全新基础模型。
- 适用场景：视觉问答 Agent、UI/网页截图理解、多模态工具链 smoke test。
- 工程影响：若视觉 graft 可用，可能扩展 AgentWorld 系列在视觉任务中的本地实验面；对多模态部署栈有跟踪价值。
- 工程风险：merge/graft 模型常见风险是投影层、processor、chat template 与基础模型版本不一致；当前无下载与评测反馈。
- 证据边界：参数量、视觉编码器来源、输入分辨率、benchmark、上下文长度、推理框架兼容性和显存需求未在候选信息中确认；license 仅依据 apache-2.0 标签。
- 建议动作：持续观察：多模态 Agent 方向重要，但先等模型卡/样例或社区验证。
- URL：https://huggingface.co/havok2/Qwen-AgentWorld-35B-A3B-VL36

### 5. `shatu/Qwen3-8B-Reasoning-Fix`

- 来源：Hugging Face
- 更新时间：2026-06-26T23:28:49Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1：Qwen3-8B-Base finetune，标签含 reasoning 与 text-generation-inference，适合作为小模型推理修复候选。
- 主题标签：推理、训练与后训练、评测与基准、模型发布与模型能力
- 核心变化：本周期更新的 Qwen3-8B reasoning-fix 微调版本。
- 适用场景：小参数推理提示词回归、TGI 部署 smoke test、reasoning 数据集微调效果对比。
- 工程影响：如果修复特定 reasoning 退化，可影响 8B 级低成本推理服务；但需自建 benchmark 复核。
- 工程风险：未提供候选层面的 benchmark 和具体 fix 内容；0 likes/0 downloads，采用前应避免只凭名称判断。
- 证据边界：修复目标、训练数据、评测分数、上下文长度、chat template、显存需求未在候选信息中确认；license 依据候选标签。
- 建议动作：持续观察：先阅读模型卡；只有发现明确修复说明和可复现实验时再今天实验。
- URL：https://huggingface.co/shatu/Qwen3-8B-Reasoning-Fix

### 6. `issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf`

- 来源：Hugging Face
- 更新时间：2026-06-27T00:41:20Z
- pipeline：未在候选信息中确认
- license：未在候选信息中确认
- likes/downloads：0 / 0
- 重要性：P1：模型名与标签显示 coding-agent 与 GGUF，适合本地 coding Agent 轻量部署试探。
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：本周期更新的 coding-agent GGUF 版本；可能是同名 safetensors 条目的本地推理格式。
- 适用场景：llama.cpp/本地 Agent worker、代码补全或代码修改子任务的快速 smoke test。
- 工程影响：若 GGUF 文件结构完整，可降低 coding Agent 试验门槛；也方便与非 GGUF 版本做质量/速度对比。
- 工程风险：候选信息缺少 pipeline、license、base_model 与量化位宽；0 下载导致可用性未验证。
- 证据边界：参数量、基础模型、license、量化等级、benchmark、chat template、上下文长度和推理命令未在候选信息中确认。
- 建议动作：今天应阅读：先确认模型卡和文件列表；license 不明前暂不进入工程候选池。
- URL：https://huggingface.co/issdandavis/scbe-coding-agent-vtc-qwen15-v1-gguf

### 7. `maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx`

- 来源：Hugging Face
- 更新时间：2026-06-26T23:54:55Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1：Qwen-AgentWorld-35B-A3B quantized，标签含 NVFP4、Blackwell、modelopt、8-bit，指向新硬件/量化部署实验。
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：本周期更新的 AgentWorld 量化版本，候选标签明确 base_model:quantized:Qwen/Qwen-AgentWorld-35B-A3B。
- 适用场景：Blackwell/DGX 或支持 NVFP4 路线的推理栈验证，AgentWorld 模型低成本部署探索。
- 工程影响：可能影响 35B-A3B MoE Agent 模型在高端 GPU 上的吞吐/显存方案；对推理系统工程有价值。
- 工程风险：NVFP4/8-bit 标签与实际运行框架、kernel 支持强相关；若没有 Blackwell 环境，短期不可复现。
- 证据边界：量化精度、实际显存、吞吐、benchmark、上下文长度、vLLM/TensorRT-LLM 兼容性未在候选信息中确认；license 依据候选标签。
- 建议动作：持续观察：有 Blackwell/DGX 资源时今天实验；否则记录为硬件相关候选。
- URL：https://huggingface.co/maltsevis/Qwen-AgentWorld-Heretic-HCl-NVFP4-dgx

### 8. `olka-fi/Ornith-1.0-397B-MXFP4`

- 来源：Hugging Face
- 更新时间：2026-06-27T00:38:52Z
- pipeline：text-generation
- license：mit
- likes/downloads：0 / 0
- 重要性：P1：397B base 的 MXFP4/compressed-tensors/quantized/vllm 条目，MIT 标签，对超大模型量化服务有工程观察价值。
- 主题标签：推理系统与工程工具、模型发布与模型能力、推理、训练与后训练
- 核心变化：本周期更新的 Ornith-1.0-397B 量化版本；候选显示 base_model:deepreinforce-ai/Ornith-1.0-397B 与 quantized 标签。
- 适用场景：vLLM 超大 MoE/稀疏模型部署评估、compressed-tensors/MXFP4 支持验证。
- 工程影响：如文件和配置完整，可能为 397B 级模型提供更低显存服务路径；但属于高资源门槛候选。
- 工程风险：actionability_needs_validation，且无下载/点赞；397B 规模来自模型名与 base_model 字段，实际架构和可运行性需核验。
- 证据边界：benchmark、真实参数/激活专家、上下文长度、硬件需求、vLLM 版本、chat template、训练数据未在候选信息中确认；license 依据 MIT 标签。
- 建议动作：今天应阅读：重点看 README、config 与 vLLM 加载说明；没有硬件资源则暂不实验。
- URL：https://huggingface.co/olka-fi/Ornith-1.0-397B-MXFP4

### 9. `migtissera/GLM-5.2`

- 来源：Hugging Face
- 更新时间：2026-06-26T23:50:47Z
- pipeline：text-generation
- license：mit
- likes/downloads：0 / 0
- 重要性：P1：GLM MoE DSA 相关标签、MIT、eval-results，且同窗口另有 fzjss/GLM-5.2 近似条目，值得关注模型卡变化。
- 主题标签：模型发布与模型能力、评测与基准、推理、训练与后训练
- 核心变化：本周期更新的 GLM-5.2 模型卡/权重条目；候选信息显示 eval-results 与中英 conversational 标签。
- 适用场景：中英对话模型卡跟踪、评测结果核验、GLM 系 MoE/DSA 架构候选观察。
- 工程影响：若 eval-results 可复现，可能影响中文/英文通用模型评测池；MIT 标签利于工程采用前的许可评估。
- 工程风险：第三方上传者与同名重复条目并存，需要核验来源权威性、权重完整性和评测可信度。
- 证据边界：参数量、上下文长度、benchmark 具体数值、训练数据、官方/非官方关系、chat template、部署要求未在候选信息中确认；license 依据 MIT 标签。
- 建议动作：今天应阅读：先核验模型卡来源和 eval-results；不建议未经验证直接实验。
- URL：https://huggingface.co/migtissera/GLM-5.2

### 10. `somosnlp-hackathon-2026/mombeu-LFM2.5-350M`

- 来源：Hugging Face
- 更新时间：2026-06-26T22:54:24Z
- pipeline：text-generation
- license：apache-2.0
- likes/downloads：0 / 0
- 重要性：P1：LFM2.5-350M 的文化对齐微调，标签含 Paraguayan culture、Guarani、DPO/SFT 和公开数据集，适合低资源语言/文化对齐观察。
- 主题标签：数据集与数据工程、模型发布与模型能力、RAG 与知识工程
- 核心变化：本周期更新的小模型文化对齐微调版本；base_model 为 LiquidAI/LFM2.5-350M。
- 适用场景：低资源语言（es/gn）RAG 答案风格、文化对齐评测、小模型 DPO/SFT 数据流程参考。
- 工程影响：对主流 LLM 部署影响有限，但对多语言 RAG、地域文化合规和小模型后训练有参考价值。
- 工程风险：350M 级模型能力边界较小，且下载/点赞为 0；需关注是否只是 hackathon 原型。
- 证据边界：benchmark、上下文长度、训练细节、chat template、实际 Guarani 能力和部署性能未在候选信息中确认；license 依据 apache-2.0 标签。
- 建议动作：持续观察：除非当前有低资源语言/RAG 需求，否则暂不跟进实验。
- URL：https://huggingface.co/somosnlp-hackathon-2026/mombeu-LFM2.5-350M
