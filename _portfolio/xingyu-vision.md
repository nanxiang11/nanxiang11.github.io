---
title: "星语 Vision：自研多模态大模型"
excerpt: "基于 CLIP 视觉编码器和文本 Transformer 的图像-文本联合推理系统，完成多模态最小可验证闭环。"
collection: portfolio
link: "https://www.modelscope.cn/studios/nanxiang1968/XY-Vision/summary"
---

在线体验：[ModelScope](https://www.modelscope.cn/studios/nanxiang1968/XY-Vision/summary)。

星语 Vision 以图像-文本联合推理为目标，验证从视觉编码、token 融合到文本生成的多模态系统链路。

* 基于 CLIP 视觉编码器提取图像表征。
* 实现视觉 token 替换策略，将图像信息融入文本 Transformer 模型。
* 完成端到端图像-文本推理验证，并支持预训练、SFT 与 LoRA 微调流程。
