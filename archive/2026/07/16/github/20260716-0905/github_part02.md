### 5. tikoci/rosetta

- **仓库**：tikoci/rosetta
- **Stars**：28
- **更新时间**：2026-07-16T01:04:52Z
- **Topics**：ai, bun, claude-code, copilot, mcp, mcp-server, mikrotik, routeros, typescript
- **重要性**：P1
- **主题标签**：RAG 与知识工程；Agent 与多智能体
- **核心变化**：候选窗口内更新，摘要显示其是 RouterOS docs + commands + products + changelogs 的 MCP server，使用 SQLite-as-RAG 并来源于 MikroTik。README 片段确认包含 363 页官方 Docusaurus 手册、4402 properties、40000-entry command tree、156 个当前产品硬件规格、658 个 YouTube transcript，并支持 RouterOS /app 容器安装。
- **一句话定位**：把 MikroTik/RouterOS 官方知识库、命令树和产品资料封装成 MCP 工具的垂直 RAG server。
- **解决的问题**：网络设备运维知识分散在文档、命令树、产品规格和视频中，普通 Agent 难以可靠引用；该项目给 RouterOS 领域提供可查询、可部署的 MCP 知识入口。
- **工程影响**：对垂直领域 RAG/MCP server 的数据组织、SQLite 检索和 Agent 运维助手设计有借鉴意义；也可直接服务 MikroTik 网络运维场景。
- **成熟度判断**：Stars 28，垂直小众但 README 数据规模和来源说明较具体；安装和运行完整性未实测。
- **证据边界**：README 已确认；stars、topics、更新时间来自候选 GitHub 元数据；SQLite 检索质量、更新链路、命令安全边界和容器部署未确认。
- **建议动作**：今天应阅读。理由：虽然领域垂直，但 MCP + SQLite-as-RAG 的实现模式可复用到内部文档/设备知识库。
- **URL**：https://github.com/tikoci/rosetta

### 6. artalis-io/bitnet.c

- **仓库**：artalis-io/bitnet.c
- **Stars**：21
- **更新时间**：2026-07-16T01:04:14Z
- **Topics**：avx2, c, cpu-inference, gguf, inference, kv-cache, llm, moe, neon, quantization, simd, turboquant, wasm
- **重要性**：P1
- **主题标签**：推理系统与工程工具；推理、训练与后训练
- **核心变化**：候选窗口内更新，摘要强调纯 C11、零依赖、CPU-first、NEON/AVX2 SIMD、Flash MoE、3-bit KV 压缩、20+ GGUF quant formats 和 WASM。README 片段确认其是 GGUF LLM 小型 C11 推理引擎，并且代码已模块化到模型结构、quant formats、backend state、transformer planning、CPU/GPU execution、KV/logits/prefill 等模块。
- **一句话定位**：用于研究 CPU/WASM/GGUF 轻量推理路径的 C11 LLM inference engine。
- **解决的问题**：在资源受限、依赖敏感或需要嵌入式/WASM 部署的场景，主流推理框架可能过重；该项目探索更小的 GGUF 推理实现和 KV/量化优化。
- **工程影响**：可影响边缘推理、浏览器/WASM 推理、CPU-only fallback、量化格式兼容和 KV cache 优化方案；也适合作为理解 GGUF 推理路径的代码参考。
- **成熟度判断**：Stars 21，早期；README 技术路线清晰，但实际性能、模型兼容性和正确性需验证。
- **证据边界**：README 已确认；stars、topics、更新时间来自候选 GitHub 元数据；benchmark、支持模型实测、WASM 构建和 Flash MoE/TurboQuant 效果未确认。
- **建议动作**：今天应阅读。理由：工程方向与轻量推理相关，但 actionability 需要验证，先读架构和构建文档再决定是否 POC。
- **URL**：https://github.com/artalis-io/bitnet.c

