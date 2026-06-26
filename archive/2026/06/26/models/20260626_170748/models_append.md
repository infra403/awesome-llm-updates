## 2026-06-26 17:07 北京时间 | 模型发布巡检

本次依据候选报告的 10 小时巡检窗口筛选；只写入候选信息或 Hugging Face API 可确认更新时间的 P0/P1 条目。未确认字段按“未在候选信息中确认”处理。

### 1. `zenlm/zen-agent-4b`

- 来源：Hugging Face
- 更新时间：2026-06-26T08:58:30.000Z
- pipeline：text-generation
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：1 / 250
- 重要性：P0
- 主题标签：模型发布与模型能力、Agent 与多智能体、推理系统与工程工具
- 核心变化：Agent 向文本生成模型条目进入本周期窗口，标签包含 qwen3、agent、function-calling、tool-use、conversational、GGUF、text-generation-inference、endpoints_compatible。
- 适用场景：Agent 子任务、函数调用/工具调用实验、轻量本地或端点推理候选。
- 工程影响：值得进入工程候选池；4B 级别名称与工具调用标签使其适合低成本 Agent 路由、边缘侧原型和 TGI/Endpoint 兼容性检查。
- 工程风险：候选信息未给出实际工具调用评测、对齐策略、失败案例、上下文长度或 chat template；GGUF 标签存在，但具体量化文件和 llama.cpp 兼容矩阵未在候选信息中确认。
- 证据边界：参数量仅由模型名暗示；benchmark、训练数据、上下文长度、系统提示格式、函数调用 schema 支持程度未在候选信息中确认。
- 建议动作：今天应阅读；理由是 P0、Apache-2.0、function-calling/tool-use 标签和 250 downloads 已具备工程试读价值。
- URL：https://huggingface.co/zenlm/zen-agent-4b

### 2. `zenlm/zen-eco-4b-agent-gguf`

- 来源：Hugging Face
- 更新时间：2026-06-26T08:58:18.000Z
- pipeline：text-generation
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：0 / 684
- 重要性：P0
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：`zenlm/zen-agent-4b` 的 GGUF/quantized 版本进入窗口；标签含 gguf、base_model:zenlm/zen-agent-4b、base_model:quantized:zenlm/zen-agent-4b、endpoints_compatible。
- 适用场景：llama.cpp/GGUF 本地推理、低成本 Agent worker、离线工具调用实验。
- 工程影响：值得进入工程候选池；在候选中 downloads 最高（684），比原始模型更偏部署落地，适合优先验证本地吞吐、显存/内存占用和质量损失。
- 工程风险：具体 GGUF 量化等级、文件大小、推荐运行参数、模板兼容性未在候选信息中确认。
- 证据边界：benchmark、上下文长度、函数调用可靠性、训练数据、推理框架实际版本兼容未在候选信息中确认。
- 建议动作：今天应实验；理由是下载量较高且直接影响本地部署成本。
- URL：https://huggingface.co/zenlm/zen-eco-4b-agent-gguf

### 3. `zenlm/zen-vl-30b-agent`

- 来源：Hugging Face
- 更新时间：2026-06-26T08:57:49.000Z
- pipeline：image-text-to-text
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：0 / 40
- 重要性：P0
- 主题标签：多模态与生成媒体、Agent 与多智能体、模型发布与模型能力
- 核心变化：视觉语言 Agent 模型进入窗口；标签包含 qwen3_vl_moe、vision-language、multimodal、function-calling、visual-agents、multilingual。
- 适用场景：视觉 Agent、图文理解任务、UI/截图分析、多模态工具调用原型。
- 工程影响：值得进入工程候选池；如果模型卡后续确认工具调用/视觉规划能力，可作为多模态 Agent 路由的中高能力候选。
- 工程风险：30B 规模由模型名体现，实际参数/激活参数、显存需求和 MoE 路由成本未在候选信息中确认；当前 downloads 仅 40，热度证据仍弱。
- 证据边界：benchmark、上下文长度、图像分辨率限制、OCR/定位能力、训练数据、chat template 未在候选信息中确认。
- 建议动作：今天应阅读；理由是 P0 且覆盖多模态 Agent，但先读模型卡确认部署要求再实验。
- URL：https://huggingface.co/zenlm/zen-vl-30b-agent

### 4. `zenlm/zen-vl-8b-agent`

- 来源：Hugging Face
- 更新时间：2026-06-26T08:58:00.000Z
- pipeline：image-text-to-text
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：1 / 39
- 重要性：P0
- 主题标签：多模态与生成媒体、Agent 与多智能体、推理系统与工程工具
- 核心变化：8B 视觉语言 Agent 模型进入窗口；标签包含 qwen3_vl、vision-language、multimodal、agent、conversational、endpoints_compatible。
- 适用场景：中小规模 VLM Agent、截图问答、文档图片理解、低成本多模态评测集跑分。
- 工程影响：值得进入工程候选池；相较 30B 条目，8B 名称暗示更容易进入单卡/低成本验证，适合做多模态 Agent 的成本基线。
- 工程风险：未确认具体参数量、显存需求、图像 token 策略、函数调用能力；候选只确认标签和基础热度。
- 证据边界：benchmark、上下文长度、训练数据、chat template、图像分辨率上限未在候选信息中确认。
- 建议动作：今天应实验；理由是 P0 且工程成本可能低于 30B，多模态 Agent 评测可先从该模型开始。
- URL：https://huggingface.co/zenlm/zen-vl-8b-agent

### 5. `zenlm/zen-vl-4b-agent`

- 来源：Hugging Face
- 更新时间：2026-06-26T08:58:34.000Z
- pipeline：image-text-to-text
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：0 / 39
- 重要性：P0
- 主题标签：多模态与生成媒体、Agent 与多智能体、推理系统与工程工具
- 核心变化：4B 视觉语言 Agent 模型进入窗口；标签包含 qwen3_vl、vision-language、multimodal、conversational、endpoints_compatible。
- 适用场景：低成本视觉问答、边缘侧多模态 Agent、截图分类/路由预处理。
- 工程影响：值得进入工程候选池；对需要低延迟或低显存的视觉 Agent worker 有潜在价值，可与 8B/30B 做成本-质量分层。
- 工程风险：未确认工具调用标签；实际视觉能力、幻觉率、OCR 能力和模板兼容性未知。
- 证据边界：参数量由名称暗示；benchmark、上下文长度、训练数据、license 以 cardData/标签确认但使用限制细节未展开。
- 建议动作：持续观察；理由是 P0 但热度和能力证据较少，适合等模型卡补充后进入实验。
- URL：https://huggingface.co/zenlm/zen-vl-4b-agent

### 6. `zenlm/zen-eco-4b-agent-mlx`

- 来源：Hugging Face
- 更新时间：2026-06-26T08:58:04.000Z
- pipeline：text-generation
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：0 / 69
- 重要性：P0
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：`zenlm/zen-agent-4b` 的 MLX/4-bit 量化版本进入窗口；标签包含 mlx、base_model:zenlm/zen-agent-4b、base_model:quantized、4-bit。
- 适用场景：Apple Silicon 本地推理、Mac 端 Agent worker、离线开发环境中的工具调用模型。
- 工程影响：值得进入工程候选池；MLX 版本降低 Mac 本地验证门槛，可补齐 GGUF 之外的 Apple 生态部署路径。
- 工程风险：未确认具体 MLX 版本、量化方法、prompt/chat template、函数调用兼容性；downloads 低于 GGUF 版本。
- 证据边界：benchmark、上下文长度、训练数据、工具调用评测和推荐运行参数未在候选信息中确认。
- 建议动作：今天应实验；理由是对 Mac 本地 Agent 工程链路有直接部署价值。
- URL：https://huggingface.co/zenlm/zen-eco-4b-agent-mlx

### 7. `dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-gguf`

- 来源：Hugging Face
- 更新时间：2026-06-26T06:29:34.000Z
- pipeline：text-generation
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、推理、训练与后训练
- 核心变化：基于 `Qwen/Qwen3.6-35B-A3B` 的 GGUF/quantized Agent-Coding 版本进入窗口；标签包含 llama.cpp、gguf、moe、coding、agent、tool-use、heretic、refusal-reduced。
- 适用场景：本地 coding Agent、工具调用、拒答降低策略对比、MoE 量化部署实验。
- 工程影响：可进入工程候选池但需谨慎；它覆盖 coding + agent + tool-use + GGUF，适合做本地代码 Agent 的“能力上限/风险”对照组。
- 工程风险：`heretic`、`refusal-reduced` 标签暗示安全/拒答策略有调整，企业环境需要额外安全评估；当前 likes/downloads 为 0，缺少社区验证。
- 证据边界：Qwen3.6 基座、35B-A3B 和 Apache-2.0 由标签/cardData 确认；benchmark、上下文长度、量化等级、训练/后训练方法未在候选信息中确认。
- 建议动作：持续观察；理由是工程方向明确但下载/评测证据不足，先记录并等待模型卡或社区反馈。
- URL：https://huggingface.co/dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-gguf

### 8. `dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-mlx-oq`

- 来源：Hugging Face
- 更新时间：2026-06-26T06:29:34.000Z
- pipeline：text-generation
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、推理、训练与后训练
- 核心变化：同一 Qwen3.6-35B-A3B Agent/Coding 分支的 MLX/OQ/8-bit 量化版本进入窗口；标签包含 mlx、oq、8-bit、coding、agent、tool-use、refusal-reduced。
- 适用场景：Apple Silicon 上的 coding Agent、MLX 量化部署对照、与 GGUF 版本做速度/质量比较。
- 工程影响：可进入工程候选池但优先级低于已有热度条目；它为 Mac 本地 MoE Agent 实验提供部署路径。
- 工程风险：0 downloads/0 likes，且 refusal-reduced 标签需要安全边界验证；具体 OQ 量化含义和运行要求未在候选信息中确认。
- 证据边界：benchmark、上下文长度、训练数据、chat template、工具调用 schema 支持未在候选信息中确认。
- 建议动作：持续观察；理由是部署方向有价值，但缺少热度和能力证据。
- URL：https://huggingface.co/dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-mlx-oq

### 9. `hardikchadda/hatch-agent-qwen2.5-1.5b`

- 来源：Hugging Face
- 更新时间：2026-06-26T06:53:14.000Z
- pipeline：text-generation
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：0 / 0
- 重要性：P1
- 主题标签：Agent 与多智能体、推理系统与工程工具、模型发布与模型能力
- 核心变化：基于 `Qwen/Qwen2.5-1.5B-Instruct` 的 GGUF/quantized 边缘 Agent 模型进入窗口；标签含 arduino、arduino-uno-q、edge-ai、on-device、tinyml、function-calling、llama.cpp。
- 适用场景：极低资源设备、Arduino/边缘 AI 原型、TinyML 函数调用实验。
- 工程影响：值得进入工程候选池中的边缘专项；虽然热度为 0，但“on-device + function-calling + GGUF”组合对设备侧 Agent 有差异化价值。
- 工程风险：未确认能否在目标 Arduino 硬件上实际运行，未确认量化等级、内存占用、响应延迟和函数调用可靠性。
- 证据边界：参数量与基座由名称/标签确认；benchmark、上下文长度、训练数据、部署脚本、硬件兼容矩阵未在候选信息中确认。
- 建议动作：今天应阅读；理由是边缘 Agent 方向稀缺，应先确认模型卡部署说明。
- URL：https://huggingface.co/hardikchadda/hatch-agent-qwen2.5-1.5b

### 10. `nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF`

- 来源：Hugging Face
- 更新时间：候选报告为 2026-06-26T08:28:37.000Z；Hugging Face API 回查为 2026-06-26T08:41:24.000Z
- pipeline：text-generation
- license：apache-2.0（候选标签与 cardData 确认）
- likes/downloads：2 / 0
- 重要性：P1
- 主题标签：推理、训练与后训练、推理系统与工程工具、评测与基准
- 核心变化：基于 `Qwen/Qwen3.6-35B-A3B` 的 Thinking Distill GGUF/quantized 条目进入窗口；标签包含 reasoning、distillation、mtp、imatrix、moe、llama.cpp。
- 适用场景：本地推理模型评测、reasoning distill 对照、GGUF 量化质量/速度评估。
- 工程影响：可进入工程候选池的评测/对照组；若目标是本地 reasoning，`imatrix`/GGUF 标签让它适合与其他 Qwen3.6 量化版本比较。
- 工程风险：actionability_needs_validation；0 downloads 说明尚无下载证据，且 DSV4Pro/Thinking Distill 的来源和训练细节未在候选信息中确认。
- 证据边界：benchmark、上下文长度、训练数据、蒸馏教师、量化等级、推荐 llama.cpp 参数未在候选信息中确认。
- 建议动作：持续观察；理由是 reasoning/quantized 方向相关，但需要模型卡和最小评测验证后再实验。
- URL：https://huggingface.co/nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF
