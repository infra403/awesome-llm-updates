## 2026-06-26 17:07 模型发布主题条目

### 模型发布与模型能力

- `zenlm/zen-agent-4b`（P0）：适合 Agent 子任务和低成本工具调用模型候选；风险是 benchmark、上下文长度、chat template 未在候选信息中确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-agent-4b
- `zenlm/zen-eco-4b-agent-gguf`（P0）：适合本地部署和 GGUF 推理成本验证；风险是量化等级、文件大小、模板兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-eco-4b-agent-gguf
- `hardikchadda/hatch-agent-qwen2.5-1.5b`（P1）：适合边缘设备/Arduino/TinyML Agent 原型；风险是硬件兼容矩阵、内存占用和延迟未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/hardikchadda/hatch-agent-qwen2.5-1.5b

### Agent 与多智能体

- `zenlm/zen-agent-4b`（P0）：适合 function-calling/tool-use Agent worker 候选；风险是函数调用 schema 支持程度和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-agent-4b
- `zenlm/zen-vl-8b-agent`（P0）：适合截图问答、文档图片理解和多模态 Agent 成本基线；风险是图像 token 策略、视觉评测和 chat template 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-vl-8b-agent
- `zenlm/zen-vl-4b-agent`（P0）：适合低成本视觉 Agent worker 和预路由；风险是未确认工具调用标签与 OCR/定位能力。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-vl-4b-agent
- `dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-gguf`（P1）：适合本地 coding Agent 和工具调用对照；风险是 refusal-reduced 标签带来安全评估需求且暂无下载验证。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-gguf
- `dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-mlx-oq`（P1）：适合 Apple Silicon coding Agent 对照；风险是 OQ/8-bit 细节、工具调用可靠性和热度证据不足。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-mlx-oq

### 推理系统与工程工具

- `zenlm/zen-eco-4b-agent-gguf`（P0）：适合 llama.cpp/GGUF 本地吞吐、内存和质量损失验证；风险是具体量化等级未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-eco-4b-agent-gguf
- `zenlm/zen-eco-4b-agent-mlx`（P0）：适合 Mac/MLX 本地 Agent 推理链路；风险是 MLX 版本、量化方法和模板兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-eco-4b-agent-mlx
- `hardikchadda/hatch-agent-qwen2.5-1.5b`（P1）：适合 on-device 函数调用和 TinyML 原型；风险是部署脚本和实际硬件运行证据未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/hardikchadda/hatch-agent-qwen2.5-1.5b
- `nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF`（P1）：适合 reasoning GGUF 本地评测和量化对照；风险是 actionability_needs_validation、0 downloads 且蒸馏细节未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF

### 多模态与生成媒体

- `zenlm/zen-vl-30b-agent`（P0）：适合视觉 Agent、UI/截图分析、多模态工具调用原型；风险是显存需求、图像分辨率和视觉 benchmark 未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-vl-30b-agent
- `zenlm/zen-vl-8b-agent`（P0）：适合低成本多模态评测和视觉问答 Agent；风险是函数调用能力和模板兼容性未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-vl-8b-agent
- `zenlm/zen-vl-4b-agent`（P0）：适合边缘侧视觉问答/截图分类；风险是视觉质量、OCR 和定位能力未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/zenlm/zen-vl-4b-agent

### 推理、训练与后训练

- `dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-gguf`（P1）：适合研究 refusal-reduced 后训练对 coding/agent 的影响；风险是安全边界和训练方法未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-gguf
- `dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-mlx-oq`（P1）：适合同分支 MLX 量化对照；风险是 OQ 量化细节和运行要求未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/dawncr0w/crowqwen3.6-35b-a3b-agent-heretic-mlx-oq
- `nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF`（P1）：适合 reasoning/distillation 路线跟踪；风险是蒸馏教师、训练数据和评测未确认。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF

### 评测与基准

- `nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF`（P1）：适合纳入本地 reasoning 评测候选池；风险是候选信息未提供 benchmark，必须自测后才能比较。详情：https://my.feishu.cn/docx/QUmuddQSpoXqsyx5MiCcO7Rxntb | 原文：https://huggingface.co/nerkyor/Qwen3.6-35B-A3B-DSV4Pro-Thinking-Distill-GGUF
