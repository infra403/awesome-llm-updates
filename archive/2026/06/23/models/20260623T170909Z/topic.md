## 2026-06-24 01:09 模型发布主题条目

### 模型发布与模型能力
- `wahidmounir/Agents-K1-Q8_0-GGUF`（P1）：适合 本地/边缘端 Agent 信息抽取、科研/生物医学文本结构化、低运维成本离线推理候选。风险：likes/downloads 均为 0，尚无社区验证；量化来源为第三方仓库，需要核对量化质量与上游权重一致性。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/wahidmounir/Agents-K1-Q8_0-GGUF
- `voidful/barbet-1b-base-agent-sft-tw-fullft`（P1）：适合 繁体中文/台湾语境工具调用、轻量 Agent SFT 对照、中文多轮工具使用数据格式参考。风险：license 标为 other，商用/再分发边界不清；custom-code 需要审计远程代码；likes/downloads 均为 0。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/voidful/barbet-1b-base-agent-sft-tw-fullft
- `npario/SIQ-1-35B-Q4_K_M-GGUF`（P1）：适合 Agentic coding/自动研究子任务、本地 GGUF 评测、蒸馏/MoE 路线观察。风险：第三方量化仓库且 likes/downloads 为 0；“35B”“MoE/tiny”等标签组合需要核对上游模型定义，避免误判实际激活参数或部署需求。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/npario/SIQ-1-35B-Q4_K_M-GGUF
- `invosmartplay/legal-chatbot-indonesia-qwen-0.5b`（P1）：适合 低成本垂直法律问答、印尼语/法律 RAG 辅助模型、边缘部署可行性观察。风险：垂直法律场景有高合规/幻觉风险；训练数据和评测未确认；0 likes/downloads 缺少实际采用信号。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/invosmartplay/legal-chatbot-indonesia-qwen-0.5b
- `Xy2509413/Llama-3.3-70B-Instruct-abliterated`（P1）：适合 安全对齐差异分析、拒答机制/安全评测红队对照，不建议作为业务模型直接候选。风险：abliterated/uncensored 明确提示安全约束弱化；license 未在候选信息中确认；70B 部署成本高且无下载/点赞信号。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Xy2509413/Llama-3.3-70B-Instruct-abliterated
- `Fallow21/glasswing-health-assistant-v1`（P1）：适合 医疗/健康问答原型、RAG 后处理/摘要子任务、低成本垂直助手实验。风险：医疗健康领域风险高，缺少训练数据/评测/安全边界；likes/downloads 为 0；不能据候选信息判断临床可靠性。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Fallow21/glasswing-health-assistant-v1
- `NullVoider/Nex-N2-Pro`（P1）：适合 多模态/图文到文本能力巡检、MoE 结构观察、评测结果字段核对。风险：候选中 pipeline 与 image-text-to-text 标签存在表达不一致；likes/downloads 为 0；模型架构、输入格式和评测细节不明。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/NullVoider/Nex-N2-Pro

### Agent 与多智能体
- `wahidmounir/Agents-K1-Q8_0-GGUF`（P1）：适合 本地/边缘端 Agent 信息抽取、科研/生物医学文本结构化、低运维成本离线推理候选。风险：likes/downloads 均为 0，尚无社区验证；量化来源为第三方仓库，需要核对量化质量与上游权重一致性。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/wahidmounir/Agents-K1-Q8_0-GGUF
- `voidful/barbet-1b-base-agent-sft-tw-fullft`（P1）：适合 繁体中文/台湾语境工具调用、轻量 Agent SFT 对照、中文多轮工具使用数据格式参考。风险：license 标为 other，商用/再分发边界不清；custom-code 需要审计远程代码；likes/downloads 均为 0。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/voidful/barbet-1b-base-agent-sft-tw-fullft
- `npario/SIQ-1-35B-Q4_K_M-GGUF`（P1）：适合 Agentic coding/自动研究子任务、本地 GGUF 评测、蒸馏/MoE 路线观察。风险：第三方量化仓库且 likes/downloads 为 0；“35B”“MoE/tiny”等标签组合需要核对上游模型定义，避免误判实际激活参数或部署需求。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/npario/SIQ-1-35B-Q4_K_M-GGUF
- `Lance1573/acrouter-qwen35-08b-router-lora`（P1）：适合 多模型路由、Agent 子任务分发、coding 请求分类/路由策略实验。风险：adapter 依赖 Qwen/Qwen3.5-0.8B 基座；候选信息未确认论文内容和评测结果；likes/downloads 为 0，社区信号弱。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Lance1573/acrouter-qwen35-08b-router-lora

### RAG 与知识工程
- `invosmartplay/legal-chatbot-indonesia-qwen-0.5b`（P1）：适合 低成本垂直法律问答、印尼语/法律 RAG 辅助模型、边缘部署可行性观察。风险：垂直法律场景有高合规/幻觉风险；训练数据和评测未确认；0 likes/downloads 缺少实际采用信号。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/invosmartplay/legal-chatbot-indonesia-qwen-0.5b
- `Fallow21/glasswing-health-assistant-v1`（P1）：适合 医疗/健康问答原型、RAG 后处理/摘要子任务、低成本垂直助手实验。风险：医疗健康领域风险高，缺少训练数据/评测/安全边界；likes/downloads 为 0；不能据候选信息判断临床可靠性。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Fallow21/glasswing-health-assistant-v1

### 推理、训练与后训练
- `voidful/barbet-1b-base-agent-sft-tw-fullft`（P1）：适合 繁体中文/台湾语境工具调用、轻量 Agent SFT 对照、中文多轮工具使用数据格式参考。风险：license 标为 other，商用/再分发边界不清；custom-code 需要审计远程代码；likes/downloads 均为 0。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/voidful/barbet-1b-base-agent-sft-tw-fullft

### 推理系统与工程工具
- `wahidmounir/Agents-K1-Q8_0-GGUF`（P1）：适合 本地/边缘端 Agent 信息抽取、科研/生物医学文本结构化、低运维成本离线推理候选。风险：likes/downloads 均为 0，尚无社区验证；量化来源为第三方仓库，需要核对量化质量与上游权重一致性。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/wahidmounir/Agents-K1-Q8_0-GGUF
- `npario/SIQ-1-35B-Q4_K_M-GGUF`（P1）：适合 Agentic coding/自动研究子任务、本地 GGUF 评测、蒸馏/MoE 路线观察。风险：第三方量化仓库且 likes/downloads 为 0；“35B”“MoE/tiny”等标签组合需要核对上游模型定义，避免误判实际激活参数或部署需求。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/npario/SIQ-1-35B-Q4_K_M-GGUF
- `Lance1573/acrouter-qwen35-08b-router-lora`（P1）：适合 多模型路由、Agent 子任务分发、coding 请求分类/路由策略实验。风险：adapter 依赖 Qwen/Qwen3.5-0.8B 基座；候选信息未确认论文内容和评测结果；likes/downloads 为 0，社区信号弱。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Lance1573/acrouter-qwen35-08b-router-lora
- `invosmartplay/legal-chatbot-indonesia-qwen-0.5b`（P1）：适合 低成本垂直法律问答、印尼语/法律 RAG 辅助模型、边缘部署可行性观察。风险：垂直法律场景有高合规/幻觉风险；训练数据和评测未确认；0 likes/downloads 缺少实际采用信号。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/invosmartplay/legal-chatbot-indonesia-qwen-0.5b
- `Xy2509413/Llama-3.3-70B-Instruct-abliterated`（P1）：适合 安全对齐差异分析、拒答机制/安全评测红队对照，不建议作为业务模型直接候选。风险：abliterated/uncensored 明确提示安全约束弱化；license 未在候选信息中确认；70B 部署成本高且无下载/点赞信号。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Xy2509413/Llama-3.3-70B-Instruct-abliterated
- `Fallow21/glasswing-health-assistant-v1`（P1）：适合 医疗/健康问答原型、RAG 后处理/摘要子任务、低成本垂直助手实验。风险：医疗健康领域风险高，缺少训练数据/评测/安全边界；likes/downloads 为 0；不能据候选信息判断临床可靠性。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Fallow21/glasswing-health-assistant-v1

### 多模态与生成媒体
- `NullVoider/Nex-N2-Pro`（P1）：适合 多模态/图文到文本能力巡检、MoE 结构观察、评测结果字段核对。风险：候选中 pipeline 与 image-text-to-text 标签存在表达不一致；likes/downloads 为 0；模型架构、输入格式和评测细节不明。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/NullVoider/Nex-N2-Pro

### 评测与基准
- `Lance1573/acrouter-qwen35-08b-router-lora`（P1）：适合 多模型路由、Agent 子任务分发、coding 请求分类/路由策略实验。风险：adapter 依赖 Qwen/Qwen3.5-0.8B 基座；候选信息未确认论文内容和评测结果；likes/downloads 为 0，社区信号弱。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/Lance1573/acrouter-qwen35-08b-router-lora
- `NullVoider/Nex-N2-Pro`（P1）：适合 多模态/图文到文本能力巡检、MoE 结构观察、评测结果字段核对。风险：候选中 pipeline 与 image-text-to-text 标签存在表达不一致；likes/downloads 为 0；模型架构、输入格式和评测细节不明。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb 原文：https://huggingface.co/NullVoider/Nex-N2-Pro
