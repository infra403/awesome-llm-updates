### 3. yantrikos/yantrikdb

- **仓库**：yantrikos/yantrikdb
- **Stars**：39
- **更新时间**：2026-07-16T00:45:09Z
- **Topics**：agent-memory, ai-agents, anthropic, claude-code, cognitive-memory, database, embeddings, hnsw, knowledge-graph, llm, llm-memory, mcp, memory, open-source, persistent-memory, python, rag, rust, semantic-memory, vector-database
- **重要性**：P1
- **主题标签**：RAG 与知识工程；Agent 与多智能体
- **核心变化**：候选窗口内更新，项目定位为 AI Agent 的 cognitive memory engine，摘要包含 temporal decay、contradiction detection、autonomous consolidation、knowledge graph、HNSW ANN recall、Rust library、Python bindings、HTTP gateway、MCP server 和 openraft cluster。README 片段确认 PyPI、Crates.io badge，以及 `pip install yantrikdb-mcp` 的 MCP 快速开始。
- **一句话定位**：面向长期 Agent 记忆的 Rust/Python/MCP 混合记忆数据库。
- **解决的问题**：普通向量库难以处理长期记忆的衰减、冲突、合并与结构化知识图谱；该项目把这些能力包装成可嵌入库和 MCP server。
- **工程影响**：可影响 RAG memory 层、个人化 Agent 记忆、长期会话状态、知识图谱与向量召回融合方案；适合与现有向量库方案对比。
- **成熟度判断**：Stars 39，早期；但 README 有 PyPI/Crates.io/MCP 安装入口，工程包装比纯概念项目更完整。AGPL 许可可能影响商业集成。
- **证据边界**：README 已确认；stars、topics、更新时间来自候选 GitHub 元数据；性能、openraft 集群可用性、冲突检测质量和许可证适配未确认。
- **建议动作**：今天应实验。理由：MCP 安装路径明确，适合用小型 Agent 记忆样例验证 API、召回质量和合并机制。
- **URL**：https://github.com/yantrikos/yantrikdb

### 4. eunomia-bpf/bpf-benchmark

- **仓库**：eunomia-bpf/bpf-benchmark
- **Stars**：22
- **更新时间**：2026-07-16T01:05:02Z
- **Topics**：agents, benchmark, bpf, ebpf, ebpf-jit, jit, kernel, koperation, llm, llvm, optimization, performance
- **重要性**：P1
- **主题标签**：评测与基准；Agent 与多智能体
- **核心变化**：候选窗口内更新，摘要称为 AI Agent eBPF optimization benchmark and framework。README 片段确认其把 eBPF 优化建模为 LLM Agent 闭环搜索问题，在 Docker/KVM/AWS 隔离环境中执行优化动作，并返回 verifier、JIT、workload、performance 反馈。
- **一句话定位**：面向系统内核/eBPF 优化任务的 Agentic benchmark 和执行框架。
- **解决的问题**：LLM Agent 在底层系统优化任务上的评测缺少可执行环境、真实反馈和闭环迭代基准；该项目提供 eBPF 这一高约束领域的评测 substrate。
- **工程影响**：对 Agent benchmark、自动代码优化、内核扩展调优和性能反馈循环有参考价值；可用于评估 Agent 是否能在真实 verifier/JIT/perf 约束下改进代码。
- **成熟度判断**：Stars 22，早期研究/基准性质明显；README 指向 paper draft 和 evaluation harness，适合研究验证，不宜作为通用生产工具。
- **证据边界**：README 已确认；stars、topics、更新时间来自候选 GitHub 元数据；benchmark 覆盖范围、可复现实验结果、运行成本和云环境脚本未确认。
- **建议动作**：持续观察。理由：方向重要但适用面较窄，先跟踪论文/基准稳定性，再决定是否纳入内部 Agent 评测集。
- **URL**：https://github.com/eunomia-bpf/bpf-benchmark

