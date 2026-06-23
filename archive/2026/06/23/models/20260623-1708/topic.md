## 2026-06-23 17:08 模型发布主题条目

### 模型发布与模型能力

- osmapi/osmQwopus3.6-27B-Fable-Agentic（P0）：适合场景：Agent 子任务、工具调用/函数调用 SFT 候选、推理轨迹数据蒸馏对比；风险：AGPL-3.0、下载为 0、函数调用格式兼容性未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic
- parth-1/metaguard-policy-agent-v1（P0）：适合场景：策略/安全策略 Agent、轻量 guard/policy routing、TGI 部署候选；风险：真实 base model、任务 schema、误判率未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/parth-1/metaguard-policy-agent-v1
- voidful/gemma-4-e4b-it-agent-sft-tw（P0）：适合场景：繁中 Agent 指令跟随、中文评测集对齐；风险：Gemma license、pipeline、评测分数未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/voidful/gemma-4-e4b-it-agent-sft-tw
- arizal/qwen2.5-1.5b-legal-sft（P1）：适合场景：法律 RAG 的答案风格微调、小模型边缘部署；风险：法律数据来源/法域和可靠性评测未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/arizal/qwen2.5-1.5b-legal-sft
- waynehwang/multimodal_sport_gemma3（P1）：适合场景：体育图文理解、韩语多模态问答；风险：数据集规模和跨语言泛化未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/waynehwang/multimodal_sport_gemma3
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4（P1）：适合场景：Mac 本地多模态推理、MLX-VLM FP4 低内存实验；风险：license 未确认且名称含 uncensored；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit（P1）：适合场景：Mac 本地多模态推理、8bit 与 FP4 质量/速度对比；风险：license、显存/内存占用、MLX 版本要求未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit
- waynehwang/multimodal_sport_gemma3_gguf（P1）：适合场景：llama.cpp/GGUF 本地部署、多模态体育模型边缘推理；风险：mmproj/视觉适配器、量化等级、llama.cpp 兼容版本未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/waynehwang/multimodal_sport_gemma3_gguf
- INCModel2/GLM-5.2-MXFP4-Mixed-LLMC（P1）：适合场景：GLM-5.2 低比特/压缩张量推理、AutoRound 量化跟踪；风险：license 为 other、量化格式兼容性未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/INCModel2/GLM-5.2-MXFP4-Mixed-LLMC

### Agent 与多智能体

- osmapi/osmQwopus3.6-27B-Fable-Agentic（P0）：适合场景：工具调用/函数调用 SFT 与 agent 评测回放；风险：AGPL-3.0 和函数调用格式未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic
- parth-1/metaguard-policy-agent-v1（P0）：适合场景：policy/guard agent 节点；风险：schema、真实基座和误判率未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/parth-1/metaguard-policy-agent-v1
- voidful/gemma-4-e4b-it-agent-sft-tw（P0）：适合场景：繁体中文 agent-sft；风险：评测分数和推理兼容性未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/voidful/gemma-4-e4b-it-agent-sft-tw
- autotrust/gemma4-31B-Fable-5-Distilled（P1）：适合场景：多模态 + tool-use/coding 复合能力探索；风险：pipeline 与 multimodal 标签需核验；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/autotrust/gemma4-31B-Fable-5-Distilled

### RAG 与知识工程

- arizal/qwen2.5-1.5b-legal-sft（P1）：适合场景：法律 RAG 的小模型答案草拟/风格微调；风险：法律数据来源、法域、幻觉控制未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/arizal/qwen2.5-1.5b-legal-sft

### 推理、训练与后训练

- osmapi/osmQwopus3.6-27B-Fable-Agentic（P0）：适合场景：Fable-5 traces 相关 agent SFT/全量微调参考；风险：训练数据授权和格式未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic
- autotrust/gemma4-31B-Fable-5-Distilled（P1）：适合场景：QLoRA/蒸馏、多模态 tool-use 数据实验；风险：授权、benchmark、视觉输入处理未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/autotrust/gemma4-31B-Fable-5-Distilled
- arizal/qwen2.5-1.5b-legal-sft（P1）：适合场景：领域 SFT 小模型基线；风险：训练语料和评测未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/arizal/qwen2.5-1.5b-legal-sft
- INCModel2/GLM-5.2-MXFP4-Mixed-LLMC（P1）：适合场景：AutoRound/压缩张量量化效果观察；风险：精度损失与后端兼容未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/INCModel2/GLM-5.2-MXFP4-Mixed-LLMC

### 推理系统与工程工具

- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4（P1）：适合场景：Apple Silicon 上 MLX-VLM FP4 低内存部署实验；风险：许可证、安全边界、加载命令未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit（P1）：适合场景：Apple Silicon 上 8bit 多模态部署和 FP4 对照；风险：资源占用和 MLX 版本要求未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit
- waynehwang/multimodal_sport_gemma3_gguf（P1）：适合场景：GGUF/llama.cpp 本地推理链路；风险：视觉投影文件和量化等级未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/waynehwang/multimodal_sport_gemma3_gguf
- INCModel2/GLM-5.2-MXFP4-Mixed-LLMC（P1）：适合场景：compressed-tensors/8-bit 量化推理；风险：license other 与后端兼容性；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/INCModel2/GLM-5.2-MXFP4-Mixed-LLMC

### 多模态与生成媒体

- autotrust/gemma4-31B-Fable-5-Distilled（P1）：适合场景：多模态 + code/tool-use 复合 Agent 子任务；风险：pipeline text-generation 与 multimodal 标签需核验；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/autotrust/gemma4-31B-Fable-5-Distilled
- waynehwang/multimodal_sport_gemma3（P1）：适合场景：韩语体育图文问答；风险：训练数据规模和视觉处理未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/waynehwang/multimodal_sport_gemma3
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4（P1）：适合场景：MLX 多模态 FP4 量化；风险：license 未确认、uncensored 安全风险；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-FP4
- AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit（P1）：适合场景：MLX 多模态 8bit 量化对照；风险：license 和资源需求未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AEON-7/Qwen3.6-27B-AEON-Ultimate-Uncensored-Multimodal-MLX-8bit
- waynehwang/multimodal_sport_gemma3_gguf（P1）：适合场景：多模态 GGUF 边缘推理；风险：mmproj/视觉适配器未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/waynehwang/multimodal_sport_gemma3_gguf

### 评测与基准

- voidful/gemma-4-e4b-it-agent-sft-tw（P0）：适合场景：繁体中文 agent-sft 与 claw-eval-zh 相关评测跟踪；风险：候选信息未提供具体 benchmark 分数；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/voidful/gemma-4-e4b-it-agent-sft-tw

### 产品与商业化

- parth-1/metaguard-policy-agent-v1（P0）：适合场景：policy/guard agent 产品节点 PoC；风险：policy 任务定义和错误成本未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/parth-1/metaguard-policy-agent-v1

### 数据集与数据工程

- waynehwang/multimodal_sport_gemma3（P1）：适合场景：hyokwan/multi_modal_sample 相关垂直多模态数据构建参考；风险：数据集规模、授权和质量未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/waynehwang/multimodal_sport_gemma3
