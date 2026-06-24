## 2026-06-24 21:35 每日主题观察

- **Agent**：核心变化是 Agent memory 评测从端到端黑盒任务分转向持久存储、检索、更新、合并、生命周期治理等子系统能力；SHERLOC 把代码修复 Agent 的故障定位推进到结构化诊断。工程影响是长期 Agent 与 coding agent 的瓶颈会落在 memory governance 与 pre-edit diagnosis。建议动作：**今天应阅读 / 今天应实验**；详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://arxiv.org/abs/2606.24775v1 ，https://arxiv.org/abs/2606.24820v1

- **RAG / 安全**：核心变化是隐私保护 RAG 与知识投毒安全 Agent 两条 P0 论文同时出现。工程影响是 RAG 安全不能只依赖 prompt guardrail，需要覆盖检索内容清洗、语义保真重写、知识库来源可信度、playbook 变更审计与投毒回归测试。建议动作：**今天应阅读**；详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://arxiv.org/abs/2606.24623v1 ，https://arxiv.org/abs/2606.24402v1

- **模型发布**：核心变化是 HF 10 小时窗口内出现多条 Agentic / terminal / reasoning / GGUF / LoRA adapter 候选。工程影响是本地 Agent 原型的模型选择可扩展到 8B GGUF、27B agentic 与 LFM2.5 adapter，但当前 likes/downloads 和评测证据有限。建议动作：**持续观察**，先做 smoke test 而非线上替换；详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://huggingface.co/osmapi/osmQwopus3.6-27B-Fable-Agentic ，https://huggingface.co/mradermacher/Fabliq-8B-Agent-Reasoning-GGUF ，https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters

- **推理 / LLM Infra**：核心变化是 OpenAI 与 Broadcom 在 2026-06-24 披露 LLM-optimized inference chip Jalapeño。工程影响是推理成本、吞吐、能耗和供应链可能成为闭源 API 竞争变量，也给自建推理团队提供 ASIC/专用硬件观察点。建议动作：**今天应阅读**；详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://openai.com/index/openai-broadcom-jalapeno-inference-chip

- **评测 / 工程工具 / 开源项目**：核心变化是 Opik、Dify、oh-my-pi 在 GitHub 窗口内活跃更新，分别对应 LLM/RAG/Agent tracing eval、agentic workflow/MCP/RAG 平台、终端 coding agent。工程影响是团队工作流需要同时关注可观测、可评测、可编排和安全编辑。建议动作：**持续观察**，先核对具体 commit/release note；详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://github.com/comet-ml/opik ，https://github.com/langgenius/dify ，https://github.com/can1357/oh-my-pi

- **多模态 / 数据**：本周期未发现可进入今日主线的独立 P0/P1 信号；多模态仅在个别模型标签中出现，数据工程主要作为 RAG 安全与知识库治理的背景。建议动作：**暂不跟进**，等待更强来源或评测证据；详情：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
