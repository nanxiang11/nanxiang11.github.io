---
layout: archive
title: "简历"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[下载 PDF 简历](/files/liuwenhao-cv.pdf){: .btn .btn--primary}

基本信息
======

* 姓名：刘文豪
* 方向：AI 算法工程师，具身智能 / 多模态 / 视觉感知
* 邮箱：liuwenhao1968@163.com
* GitHub：[github.com/nanxiang11](https://github.com/nanxiang11)
* Research Focus：具身智能、大模型多模态、视觉感知

教育背景
======

* 2023.09 - 2026.06，上海工程技术大学，电子信息硕士
* 研究方向：具身智能、大模型、多模态、轻量化语义分割、多尺度特征建模、工业视觉感知

科研与算法创新
======

* **V2Net: A Nested Framework for Crack Segmentation Based on Multiscale Feature Learning**
  * 第一作者，*IEEE Transactions on Instrumentation and Measurement*，Q1，IF 5.9。
  * 针对工业裂缝分割中目标尺度变化剧烈、细粒度结构易在多次下采样中丢失的问题，从特征组织结构层面分析 UNet / UNet++ 的冗余融合与语义错位。
  * 提出嵌套式多尺度特征学习框架 V2Net，将网络拆解为多个 VNet 子结构，并通过匹配式跳跃连接进行跨尺度语义对齐和特征复用。
  * 设计渐进式特征增强机制，强化裂缝方向性和细粒度几何特征表达。
  * 在 KHANHHAS 等裂缝数据集上取得领先效果，相较 UNet 基线提升 41.69% IoU，相较 CrackSAM 在 CSBSR 指标上分别提升 1.56% 与 1.21% IoU。

* **HAFNet: Hierarchical Attention and Feature Fusion for Real-Time Lightweight Semantic Segmentation**
  * 第一作者，*IEEE TPAMI* Under Review，Q1，IF 18.6。
  * 从浅层、中层和深层特征的功能划分出发，构建分层协同的轻量化语义分割架构。
  * 设计 AcquisitionFeature、MS-ACSBlock 和 GeoLiteConv 等模块，分别强化边界纹理、局部结构和全局语义建模。
  * 在 Crack500、MIAD、WHDLD、Cityscapes 等数据集上系统评测；在 WHDLD 场景中以 1.98 GFLOPs 和 1.19M 参数达到 63.17% mIoU。

实习经历
======

* **商汤科技 SenseTime，算法实习生**，2025.04 - 2025.11
  * 具身智能无人零售系统：基于 π0.5 模型进行零售场景适配，构建指令-动作数据和遥操作采集流程，参与视觉检测结果与 Prompt 融合策略设计，并对接导航模块完成关键流程端到端打通。
  * 图像质量分类模型：设计半自动化数据生成闭环，结合传统退化模拟与风格迁移生成数据，优化 EfficientNetV2 训练与千万级推理流程；生成 100w+ 高质量训练图像，测试集准确率达到 99.7%。
  * 人体图像分割数据集生成引擎：构建人工标注、SegFormer 初训练、SAM 批量生成 mask、自动化质量分类和人工筛选的迭代闭环，提升智能冰箱场景的人体分割与结算稳定性。
  * 商品货架旋转检测优化：通过损失函数、样本增强、数据加载和缩放策略优化，线上方案提升 6.5% 检测准确率和 3.1% 召回率；同时验证分割方案兼容旋转检测输出格式。

* **首形科技，具身智能算法实习生**，2025.12 - 2026.01
  * 研发具身智能多模态情感交互系统，基于 Qwen3 微调构建情感感知对话模型。
  * 设计情感提示词体系，将文本语义映射为 8 维情绪向量，并建立 LLM 情绪向量到 TTS 的控制链路。
  * 完成 LLM 生成、情感解析、情绪向量映射和 TTS 合成的实时推理闭环，支持情绪强度调节和混合表达。

项目经历
======

* **星语 MoE：自研 MoE 架构大模型**
  * GitHub：[CodeLab_LLM](https://github.com/nanxiang11/CodeLab_LLM)
  * ModelScope：[XY-MoE](https://www.modelscope.cn/studios/nanxiang1968/XY-MoE)
  * 从零实现 LLaMA3 Attention、FFN、RMSNorm、Rotary Embedding 等核心模块，支持预训练、SFT 和 LoRA 微调；0.2B 参数量模型可在 CPU 环境推理约 10 token/s。

* **星语 Vision：自研多模态大模型**
  * ModelScope：[XY-Vision](https://www.modelscope.cn/studios/nanxiang1968/XY-Vision/summary)
  * 基于 CLIP 视觉编码器实现视觉 token 替换策略，将图像信息融入文本 Transformer，完成端到端图像-文本推理闭环。

* **星语 pi0：VLA 模型源码拆解与最小复现**
  * GitHub：[XY_Pi0](https://github.com/nanxiang11/XY_Pi0)
  * 拆解视觉编码、语言建模与动作预测模块，手动复现 attention、位置编码和多模态融合等关键组件，跟踪 forward / loss / 推理流程。

竞赛与荣誉
======

* 国家级：研究生数学建模国家二等奖（队长）、CAAI 智新杯国家二等奖、机器人与人工智能国家三等奖、研究生国家奖学金。
* 省市级：江西省工程训练省二等奖（队长）、机器人大赛省三等奖、上海市双创市级立项。
* 校级：研究生学业奖学金排名第一、数学建模校二等奖、互联网+ 校三等奖、程创杯校三等奖、三好学生、机械创新校一等奖。
* Kaggle 树叶图像分类：176 类、18k+ 训练样本，基于 ResNet50、Deformable Convolution、ECA 注意力、Label Smoothing、Focal Loss 和 AdamW + CosineAnnealing，最终前 10%，分类精度 98.27%。
* 2018 Data Science Bowl 细胞核分割：改进 U-Net，引入 Deformable Convolution、密集跳跃连接、复合损失和强数据增强，IoU 57.21%，排名前 5%。

技能关键词
======

* 具身智能：VLA、遥操作数据、指令-动作建模、系统联调。
* 多模态与大模型：Transformer、MoE、LoRA、CLIP、Qwen、Prompt Engineering、LLM + TTS。
* 视觉算法：语义分割、裂缝分割、人体分割、目标检测、旋转检测、图像质量分类。
* 工程能力：数据生成闭环、模型训练推理、百万级数据训练、千万级数据推理、端到端落地验证。
