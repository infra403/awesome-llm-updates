<fragment mode="range" requested-end="-1" requested-start="doxcnkZ3mcwSWrVX962H3B319gg">
### 10. lianluo-esign/ferrogate

## 2026-06-28 03:05 北京时间 | GitHub 项目巡检

本节仅纳入候选报告 8 小时 recency window 内、带 GitHub URL 与更新时间的 P0/P1 仓库；未为补数量写入 P2 或证据不足条目。

### 1. luckyPipewrench/pipelock（P0）

- 仓库：luckyPipewrench/pipelock
- stars：732
- 更新时间：2026-06-27T19:03:15Z
- topics：agent-security, ai-agent-security, ai-agents, ai-firewall, ai-security, dlp, egress-proxy, fetch-proxy, github-action, golang, integrity-monitoring, llm-security, mcp, mcp-security, prompt-injection, security, security-scanning, security-tools, ssrf, ssrf-protection
- 重要性：Agent 安全边界 / MCP egress 审计
- 主题标签：Agent 与多智能体 / 推理系统与工程工具
- 核心变化：本轮窗口内更新；面向 MCP 与 Agent 出站流量的开源防火墙，把 HTTP、MCP、A2A、WebSocket 访问放到可扫描、可签名留痕的中介层。
- 一句话定位：面向 MCP 与 Agent 出站流量的开源防火墙，把 HTTP、MCP、A2A、WebSocket 访问放到可扫描、可签名留痕的中介层。
- 解决的问题：解决 Agent 工具调用中的数据外泄、SSRF、Prompt Injection 与审计证据不足问题。
- 工程影响：可作为 LLM gateway、MCP server、Agent runtime 的 egress proxy/策略层候选，尤其适合在生产 Agent 前加 DLP、SSRF 与操作收据。
- 成熟度判断：已有一定关注（732 stars），仍处于需要验证的工程候选；生产成熟度未确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=732、updated=2026-06-27T19:03:15Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：今天应阅读：安全边界与 mediator-signed action receipts 可能直接影响现有 Agent/MCP 安全方案。
- URL：https://github.com/luckyPipewrench/pipelock
- README：https://github.com/luckyPipewrench/pipelock/blob/main/README.md

### 2. framerslab/agentos（P0）

- 仓库：framerslab/agentos
- stars：585
- 更新时间：2026-06-27T18:58:27Z
- topics：agent-framework, agent-memory, agentic-ai, ai-agent-framework, ai-agents, autonomous-agents, cognitive-memory, emergent-behavior, guardrails, hexaco, llm, llm-orchestration, long-term-memory, multi-agent, rag, runtime-tool-generation, tool-use, vector-search, voice-ai
- 重要性：Agent 框架 / 记忆与运行时工具生成
- 主题标签：Agent 与多智能体 / RAG 与知识工程
- 核心变化：本轮窗口内更新；TypeScript Agent 框架，强调 cognitive memory、runtime tool forging、多 Agent 编排和 11 个 LLM provider。
- 一句话定位：TypeScript Agent 框架，强调 cognitive memory、runtime tool forging、多 Agent 编排和 11 个 LLM provider。
- 解决的问题：解决长程 Agent 的记忆、工具生成、provider 适配与多智能体协调问题。
- 工程影响：可对比现有 Agent runtime 的 memory abstraction、tool-use API、provider adapter 设计；对 RAG 与长期记忆模块有参考价值。
- 成熟度判断：已有一定关注（585 stars），仍处于需要验证的工程候选；生产成熟度未确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=585、updated=2026-06-27T18:58:27Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：今天应阅读：覆盖 Agent memory、tool forging、multi-agent，多处可能影响框架选型。
- URL：https://github.com/framerslab/agentos
- README：https://github.com/framerslab/agentos/blob/master/README.md

### 3. rivet-dev/agentos（P0）

- 仓库：rivet-dev/agentos
- stars：3283
- 更新时间：2026-06-27T19:01:32Z
- topics：agent, ai, javascript, llm, sandbox, v8, wasm, webassembly
- 重要性：Coding Agent 沙箱 / 隔离运行环境
- 主题标签：Agent 与多智能体 / 推理系统与工程工具
- 核心变化：本轮窗口内更新；用隔离 Linux VM 承载 coding agent，定位为比传统 sandbox 更轻、更快、更便宜，并内建 agent orchestration。
- 一句话定位：用隔离 Linux VM 承载 coding agent，定位为比传统 sandbox 更轻、更快、更便宜，并内建 agent orchestration。
- 解决的问题：解决 coding agent 执行任意命令时的隔离、成本和编排问题。
- 工程影响：可影响内部 agent 执行器、CI 沙箱、浏览器/终端工具调用隔离方案；WASM/V8 方向值得与容器/Firecracker 对比。
- 成熟度判断：社区关注度较高（3283 stars），但生产成熟度、维护节奏和安装稳定性仍需 README/试跑确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=3283、updated=2026-06-27T19:01:32Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：今天应实验：星数和定位显示生态关注度高，适合做一次最小 agent sandbox POC。
- URL：https://github.com/rivet-dev/agentos
- README：https://github.com/rivet-dev/agentos/blob/main/README.md

### 4. hwdsl2/self-hosted-ai-stack（P0）

- 仓库：hwdsl2/self-hosted-ai-stack
- stars：108
- 更新时间：2026-06-27T18:56:51Z
- topics：ai, ai-stack, cuda, docker, docker-compose, docling, embeddings, linux, litellm, llm, local-ai, mcp, ollama, openai-compatible, private-ai, rag, self-hosted, speech-to-text, text-to-speech, whisper
- 重要性：本地 AI 栈 / Docker Compose 参考架构
- 主题标签：推理系统与工程工具 / RAG 与知识工程
- 核心变化：本轮窗口内更新；Docker Compose 一键部署本地 AI 栈：Ollama、LiteLLM、AnythingLLM、Whisper、Kokoro、Embeddings、Docling 与 MCP Gateway。
- 一句话定位：Docker Compose 一键部署本地 AI 栈：Ollama、LiteLLM、AnythingLLM、Whisper、Kokoro、Embeddings、Docling 与 MCP Gateway。
- 解决的问题：解决私有化 LLM/RAG/语音能力组合部署、CUDA 可选加速、多架构适配的问题。
- 工程影响：可作为本地-first AI demo、内网 RAG/语音管线、LiteLLM gateway 与 MCP gateway 联调的基线模板。
- 成熟度判断：已有一定关注（108 stars），仍处于需要验证的工程候选；生产成熟度未确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=108、updated=2026-06-27T18:56:51Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：今天应实验：部署面覆盖推理、RAG、语音和 MCP，适合快速验证私有化栈组合。
- URL：https://github.com/hwdsl2/self-hosted-ai-stack
- README：https://github.com/hwdsl2/self-hosted-ai-stack/blob/main/README.md

### 5. MakazhanAlpamys/Soup（P0）

- 仓库：MakazhanAlpamys/Soup
- stars：72
- 更新时间：2026-06-27T19:02:25Z
- topics：artificial-intelligence, cli, dpo, fine-tuning, finetuning, gguf, huggingface, llm, llmops, local-llm, lora, machine-learning, model-finetuning, ollama, peft, python, pytorch, qlora, sft, transformers
- 重要性：微调工作流 CLI / SFT-DPO-QLoRA
- 主题标签：推理、训练与后训练 / 模型发布与模型能力
- 核心变化：本轮窗口内更新；把 LLM fine-tuning 简化为一个配置、一个命令的 workflow，覆盖 LoRA/QLoRA、SFT/DPO、HF/Ollama/GGUF 相关生态。
- 一句话定位：把 LLM fine-tuning 简化为一个配置、一个命令的 workflow，覆盖 LoRA/QLoRA、SFT/DPO、HF/Ollama/GGUF 相关生态。
- 解决的问题：解决微调脚本、数据/配置、导出/本地部署流程分散的问题。
- 工程影响：可作为团队内部轻量微调脚手架参考，重点检查配置抽象、训练后导出 GGUF/Ollama 的链路是否可复用。
- 成熟度判断：早期项目（72 stars），适合技术储备或小范围 POC；生产成熟度未确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=72、updated=2026-06-27T19:02:25Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：今天应阅读：如配置模型清晰，可能降低小模型后训练试验成本。
- URL：https://github.com/MakazhanAlpamys/Soup
- README：https://github.com/MakazhanAlpamys/Soup/blob/main/README.md

### 6. Michael-OvO/obsidian-knowledge-agent（P0）

- 仓库：Michael-OvO/obsidian-knowledge-agent
- stars：202
- 更新时间：2026-06-27T19:04:59Z
- topics：agentic-workflows, ai-agents, claude, codex, knowledge-management, llm, obsidian
- 重要性：知识加工 Agent / Obsidian 管线
- 主题标签：RAG 与知识工程 / Agent 与多智能体
- 核心变化：本轮窗口内更新；把 PDF、slides、syllabi、papers、URL 等原始材料转成结构化、教学质量的 Obsidian notes，包含 ingest、compile、distribute 流程。
- 一句话定位：把 PDF、slides、syllabi、papers、URL 等原始材料转成结构化、教学质量的 Obsidian notes，包含 ingest、compile、distribute 流程。
- 解决的问题：解决知识库从原始材料到可读笔记/课程化内容的自动加工与分发问题。
- 工程影响：可参考其 ingest-compile-distribute 拆分，用于 RAG 资料清洗、教学资料生成、企业知识库整理。
- 成熟度判断：已有一定关注（202 stars），仍处于需要验证的工程候选；生产成熟度未确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=202、updated=2026-06-27T19:04:59Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：持续观察：定位清晰但更偏知识工作流，需要确认安装方式和输出质量后再 POC。
- URL：https://github.com/Michael-OvO/obsidian-knowledge-agent
- README：https://github.com/Michael-OvO/obsidian-knowledge-agent/blob/main/README.md

### 7. mrwadams/attackgen（P0）

- 仓库：mrwadams/attackgen
- stars：1222
- 更新时间：2026-06-27T17:32:24Z
- topics：README topics 未在候选中提供
- 重要性：安全演练场景生成 / LLM + MITRE ATT&CK
- 主题标签：评测与基准 / Agent 与多智能体
- 核心变化：本轮窗口内更新；基于 LLM 和 MITRE ATT&CK，为组织生成定制化 incident response 测试场景。
- 一句话定位：基于 LLM 和 MITRE ATT&CK，为组织生成定制化 incident response 测试场景。
- 解决的问题：解决安全团队演练题材构造、威胁 actor 映射和响应流程压力测试的内容生成问题。
- 工程影响：可用于评估安全 Agent、SOC copilot、IR runbook 的场景覆盖；也可生成红队/蓝队演练数据。
- 成熟度判断：社区关注度较高（1222 stars），但生产成熟度、维护节奏和安装稳定性仍需 README/试跑确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=1222、updated=2026-06-27T17:32:24Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。 候选未提供 topics，需后续补查仓库 topics。
- 建议动作：今天应阅读：高 star 且与评测/安全场景生成相关，适合纳入安全评测素材池。
- URL：https://github.com/mrwadams/attackgen
- README：https://github.com/mrwadams/attackgen/blob/main/README.md

### 8. callstack/agent-device（P0）

- 仓库：callstack/agent-device
- stars：2928
- 更新时间：2026-06-27T19:05:20Z
- topics：adb, agentic-ai, agents, ai-agents, android-emulator, automation, e2e-testing, expo, flutter, ios-simulator, mcp, mobile, mobile-testing, performance-optimization, react-native, testing, xcuitest
- 重要性：移动设备控制 CLI / Agent E2E 测试
- 主题标签：Agent 与多智能体 / 评测与基准
- 核心变化：本轮窗口内更新；让 AI agents 控制 iOS 与 Android 设备的 CLI，覆盖模拟器、ADB、XCUITest、移动端 E2E 与 MCP 场景。
- 一句话定位：让 AI agents 控制 iOS 与 Android 设备的 CLI，覆盖模拟器、ADB、XCUITest、移动端 E2E 与 MCP 场景。
- 解决的问题：解决 Agent 对真实/模拟移动设备操作能力不足、跨平台移动测试自动化接入困难的问题。
- 工程影响：可接入 coding/testing agent 做移动 App 自动测试、性能验证和 MCP device-control 工具链。
- 成熟度判断：社区关注度较高（2928 stars），但生产成熟度、维护节奏和安装稳定性仍需 README/试跑确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=2928、updated=2026-06-27T19:05:20Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：今天应实验：移动端 agent control 是明确短板，星数和 topics 显示已有工程关注度。
- URL：https://github.com/callstack/agent-device
- README：https://github.com/callstack/agent-device/blob/main/README.md

### 9. tobocop2/lilbee（P1）

- 仓库：tobocop2/lilbee
- stars：30
- 更新时间：2026-06-27T19:00:03Z
- topics：ai-agents, ai-search-engine, embeddings, gguf, huggingface, llama-cpp, lm-studio, local-ai, local-llm, local-search-engine, mcp, ollama, privacy, python, rag, search-engine, self-hosted, semantic-search, tui, vector-search
- 重要性：本地 AI 搜索 / MCP server
- 主题标签：RAG 与知识工程 / 推理系统与工程工具
- 核心变化：本轮窗口内更新；本地 AI 搜索引擎，管理本地模型、搜索文件与代码、爬取网页，提供引用答案、TUI/CLI/REST/Python library 和 MCP server。
- 一句话定位：本地 AI 搜索引擎，管理本地模型、搜索文件与代码、爬取网页，提供引用答案、TUI/CLI/REST/Python library 和 MCP server。
- 解决的问题：解决本地隐私搜索、代码/文件语义检索、Agent 可调用知识入口的问题。
- 工程影响：可作为 local-first RAG 和 MCP search tool 的实验对象，对比现有向量库/embedding 管线。
- 成熟度判断：早期项目（30 stars），适合技术储备或小范围 POC；生产成熟度未确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=30、updated=2026-06-27T19:00:03Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：持续观察：工程方向契合 RAG/MCP，但 stars 低，先确认活跃度和安装成本。
- URL：https://github.com/tobocop2/lilbee
- README：https://github.com/tobocop2/lilbee/blob/main/README.md

### 10. SlavaSexton/ComfyUI-Agent-Kit（P1）

- 仓库：SlavaSexton/ComfyUI-Agent-Kit
- stars：12
- 更新时间：2026-06-27T19:02:59Z
- topics：ai-art, anthropic, claude, claude-code, claude-skill, codex, comfyui, gemini-cli, glm, image-generation, mcp, qwen, stable-diffusion, video-generation
- 重要性：ComfyUI Agent 技能包 / 多模态工作流
- 主题标签：多模态与生成媒体 / Agent 与多智能体
- 核心变化：本轮窗口内更新；为 Claude Code、Codex、Gemini CLI、Qwen Code 等 coding agents 提供一个 ComfyUI skill，包含模型提示 recipes、模板、硬件感知选择、自动启动和 workflow building。
- 一句话定位：为 Claude Code、Codex、Gemini CLI、Qwen Code 等 coding agents 提供一个 ComfyUI skill，包含模型提示 recipes、模板、硬件感知选择、自动启动和 workflow building。
- 解决的问题：解决 coding agent 驱动本地 ComfyUI 端到端生成图像/视频工作流时的提示、模板和环境编排问题。
- 工程影响：可用于多模态 agent 工具链实验，观察 skill 化 prompt/workflow 模板如何跨 agent 复用。
- 成熟度判断：早期项目（12 stars），适合技术储备或小范围 POC；生产成熟度未确认。
- 证据边界：证据来自本轮 GitHub updated 窗口、候选 metadata、stars=12、updated=2026-06-27T19:02:59Z、topics。README 已读取。安装方式、许可证兼容性、CI 状态、真实可运行性未确认。
- 建议动作：暂不跟进：方向有参考价值，但 stars 很低、成熟度未确认，保留为多模态 agent 备选。
- URL：https://github.com/SlavaSexton/ComfyUI-Agent-Kit
- README：https://github.com/SlavaSexton/ComfyUI-Agent-Kit/blob/master/README.md
- 仓库：lianluo-esign/ferrogate
- stars：16
- 更新时间：2026-06-27T13:00:18Z
- topics：ai, ai-agent, ai-gateway, ai-tools, aigateway, api-gateway, bifrost, infrastructure, mcp-gateway, portkey, reverse-proxy
- 重要性：P1
- 主题标签：推理系统与工程工具；Agent 与多智能体
- 核心变化：本窗口内更新，README 描述 FerroGate 是基于 Cloudflare Pingora 的开源 Rust API gateway / AI gateway，覆盖 OpenAI-compatible APIs、provider routing、virtual API keys、policy checks、token accounting、MCP/tool execution、agent runs、WASM sandboxed agent execution、observability、Admin APIs、cluster ops 和 automatic HTTPS。
- 一句话定位：自托管 LLM 流量控制与 MCP/tool 执行网关。
- 解决的问题：多模型/多 provider 调用中需要统一路由、fallback、虚拟 key、预算策略、缓存、审计观测和工具执行控制点。
- 工程影响：对 LLM gateway、MCP gateway、安全执行沙箱和 provider governance 方向值得关注；若实现成熟，可承载企业内统一 AI 出口和策略层。
- 成熟度判断：stars 16，极早期；Rust/Pingora 技术选型有性能潜力，但功能面很宽，必须以 product overview 和实测确认哪些已实现。
- 证据边界：README 已确认定位、能力清单和 Token4AI Cloud 背景；候选元数据确认 stars、topics、更新时间；具体实现完成度、部署文档、缓存/fallback 行为未确认。
- 建议动作：持续观察。理由：方向重要但成熟度低，先跟踪实现状态和 release。
- URL：https://github.com/lianluo-esign/ferrogate
</fragment>
