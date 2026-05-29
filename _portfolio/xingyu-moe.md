---
title: "星语 MoE：自研 MoE 架构大模型"
excerpt: "0.2B 参数量、CPU 可推理的大模型最小闭环实践；从零实现 LLaMA3 核心模块，支持预训练、SFT 与 LoRA。"
collection: portfolio
link: "https://github.com/nanxiang11/CodeLab_LLM"
---

项目链接：[GitHub](https://github.com/nanxiang11/CodeLab_LLM)；在线体验：[ModelScope](https://www.modelscope.cn/studios/nanxiang1968/XY-MoE)。

这个项目以快速理解 Transformer 与 MoE 原理为目标，在约一周内完成可训练、可推理的大模型最小闭环。

* 从零实现 LLaMA3 核心模块，包括 Attention、FFN、RMSNorm 和 Rotary Embedding。
* 设计 MoE-FFN 替换策略，使 0.2B 参数量模型在 CPU 环境可推理，速度约 10 token/s。
* 支持预训练、SFT 与 LoRA 微调流程，完成从结构实现到训练调试、推理验证的完整链路。
