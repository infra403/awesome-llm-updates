### 推理、训练与后训练

- **artalis-io/bitnet.c**（P1）：适用场景为 CPU/WASM/GGUF 轻量推理、KV cache 压缩、MoE 与量化格式研究；成熟度为 Stars 21、README 模块化说明已确认，benchmark 与模型兼容性未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/artalis-io/bitnet.c
- **Extraltodeus/J-Wash**（P1）：适用场景为后训练替代路线、手动 alignment、模型 steering 和解释可视化；成熟度为 Stars 157、README 工具形态已确认，效果与风险控制未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/Extraltodeus/J-Wash

### 推理系统与工程工具

- **lemonade-sdk/lemonade**（P0）：适用场景为本地推理服务、GPU/NPU/ONNXRuntime/ROCm/Vulkan 后端和 OpenAI API 兼容网关；成熟度为本批最高，需实测硬件兼容与性能；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/lemonade-sdk/lemonade
- **isaacsight/kernel**（P1）：适用场景为 Agent 工具治理、安全运行时和 provenance 工程；成熟度为早期，设计值得阅读但不宜直接依赖；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/isaacsight/kernel
- **artalis-io/bitnet.c**（P1）：适用场景为无重依赖 C11 推理引擎、边缘端和 WASM fallback；成熟度为早期，需要构建和推理正确性验证；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/artalis-io/bitnet.c
- **JustInCache/awesome-mcp-collection**（P1）：适用场景为 MCP 工具发现和配置复用；成熟度为列表型项目，当前证据较弱，持续观察即可；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/JustInCache/awesome-mcp-collection

### 多模态与生成媒体

- 本周期未纳入符合质量门槛的新项目。

### 评测与基准

- **eunomia-bpf/bpf-benchmark**（P1）：适用场景为 Agent 在真实系统优化环境中的闭环评测，尤其是 verifier/JIT/performance feedback；成熟度为研究/基准项目，需验证可复现性和运行成本；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/eunomia-bpf/bpf-benchmark

### 产品与商业化

- **RoboFinSystems/robosystems**（P1）：适用场景为金融智能平台、账本/报告/投资管理 Agent、AWS IaC 交付；成熟度为早期行业平台，范围大但实测证据不足；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/RoboFinSystems/robosystems

### 数据集与数据工程

- **RoboFinSystems/robosystems**（P1）：适用场景为 financial data、XBRL、dbt/Dagster/DuckDB/PostgreSQL/OpenSearch 等数据工程组合；成熟度为 README 已确认但数据管道和部署稳定性未确认；详情：https://my.feishu.cn/docx/IXZGdmtp2oCKKJxfWsXcrBbTn0g；原文：https://github.com/RoboFinSystems/robosystems
