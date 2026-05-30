---
title: "HAFNet: Hierarchical Attention and Feature Fusion for Real-Time Lightweight Semantic Segmentation"
collection: publications
category: manuscripts
permalink: /publication/hafnet-lightweight-semantic-segmentation
excerpt: "实时轻量化语义分割网络，基于浅层边界、中层结构与深层语义的层级功能划分，结合注意力与多尺度特征融合提升复杂场景分割效果。"
date: 2026-02-01
venue: "IEEE Transactions on Pattern Analysis and Machine Intelligence"
status: "第一作者，Under Review"
image: "/images/publications/hafnet-architecture.png"
citation: "Wenhao Liu. &quot;HAFNet: Hierarchical Attention and Feature Fusion for Real-Time Lightweight Semantic Segmentation.&quot; <i>IEEE Transactions on Pattern Analysis and Machine Intelligence</i>, Under Review."
tags:
  - Lightweight Segmentation
  - Attention
  - Feature Fusion
  - Real-Time
stats:
  - "Under Review"
  - "1.19M Params"
  - "1.98 GFLOPs"
links:
  - label: "GitHub"
    url: "https://github.com/nanxiang11/HAFNet"
---

HAFNet 从语义分割网络的层级功能划分出发，分析浅层、中层与深层特征在边界建模、结构感知与语义抽象中的不同作用，针对传统轻量化模型多尺度协同不足的问题进行结构设计。

## 网络结构图

<figure>
  <img src="/images/publications/hafnet-architecture.png" alt="HAFNet 网络结构图" loading="lazy">
  <figcaption>HAFNet 网络结构图。</figcaption>
</figure>

主要贡献包括：

* 提出分层协同的轻量化语义分割架构，明确不同层级特征的功能分工。
* 在浅层设计 AcquisitionFeature 模块，强化边缘和纹理等低级特征提取并抑制冗余信息。
* 在中层设计 MS-ACSBlock，融合多尺度建模与注意力机制，提升局部结构与目标轮廓感知能力。
* 在深层设计 GeoLiteConv 模块，增强语义抽象与全局上下文建模能力。
* 在 Crack500、MIAD、WHDLD 和 Cityscapes 等数据集上评测；在 WHDLD 遥感航拍场景中以 1.98 GFLOPs、1.19M 参数达到 63.17% mIoU。
