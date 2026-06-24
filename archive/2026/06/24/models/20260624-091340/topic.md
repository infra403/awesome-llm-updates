## 2026-06-24 09:13 模型发布主题条目

### 模型发布与模型能力

- **rodin-llm/rodin-1b（P0）**：适合法语基座、本地低成本推理、法语 RAG/抽取任务的候选；风险是 benchmark、上下文长度、chat template 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/rodin-llm/rodin-1b
- **rodin-llm/rodin-1b-instruct（P1）**：适合法语指令跟随、轻量对话和本地 GGUF 冒烟测试；风险是 license、模板和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/rodin-llm/rodin-1b-instruct
- **CMU-AIRe/MRT-online（P1）**：适合小模型推理、数学和 test-time-compute 方法观察；风险是效果、开销和模板未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/CMU-AIRe/MRT-online
- **hyokwan/gemma3_multimodal_test（P1，弱证据）**：适合 Gemma3 多模态加载/TGI 兼容性观察；风险是 test 命名、license/base_model/图像规格/benchmark 均未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/hyokwan/gemma3_multimodal_test

### Agent 与多智能体

- **wilsonramos/qwen3-4b-2507-agentic-questionnaire-gguf（P1）**：适合本地 Agent 工具调用、问卷/结构化任务、llama.cpp 兼容测试；风险是非官方量化、license/量化位宽/tool template 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/wilsonramos/qwen3-4b-2507-agentic-questionnaire-gguf
- **voidful/gemma-4-12b-it-agent-sft-tw-fullft（P1）**：适合繁中 Agent 指令跟随、多模态保留验证和 Gemma 4 12B IT 微调对比；风险是 Gemma license 需审查、full-finetune 可能改变安全/多模态行为。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/voidful/gemma-4-12b-it-agent-sft-tw-fullft
- **LLM-OS-Models/Fabliq-1.2B-Agent-JP-GGUF（P1，弱证据）**：适合日语轻量 Agent、本地 GGUF 推理、Base vs Agent 变体观察；风险是 license、模板、量化位宽和 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LLM-OS-Models/Fabliq-1.2B-Agent-JP-GGUF

### 推理、训练与后训练

- **CMU-AIRe/MRT-online（P1）**：适合 GRPO/MRT/test-time-compute 方向的低成本推理后训练复现；风险是候选无公开分数和推理时开销数据。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/CMU-AIRe/MRT-online
- **arlarena/if_step200（P1）**：适合 Qwen3-8B-Base 指令跟随 RL/GRPO checkpoint 观察、IFBench/SLIME 方向复现；风险是 step200 可能只是中间 checkpoint，不一定可直接服务化。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/arlarena/if_step200

### 推理系统与工程工具

- **rodin-llm/rodin-1b（P0）**：适合用 GGUF/TGI 做法语本地推理与服务化评估；风险是社区验证和资源需求未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/rodin-llm/rodin-1b
- **wilsonramos/qwen3-4b-2507-agentic-questionnaire-gguf（P1）**：适合 llama.cpp/Agent runtime 的工具调用模板兼容性测试；风险是非官方量化质量和 license 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/wilsonramos/qwen3-4b-2507-agentic-questionnaire-gguf
- **LLM-OS-Models/Fabliq-1.2B-Agent-JP-GGUF（P1，弱证据）**：适合本地 GGUF 的日语 Agent 覆盖 smoke test；风险是信息密度低且没有热度。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/LLM-OS-Models/Fabliq-1.2B-Agent-JP-GGUF

### 多模态与生成媒体

- **voidful/gemma-4-12b-it-agent-sft-tw-fullft（P1）**：适合验证 Agent SFT 后 Gemma 多模态能力是否保留；风险是多模态评测和输入规格未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/voidful/gemma-4-12b-it-agent-sft-tw-fullft
- **hyokwan/gemma3_multimodal_test（P1，弱证据）**：适合图文到文本 pipeline/TGI 兼容性观察；风险是测试仓库属性明显，暂不建议工程投入。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/hyokwan/gemma3_multimodal_test

### 评测与基准

- **CMU-AIRe/MRT-online（P1）**：适合数学/推理评测集与 test-time-compute 策略对比；风险是候选未提供 benchmark 分数。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/CMU-AIRe/MRT-online
- **arlarena/if_step200（P1）**：适合 IFBench 指令跟随评测流程观察；风险是具体 IFBench 分数未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/arlarena/if_step200

### 数据集与数据工程

- **rodin-llm/rodin-1b（P0）**：适合追踪法语/多语训练数据组合对 1B 基座的影响，候选标签列出 HPLT、cc100、wikipedia、wikisource、PleIAs/common_corpus；风险是数据清洗、比例、license 和训练细节未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb；原文：https://huggingface.co/rodin-llm/rodin-1b
