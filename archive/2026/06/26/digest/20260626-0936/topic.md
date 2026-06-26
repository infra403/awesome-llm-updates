## 2026-06-26 09:36 每日主题观察

- **安全**：MCP 与 RAG 是今日最高优先级安全面。核心变化：ShareLock 描述 MCP 多工具阈值投毒，RAG 安全综述强调检索索引、查询日志、上下文构造的泄露风险。工程影响：Agent 工具注册、工具描述审计、RAG 权限隔离和日志脱敏都需要进入设计评审。建议动作：**今天应阅读** ShareLock 与 RAG 综述，并转成内部 checklist。详情： https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
- **评测**：OpenRCA 2.0 是今日 Agent 评测重点。核心变化：从只标注 root cause 转向故障传播路径/因果过程监督。工程影响：可改造 SRE Agent、长上下文诊断 Agent 和工具调用 Agent 的评测，不再只看最终答案。建议动作：**今天应阅读**，并抽取可复用指标。详情： https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
- **LLM Infra / 推理**：HF vLLM Jobs 提供快速部署 vLLM server 的当前窗口教程。工程影响：适合临时模型评测、demo 和冒烟服务，可能降低 GPU 环境维护成本。建议动作：**今天应实验**，记录启动命令、冷启动时间、并发、成本和日志能力。详情： https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
- **Agent**：OpenAI Agent 工作研究、pmb 本地持久记忆 MCP、ECC/Dify/RAGFlow 当前窗口更新共同显示 Agent workflow 正在向长任务、可记忆、可编排方向推进。工程影响：团队应关注任务持续时间、可验证中间产物、权限边界、记忆审计。建议动作：pmb **今天应实验**；OpenAI 文章和成熟仓库更新 **持续观察**。详情： https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
- **模型发布**：LFM2.5 Agent/RLVR/GRPO adapter 与 Qwen/AgentWorld 相关模型进入当前窗口。工程影响：显示小模型/适配器面向 terminal-agent、reasoning、coding 的后训练试验活跃。建议动作：**今天应实验**仅限 sandbox，先看许可证、模型卡、训练数据和基础 benchmark；低下载/低点赞不宜直接生产选型。详情： https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
- **多模态**：证据顺序敏感性审计论文提示 MLLM 对输入证据顺序可能不稳定。工程影响：多模态评测需要加入 evidence permutation 和 prompt perturbation。建议动作：**持续观察**，如团队有 MLLM 产品则加入回归测试。详情： https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
- **数据 / RAG**：本周期没有高置信新增数据集主线；但 RAG 安全议题要求重新审视索引、日志和上下文数据治理。建议动作：**持续观察**，优先补齐权限与脱敏策略。详情： https://my.feishu.cn/docx/WLhAdbeLooENsmxWJcLckWW6nkd
