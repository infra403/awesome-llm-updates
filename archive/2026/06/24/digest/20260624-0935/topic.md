## 2026-06-24 09:35 每日主题观察

### Agent
- **值得跟进方向**：Agent workflow、memory、context budget、multi-harness orchestration。
- **核心变化**：GitHub 当前窗口 P0 候选集中在 Dify、Openloomi、SDL-MCP、Omnigent；HF CUGA 博客提供轻量 harness 的 agentic app examples。
- **工程影响**：coding/业务 Agent 架构需要把上下文预算、工具治理、长期记忆和失败恢复作为一等公民。
- **建议动作**：**今天应实验** SDL-MCP/CUGA；对 Dify/Openloomi/Omnigent 先看本次 diff 或 release notes。
- **详情链接**：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://github.com/GlitterKill/sdl-mcp 、https://github.com/langgenius/dify 、https://github.com/melandlabs/openloomi 、https://github.com/omnigent-ai/omnigent 、https://huggingface.co/blog/ibm-research/cuga-apps

### RAG
- **值得跟进方向**：检索后隐私净化、RAG knowledge poisoning、cross-chart RAG benchmark。
- **核心变化**：Privacy-Preserving RAG 提出多 Agent semantic rewriting；Poisoned Playbooks 关注 RAG 知识投毒对行动型安全 Agent 的影响；ChartWalker 将 RAG 评测扩到跨图表任务。
- **工程影响**：企业 RAG 需要同时做 PII/敏感实体处理、来源可信度评分、检索结果隔离和任务型 eval。
- **建议动作**：**今天应阅读/实验** 前两篇；ChartWalker **持续观察**，等确认复现成本。
- **详情链接**：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://arxiv.org/abs/2606.24623v1 、https://arxiv.org/abs/2606.24402v1 、https://arxiv.org/abs/2606.23997v1

### 安全
- **值得跟进方向**：RAG 投毒、敏感信息泄漏、Agent 行动前验证。
- **核心变化**：今日安全证据不再只停留在 prompt injection，而是指向“检索内容被污染后驱动工具执行错误行动”。
- **工程影响**：安全/代码 Agent 需要把检索结果当作不可信输入；工具调用前要有二次验证、来源审计和策略约束。
- **建议动作**：**今天应阅读** Poisoned Playbooks，并把相关威胁模型加入 Agent 安全 checklist。
- **详情链接**：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd

### 评测
- **值得跟进方向**：advanced AI shared standards、social bias eval methodology、RAG/chart eval。
- **核心变化**：OpenAI 新闻释放评测/安全标准化信号；arXiv Social Bias methodology 关注 benchmark framing 的方法学碎片化。
- **工程影响**：模型上线流程应从单次分数比较转向可审计、可复现、按任务分层的 eval 报告。
- **建议动作**：**今天应阅读** OpenAI 标准化新闻；Social Bias/ChartWalker **持续观察**，读原文后决定是否加入 eval backlog。
- **详情链接**：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://openai.com/index/helping-build-shared-standards-for-advanced-ai 、https://arxiv.org/abs/2606.24596v1 、https://arxiv.org/abs/2606.23997v1

### 模型发布
- **值得跟进方向**：agent 后训练 adapter、本地/小模型、法语低资源模型、MLX/GGUF 部署。
- **核心变化**：HF 窗口 P0/P1 包含 LFM2.5 RLVR/GRPO adapter、rodin-1b、Qwopus3.6 Coder MLX 5Bit、Gemma-4 agent SFT 繁中、Qwen3 GGUF agentic questionnaire。
- **工程影响**：适合做内部小样本 sanity eval，尤其是工具调用、terminal-agent、繁中/法语和本地推理部署；不建议仅凭模型卡标签切换生产模型。
- **建议动作**：**持续观察**；有对应场景时做今天小实验。
- **详情链接**：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://huggingface.co/LLM-OS-Models/LFM2.5-8B-A1B-Raw-ECHO-RLVR-GRPO-Adapters 、https://huggingface.co/rodin-llm/rodin-1b

### LLM Infra
- **值得跟进方向**：MCP、context engine、workflow platform、browser-side model cache。
- **核心变化**：SDL-MCP 指向 policy-centered context budget；Transformers.js Cross-Origin Storage 探索浏览器端跨源存储。
- **工程影响**：前者影响 coding agent token 成本和上下文召回质量；后者影响 Web LLM/embedding/RAG demo 的模型缓存策略。
- **建议动作**：SDL-MCP **今天应实验**；Cross-Origin Storage **持续观察** 浏览器兼容性和权限模型。
- **详情链接**：https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd；来源：https://github.com/GlitterKill/sdl-mcp 、https://huggingface.co/blog/cross-origin-storage
