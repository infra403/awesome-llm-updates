## 2026-06-27 09:11 论文主题条目

### Agent 与多智能体

- NOVA: A Verification-Aware Agent Harness for Architecture Evolution in Industrial Recommender Systems
  - 重要性：P1
  - 为什么值得看：它把 LLM Agent 放进工业推荐模型架构演进流程，并把验证护栏作为核心，而不是只做代码生成或超参搜索。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27243v1
- Joint Learning of Experiential Rules and Policies for Large Language Model Agents
  - 重要性：P1
  - 为什么值得看：长期运行 Agent 的经验规则与策略更新容易不同步，这篇论文直接讨论联合学习二者的路线。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27136v1

### RAG 与知识工程

- Language-Based Digital Twins for Elderly Cognitive Assistance
  - 重要性：P1
  - 为什么值得看：语言数字孪生把个性化记忆、用户画像和状态模拟结合到高风险健康场景，适合做长期记忆/RAG 产品的风险参照。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27334v1

### 推理、训练与后训练

- RolloutPipe: Overlapping Pipelined Rollout and Training in Disaggregated On-Policy LLM Reinforcement Learning
  - 重要性：P1
  - 为什么值得看：RLVR/GRPO 后训练越来越依赖分离式 rollout 和训练资源池，流水重叠可能直接影响 GPU 利用率与迭代速度。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26997v1
- Designing Reward Signals for Portable Query Generation: A Case Study in Industrial Semantic Job Search
  - 重要性：P1
  - 为什么值得看：工业 RLAIF 查询生成展示了 LLM-as-judge 奖励表面的对抗性，对所有用奖励模型优化产品行为的团队都有警示意义。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27291v1

### 推理系统与工程工具

- TOPS: First-Principles Visual Token Pruning via Constructing Token Optimal Preservation Sets for Efficient MLLM Inference
  - 重要性：P1
  - 为什么值得看：视觉 token 是 MLLM 推理成本大头，论文提出更原则化的 token 保留集合构造，适合服务端降本团队跟踪。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27161v1
- NOVA: A Verification-Aware Agent Harness for Architecture Evolution in Industrial Recommender Systems
  - 重要性：P1
  - 为什么值得看：它给“Agent 参与生产模型改造”提供了 harness + verification 的工程组织方式。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27243v1
- RolloutPipe: Overlapping Pipelined Rollout and Training in Disaggregated On-Policy LLM Reinforcement Learning
  - 重要性：P1
  - 为什么值得看：它属于后训练基础设施论文，关注 rollout/training 解耦后的资源调度与流水并行。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26997v1

### 多模态与生成媒体

- TOPS: First-Principles Visual Token Pruning via Constructing Token Optimal Preservation Sets for Efficient MLLM Inference
  - 重要性：P1
  - 为什么值得看：多模态模型的视觉 token 裁剪如果能保持指令相关信息，将直接影响 MLLM serving 的成本/质量权衡。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27161v1
- ReasonCLIP-58M: Visually Grounded Commonsense Reasoning Supervision for CLIP
  - 重要性：P1
  - 为什么值得看：它把常识推理监督加入 CLIP 持续预训练，提示视觉编码器本身也可能是多模态推理短板。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26794v1

### 评测与基准

- Prompt Injection in Automated Résumé Screening with Large Language Models: Single and Multi-Injection Settings
  - 重要性：P1
  - 为什么值得看：简历筛选是典型文档型 LLM judge/ranker 场景，prompt injection 会影响排序，适合转化为红队评测集。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27287v1
- Designing Reward Signals for Portable Query Generation: A Case Study in Industrial Semantic Job Search
  - 重要性：P1
  - 为什么值得看：奖励设计与评测器漏洞直接影响 RLAIF 训练方向，需要从 benchmark/线上指标双重视角检查。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27291v1

### 产品与商业化

- Prompt Injection in Automated Résumé Screening with Large Language Models: Single and Multi-Injection Settings
  - 重要性：P1
  - 为什么值得看：招聘排序、材料审核、工单优先级等产品都可能被用户文本中的隐藏指令影响。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27287v1
- Designing Reward Signals for Portable Query Generation: A Case Study in Industrial Semantic Job Search
  - 重要性：P1
  - 为什么值得看：语义职位搜索是明确工业场景，论文讨论的 reward hacking 风险可迁移到搜索、推荐、广告等业务优化。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27291v1
- Language-Based Digital Twins for Elderly Cognitive Assistance
  - 重要性：P1
  - 为什么值得看：健康/养老助手是强需求但高风险场景，数字孪生类产品必须先审视隐私、验证和安全边界。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.27334v1

### 数据集与数据工程

- ReasonCLIP-58M: Visually Grounded Commonsense Reasoning Supervision for CLIP
  - 重要性：P1
  - 为什么值得看：58M 规模推理监督数据若可用，将影响多模态数据构造、过滤和持续预训练策略。
  - 详情：https://my.feishu.cn/docx/GFhOdA2KroFr74xc8eCc5fgbnDc
  - 原文：https://arxiv.org/abs/2606.26794v1
