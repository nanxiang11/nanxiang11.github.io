---
title: "Kaggle 树叶图像分类"
excerpt: "176 类、18k+ 训练样本的细粒度图像分类任务；最终进入前 10%，分类精度 98.27%。"
collection: portfolio
order: 70
type: "Competition"
status: "Top 10%"
image: "/images/project-kaggle-leaf.svg"
stats:
  - "176 Classes"
  - "18k+ Images"
  - "98.27% Acc"
tags:
  - Kaggle
  - Classification
  - ResNet50
  - ECA
---

针对树叶类别之间形态差异细微、类内变化明显的问题，对 ResNet50 进行结构和训练策略优化。

* 引入 Deformable Convolution 与轻量化 ECA 注意力，增强叶片细粒度特征表达。
* 结合 Label Smoothing、Focal Loss 以及 AdamW + CosineAnnealing 策略训练。
* 最终取得前 10% 名次，分类精度 98.27%。
