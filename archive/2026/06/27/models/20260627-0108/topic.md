## 2026-06-27 01:08 模型发布主题条目

### 模型发布与模型能力
- s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF（P1）：适合本地推理、量化和 Agent coding 候选池预研；风险是 license、benchmark、上下文长度与实际 llama.cpp/NVFP4/MTP 兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF
- renaudb1999/le-harnais-ft-agentworld-8b（P1）：适合 Agent 工具调用/对话任务的 8B 级候选；风险是 AgentWorld 微调收益、benchmark、chat template 和 Llama 3.1 许可证边界需核验。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-8b
- renaudb1999/le-harnais-ft-agentworld-3b（P1）：适合轻量 Agent 和低成本端点实验；风险是 0 下载/点赞且微调收益未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-3b
- renaudb1999/le-harnais-ft-agentworld-1b（P1）：适合极低成本 Agent 分类/路由 baseline；风险是 1B 级多步推理和工具调用稳定性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-1b
- Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000（P1）：适合长上下文 Agent 与投机解码预研；风险是 checkpoint 性质、pipeline、真实上下文长度和加载方式未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000
- Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF（P1）：适合本地多模态/长上下文 GGUF smoke test；风险是 uncensored/abliterated 安全合规、1M context 与 vision 能力未实测。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF
- srmty/smolLM2-360M-instruct-math-v1（P1）：适合小模型数学推理 baseline；风险是复杂推理能力、训练数据配比和 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/srmty/smolLM2-360M-instruct-math-v1
- jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-8B（P1）：适合粤语对话、区域语言 RAG/客服；风险是数据许可、合并方法和 TGI 实际兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-8B
- nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4（P1）：适合推理模型蒸馏与 NVFP4/W4A16 部署预研；风险是命名来源、蒸馏数据、modelopt 配置和硬件兼容性需核验。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4
- jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507（P1）：适合粤语复杂问答和 MoE 方言推理对照；风险是 active parameters、部署成本、benchmark 和训练数据许可未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507

### Agent 与多智能体
- s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF（P1）：适合 Agent coding 与 reasoning 本地候选池；风险是 agentic-coding 标签之外没有候选内 benchmark 证据。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF
- renaudb1999/le-harnais-ft-agentworld-8b / 3b / 1b（P1）：适合构建同系列大小模型 Agent 成本-效果对照；风险是三者均 0 likes/downloads，AgentWorld 任务定义和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-8b 、https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-3b 、https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-1b
- Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000（P1）：适合长上下文 Agent 与 speculative decoding 路线评估；风险是具体窗口和 checkpoint 可用性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000

### 推理系统与工程工具
- s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF（P1）：适合 llama.cpp、NVFP4、MTP 和 Blackwell 相关推理栈 smoke test；风险是硬件/软件版本要求未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/s-batman/Ornith-1.0-35B-NVFP4-MTP-GGUF
- renaudb1999/le-harnais-ft-agentworld-8b / 3b / 1b（P1）：适合 TGI/endpoints_compatible 与 GGUF 双路径检查；风险是实际端点兼容性和量化精度未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/renaudb1999/le-harnais-ft-agentworld-8b
- Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000（P1）：适合 dflash 与 speculative-decoding 工程路线追踪；风险是没有候选内推理命令和性能数据。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000
- Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF（P1）：适合 llama.cpp GGUF 本地加载和长上下文 smoke test；风险是多模态与 1M context 实际支持未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF
- nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4（P1）：适合 NVFP4/W4A16 量化部署验证；风险是 modelopt 配置和硬件兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4

### 推理、训练与后训练
- Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000（P1）：适合观察 Qwen3 衍生 longctx / speculative decoding checkpoint；风险是训练阶段和 step38000 含义未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Lucebox/Laguna-XS.2-Dflash-v28-agent-longctx-step38000
- srmty/smolLM2-360M-instruct-math-v1（P1）：适合 SFT 小模型数学推理 baseline；风险是数据来源和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/srmty/smolLM2-360M-instruct-math-v1
- nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4（P1）：适合 thinking/distill 与量化折中评估；风险是蒸馏来源和质量数据未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/nerkyor/Qwen3.6-27B-DSV4Pro-Thinking-Distill-NVFP4
- jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507（P1）：适合 MoE/Think 方言推理对照；风险是推理开销和模型卡证据不足。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507

### 多模态与生成媒体
- Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF（P1）：适合 image-text-to-text 与本地多模态路线初步验证；风险是 vision 输入链路、上下文长度和安全合规未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Abiray/Huihui-Qwythos-9B-Claude-Mythos-5-1M-abliterated-GGUF

### 评测与基准
- srmty/smolLM2-360M-instruct-math-v1（P1）：适合补充小模型 math/reasoning baseline；风险是候选内无 benchmark，需自建 GSM/math smoke test。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/srmty/smolLM2-360M-instruct-math-v1

### 数据集与数据工程
- jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-8B（P1）：适合粤语测试集、RAG 语料和区域语言客服评估；风险是训练数据许可和向量合并方法未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-8B
- jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507（P1）：适合方言复杂问答数据集对照；风险是数据来源、benchmark 和 MoE serving 成本未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/jed351/cantonese_llm_v2_chat_vector_merged_Qwen3-30B-A3B-Think-2507
