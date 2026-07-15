### 10. timothystewart6/vllm-gb10

- 仓库：timothystewart6/vllm-gb10
- stars：33
- 更新时间：2026-07-15T19:03:58Z（GitHub Search 候选）；GitHub API 复核为 2026-07-15T19:04:01Z
- topics：arm64, cuda, dgx-spark, docker, gb10, inference, llm, nvidia, pytorch, vllm
- 重要性：P1
- 主题标签：推理系统与工程工具
- 核心变化：README 已确认这是面向 NVIDIA DGX Spark GB10/sm_121a 的可复现 vLLM Docker 镜像，固定 CUDA base、PyTorch、NCCL、FlashInfer、vLLM 等输入，并声明仅支持 linux/arm64 与 GB10 SoC。
- 一句话定位：为 GB10/DGX Spark 提供 pinned stack 的 vLLM 推理镜像。
- 解决的问题：新硬件/新 CUDA 架构上 vLLM、PyTorch、FlashInfer、NCCL 组合容易不可复现；该仓库把组件版本固化为可构建镜像。
- 工程影响：对推理平台工程有参考价值，尤其是新硬件适配、镜像可复现、版本 pinning、GHCR 发布和 release component table 管理。
- 成熟度判断：33 stars，Shell，MIT；README 已确认 GHCR 镜像、docker run 示例、版本 pinning 和硬件限制；适用面很窄，只对 GB10/sm_121a 用户直接有用。
- 证据边界：README 已确认；stars、topics、更新时间来自候选和 GitHub API；未拉取镜像，未在 GB10 硬件验证吞吐、兼容模型和 quantization 行为。
- 建议动作：持续观察。理由：不是通用推理方案，但对新 NVIDIA ARM64 推理栈适配有工程参考，适合在有 GB10 需求时 POC。
- URL：https://github.com/timothystewart6/vllm-gb10
