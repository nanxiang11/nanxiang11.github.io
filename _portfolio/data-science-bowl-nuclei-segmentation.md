---
title: "2018 Data Science Bowl：细胞核分割"
excerpt: "改进 U-Net 进行细胞核实例分割，结合 Deformable Convolution、密集跳跃连接和强数据增强，最终排名前 5%。"
collection: portfolio
order: 80
type: "Competition"
status: "Top 5%"
image: "/images/project-dsb-nuclei.svg"
stats:
  - "57.21% IoU"
  - "U-Net"
  - "Dense Skip"
tags:
  - Kaggle
  - Segmentation
  - U-Net
  - Medical Image
---

该项目面向细胞核形态复杂、尺度差异明显的医学图像分割任务。

* 在 U-Net 基础上引入 Deformable Convolution 和密集跳跃连接。
* 结合复合损失函数与强数据增强，提升核形态和尺度建模能力。
* 比赛 IoU 达到 57.21%，最终排名前 5%。
