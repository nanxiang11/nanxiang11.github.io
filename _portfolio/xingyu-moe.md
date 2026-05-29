---
title: "星语 MoE：自研 MoE 架构大模型"
excerpt: "从零实现 LLaMA/LLaMA3 核心模块与 MoE-FFN 替换策略，构建可训练、可推理的大模型最小闭环。"
collection: portfolio
link: "https://github.com/nanxiang11/CodeLab_LLM"
order: 10
type: "Large Language Model"
status: "Open Source"
image: "/images/project-codelab-llm.svg"
stats:
  - "76+ Stars"
  - "0.2B Parameters"
  - "CPU 10 token/s"
tags:
  - Transformer
  - MoE
  - LoRA
  - PyTorch
links:
  - label: "GitHub"
    url: "https://github.com/nanxiang11/CodeLab_LLM"
  - label: "ModelScope"
    url: "https://www.modelscope.cn/studios/nanxiang1968/XY-MoE"
---

项目链接：[GitHub](https://github.com/nanxiang11/CodeLab_LLM)；在线体验：[ModelScope](https://www.modelscope.cn/studios/nanxiang1968/XY-MoE)。

这个项目以快速理解 Transformer 与 MoE 原理为目标，在约一周内完成可训练、可推理的大模型最小闭环。

* 从零实现 LLaMA / LLaMA3 核心模块，包括 Attention、FFN、RMSNorm 和 Rotary Embedding。
* 设计 MoE-FFN 替换策略，使 0.2B 参数量模型在 CPU 环境可推理，速度约 10 token/s。
* 支持预训练、SFT 与 LoRA 微调流程，完成从结构实现到训练调试、推理验证的完整链路。
