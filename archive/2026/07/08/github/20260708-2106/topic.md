## 2026-07-08 21:06 GitHub 项目主题条目

### Agent 与多智能体

- **volcengine/SearchCLI**（P0）：适用场景：Agent 需要稳定接入搜索、推荐、conversational retrieval，并通过 dry-run、确认门禁、read-after-write 验证形成可审计工作流。成熟度：stars 999，README 已确认功能和依赖；实际 Volcengine 服务调用未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/volcengine/SearchCLI
- **SepineTam/mcp-for-stata**（P0）：适用场景：让 Claude Code、Codex、OpenClaw 等 Agent 安全调用 Stata 执行计量 / 社科数据分析。成熟度：stars 217，有 PyPI、插件和多 Agent 指南；本地 Stata、沙箱和权限边界未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/SepineTam/mcp-for-stata
- **PythonnotJava/RemindAI**（P1）：适用场景：桌面个人 Agent 工作台，整合本地执行器、文件操作、记忆、MCP 和技能系统。成熟度：stars 12，功能面广但社区验证弱，未运行 release。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/PythonnotJava/RemindAI
- **Hack23/European-Parliament-MCP-Server**（P1）：适用场景：把领域开放数据封装成 MCP 工具，供 Claude Desktop、VS Code、Cursor、GitHub Copilot 等客户端查询和分析。成熟度：stars 17，文档 / npm 信号存在，但工具输出质量未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/Hack23/European-Parliament-MCP-Server

### RAG 与知识工程

- **volcengine/SearchCLI**（P0）：适用场景：生产 RAG、搜索推荐系统的数据接入、检索验证、坏例分析和调优闭环。成熟度：stars 999，README 完整；依赖 Volcengine AI Search 权限，未实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/volcengine/SearchCLI
- **vanthree31/PaperLens**（P1）：适用场景：学术文献 RAG / research workbench，结合自然语言 query planning、跨库检索、论文分析和 citation graph。成熟度：stars 13，README 声称 35 数据源与 CARSI，demo 资产仍有 TODO，未部署验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/vanthree31/PaperLens

### 推理系统与工程工具

- **kekzl/imp**（P1）：适用场景：RTX 5090 / RTX PRO 6000 单卡本地 LLM 推理、NVFP4 SafeTensors、GGUF dense decode 和低延迟 Agent 循环。成熟度：stars 29，技术目标清晰但硬件强绑定；性能未复测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/kekzl/imp
- **volcengine/SearchCLI**（P0）：适用场景：以 CLI / skills 方式把检索、推荐和调优操作纳入 Agent runtime 的工程工具层。成熟度：stars 999，README 已确认命令面；未安装验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/volcengine/SearchCLI
- **SepineTam/mcp-for-stata**（P0）：适用场景：专业统计软件的 MCP / CLI 工具化接入，供 Coding Agent 生成、执行、迭代分析代码。成熟度：stars 217，生态适配较明确；实际 Stata 执行未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/SepineTam/mcp-for-stata
- **PythonnotJava/RemindAI**（P1）：适用场景：本地工具执行器、技能系统、记忆和 MCP server 管理的桌面集成。成熟度：stars 12，未审计沙箱与插件权限。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/PythonnotJava/RemindAI

### 推理、训练与后训练

- **kekzl/imp**（P1）：适用场景：观察 Blackwell FP4 / NVFP4 量化模型在消费级 GPU 上的推理路径和 kernel 设计。成熟度：stars 29，README 性能为作者自报，需硬件复测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/kekzl/imp

### 数据集与数据工程

- **SepineTam/mcp-for-stata**（P0）：适用场景：社科 / 计量数据分析流程自动化，把 Stata 执行纳入 Agent 数据处理闭环。成熟度：stars 217，需要本地 Stata 环境，未实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/SepineTam/mcp-for-stata
- **vanthree31/PaperLens**（P1）：适用场景：学术数据源聚合、机构访问、跨库检索和 citation graph 数据产品。成熟度：stars 13，CARSI / 35 数据源可用性未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/vanthree31/PaperLens
- **Hack23/European-Parliament-MCP-Server**（P1）：适用场景：European Parliament Open Data 的结构化查询、领域 schema 封装和 OSINT 分析工具。成熟度：stars 17，API 调用未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/Hack23/European-Parliament-MCP-Server

### 产品与商业化

- **PythonnotJava/RemindAI**（P1）：适用场景：个人桌面 AI 助手产品形态、ToolShell UX、技能安装和本地记忆体验。成熟度：stars 12，早期项目，未体验安装包。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/PythonnotJava/RemindAI
- **vanthree31/PaperLens**（P1）：适用场景：中文科研用户的一站式论文发现与分析产品。成熟度：stars 13，访问链路和 AI 检索质量未验证。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/vanthree31/PaperLens

### 评测与基准

- **Hack23/European-Parliament-MCP-Server**（P1）：适用场景：领域 MCP 工具的结构化问答 / 开放数据分析评测样例，尤其是政治事实查询和分析指标一致性检查。成熟度：stars 17，指标输出和 API 响应未实测。详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g | 原文：https://github.com/Hack23/European-Parliament-MCP-Server
