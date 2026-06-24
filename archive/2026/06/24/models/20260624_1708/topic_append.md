## 2026-06-24 17:08 模型发布主题条目

### 模型发布与模型能力

- gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF（P0）：适合本地/边缘 Agent 世界模型、环境模拟、llama.cpp 兼容性验证；风险：非官方量化包、下载量 0、上下文长度与 benchmark 未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF
- lovedheart/Qwen-AgentWorld-35B-A3B-FP8（P1）：适合 GPU 侧 FP8 推理/服务化试验；风险：推理框架兼容性和 chat template 未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-FP8
- mradermacher/Fabliq-8B-Agent-i1-GGUF（P1）：适合终端/coding-agent 本地推理；风险：i1 与普通版本差异、pipeline、上下文长度未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-i1-GGUF
- ssurface/qwen3-4b-grpo-l5（P1）：适合小模型后训练、CoT 压缩实验对照；风险：level-5 含义和 benchmark 未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ssurface/qwen3-4b-grpo-l5
- idealab-cs2/reappraisal-4b-grpo（P1）：适合情绪调节/行为塑形研究；风险：垂直心理场景合规与安全评测未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/idealab-cs2/reappraisal-4b-grpo

### Agent 与多智能体

- gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF（P0）：适合本地 AgentWorld 与环境模拟 smoke test；风险：非官方量化包、量化配置和基座一致性需核查；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF
- Dhptl/Qwen-AgentWorld-35B-A3B-GGUF（P1）：适合多模态 Agent 环境模拟；风险：多模态 GGUF projector/视觉塔文件可能缺失；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Dhptl/Qwen-AgentWorld-35B-A3B-GGUF
- lovedheart/Qwen-AgentWorld-35B-A3B-FP8（P1）：适合 AgentWorld GPU FP8 路线观察；风险：vLLM/TGI/Transformers 要求未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-FP8
- Nexlab/VibeThinker-Fable-Nano-Agentic-3B（P1）：适合低成本 Agent worker 和 coding/tool-use 子任务；风险：工具调用格式、chat template、继承许可证需核查；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Nexlab/VibeThinker-Fable-Nano-Agentic-3B
- mradermacher/Fabliq-8B-Agent-i1-GGUF（P1）：适合 terminal/coding-agent 本地推理；风险：发布者为量化命名空间，需核查原始模型卡；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-i1-GGUF
- LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN（P1）：适合低比特 AgentWorld 量化路线观察；风险：actionability_needs_validation、license 未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN

### RAG 与知识工程

- LorMolf/Qwen-Embedding-ProcCode-aligned-2k（P1）：适合采购/法务/流程文档检索与领域 RAG embedding baseline；风险：license、向量维度、最大输入长度、benchmark 未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LorMolf/Qwen-Embedding-ProcCode-aligned-2k

### 推理、训练与后训练

- Nexlab/VibeThinker-Fable-Nano-Agentic-3B（P1）：适合观察 QLoRA/agentic/coding 小模型路线；风险：base_model 与训练数据声明需核查；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Nexlab/VibeThinker-Fable-Nano-Agentic-3B
- ssurface/qwen3-4b-grpo-l5（P1）：适合 GRPO + CoT 压缩对小模型推理成本影响的实验；风险：checkpoint 稳定性和 benchmark 未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ssurface/qwen3-4b-grpo-l5
- idealab-cs2/reappraisal-4b-grpo（P1）：适合 RLHF/GRPO 行为塑形和对话安全研究；风险：临床/安全评测未确认，不建议直接上线；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/idealab-cs2/reappraisal-4b-grpo

### 推理系统与工程工具

- gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF（P0）：适合 llama.cpp 本地推理和离线 Agent 子任务；风险：实际 llama.cpp 版本兼容性未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/gaoqianshen/Qwen-AgentWorld-35B-A3B-Q4_K_M-GGUF
- Dhptl/Qwen-AgentWorld-35B-A3B-GGUF（P1）：适合多模态本地推理可行性验证；风险：多模态组件完整性未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Dhptl/Qwen-AgentWorld-35B-A3B-GGUF
- lovedheart/Qwen-AgentWorld-35B-A3B-FP8（P1）：适合 FP8 GPU 服务化路线观察；风险：推理框架版本要求未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/lovedheart/Qwen-AgentWorld-35B-A3B-FP8
- Nexlab/VibeThinker-Fable-Nano-Agentic-3B（P1）：适合本地 Agent worker 和 coding 辅助；风险：输出格式稳定性需实测；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Nexlab/VibeThinker-Fable-Nano-Agentic-3B
- mradermacher/Fabliq-8B-Agent-i1-GGUF（P1）：适合 GGUF 终端 Agent 试验；风险：具体量化位宽和 imatrix 来源未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/mradermacher/Fabliq-8B-Agent-i1-GGUF
- LorMolf/Qwen-Embedding-ProcCode-aligned-2k（P1）：适合 text-embeddings-inference 链路候选；风险：TEI 实际配置未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LorMolf/Qwen-Embedding-ProcCode-aligned-2k
- LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN（P1）：适合 W4A16/AutoRound 量化方法观察；风险：推理框架兼容性和 license 未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN
- AgentRen/avro-python-deflate-bomb-poc（P1）：适合模型下载/解析安全治理；风险：PoC 不是可部署模型，误运行有安全风险；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AgentRen/avro-python-deflate-bomb-poc

### 多模态与生成媒体

- Dhptl/Qwen-AgentWorld-35B-A3B-GGUF（P1）：适合视觉输入到文本决策链路验证；风险：vision/projector 加载方式未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/Dhptl/Qwen-AgentWorld-35B-A3B-GGUF

### 评测与基准

- ssurface/qwen3-4b-grpo-l5（P1）：适合 GSM8K/CoT 压缩研究对照；风险：候选信息未给出 benchmark 分数；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/ssurface/qwen3-4b-grpo-l5
- LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN（P1）：适合低比特 Open LLM leaderboard/量化退化观察；风险：排行榜结果和实际任务表现未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LeaderboardModel1/Qwen-AgentWorld-35B-A3B-AutoRound-W4A16-RTN

### 产品与商业化

- idealab-cs2/reappraisal-4b-grpo（P1）：适合心理/情绪调节垂直产品的安全研究；风险：合规风险高且临床安全证据未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/idealab-cs2/reappraisal-4b-grpo

### 数据集与数据工程

- LorMolf/Qwen-Embedding-ProcCode-aligned-2k（P1）：适合采购/法务文档检索数据集评估；风险：训练数据和领域泛化未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LorMolf/Qwen-Embedding-ProcCode-aligned-2k
- AgentRen/avro-python-deflate-bomb-poc（P1）：适合训练/评测数据解析管线安全检查；风险：漏洞影响范围和修复版本未确认；详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/AgentRen/avro-python-deflate-bomb-poc

