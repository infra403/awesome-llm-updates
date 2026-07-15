### 5. kagent-dev/kagent

- 仓库：kagent-dev/kagent
- stars：3312
- 更新时间：2026-07-15T19:05:00Z（GitHub Search 候选）；GitHub API 复核为 2026-07-15T19:05:08Z
- topics：agents, ai, cncf, devops, mcp
- 重要性：P0
- 主题标签：Agent 与多智能体；推理系统与工程工具
- 核心变化：README 已确认 kagent 是 Kubernetes native framework，用于在 Kubernetes 中构建、部署和管理 AI agents，并带有 UI、release、CI、OpenSSF badge、Discord/DeepWiki 等生态入口。
- 一句话定位：云原生/Kubernetes 场景的 Agent 管理与运行框架。
- 解决的问题：Agent 从本地脚本走向云端运行时，需要部署、生命周期管理、工具/权限、可观测和集群原生集成；kagent 把 Agent 管理问题放进 Kubernetes 控制平面。
- 工程影响：对企业级多 Agent 运维、DevOps Agent、MCP 工具接入和 K8s 原生运行时有参考价值；可能影响 Agent 平台的 CRD/operator、权限模型和 UI 管理形态。
- 成熟度判断：3312 stars，Go，Apache-2.0；README 已确认项目活跃且有 CI/release/社区信号；但具体 API 稳定性、生产案例细节和多租户隔离未确认。
- 证据边界：README 已确认；stars、topics、更新时间来自候选和 GitHub API；未安装到 K8s 集群，未验证 CRD、控制器和 MCP 集成。
- 建议动作：持续观察。理由：成熟度和生态信号强，但 POC 成本高；短期先跟踪架构与 release，待有 K8s Agent 场景再实验。
- URL：https://github.com/kagent-dev/kagent
