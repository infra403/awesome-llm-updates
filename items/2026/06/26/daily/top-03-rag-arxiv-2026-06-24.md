---
type: IntelItem
title: "RAG 安全与隐私综述：把检索索引、查询日志、上下文构造纳入威胁面"
date: "2026-06-26"
language: zh-CN
importance: P0
tags: [rag, evals, safety, llm-infra]
source: "../../../../../archive/2026/06/26/digest/20260626-0936/daily.md"
window: daily
---

# RAG 安全与隐私综述：把检索索引、查询日志、上下文构造纳入威胁面

## 摘要

**RAG 安全与隐私综述：把检索索引、查询日志、上下文构造纳入威胁面**：核心变化是 arXiv 2026-06-24 当前窗口候选给出 RAG 安全/隐私系统综述，强调风险不只在生成模型本身，也在检索 pipeline、索引、日志和 context construction；工程影响是企业 RAG 需要补齐数据分级、索引隔离、日志脱敏、检索权限和 prompt/context 泄露测试，而不是只做答案安全过滤；建议动作：**今天应阅读**，适合作为 RAG 安全 checklist 的输入；证据边界：候选确认论文主题和摘要，未确认综述覆盖的防御成熟度或是否有可执行工具；

## P级别依据

P0：命中 RAG / Knowledge、评测 / Benchmarks、安全 / Alignment，包含可直接核验的源链接；可能影响近期工程选型、架构约束或评测优先级。

## 工程影响

进入模型候选池前先验证 license、chat template、推理吞吐、显存、部署兼容性和内部 prompt regression。

## 来源

- [每日 digest](../../../../../archive/2026/06/26/digest/20260626-0936/daily.md)

## 来源链接

- [arXiv: 2606.25533v1](https://arxiv.org/abs/2606.25533v1)
