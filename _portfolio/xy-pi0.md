---
title: "星语 pi0：VLA 模型源码拆解与最小复现"
excerpt: "围绕 pi0 源码构建最小可运行 VLA 系统，拆解视觉编码、语言建模和动作预测模块。"
collection: portfolio
link: "https://github.com/nanxiang11/XY_Pi0"
---

项目链接：[GitHub](https://github.com/nanxiang11/XY_Pi0)。

该项目围绕 VLA 模型进行源码级理解和最小复现，目标是从“调用模型”深入到“实现模型”。

* 系统拆解视觉编码、语言建模与动作预测模块，梳理多模态 token 组织与特征流动。
* 手动复现 attention、位置编码和多模态融合等关键组件。
* 跟踪 forward / loss / 推理流程，验证视觉-语言-动作建模的数据流。
