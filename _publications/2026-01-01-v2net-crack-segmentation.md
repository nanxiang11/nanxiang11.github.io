---
title: "V2Net: A Nested Framework for Crack Segmentation Based on Multiscale Feature Learning"
collection: publications
category: manuscripts
permalink: /publication/v2net-crack-segmentation
excerpt: "面向工业裂缝分割的嵌套式多尺度特征学习框架，通过 VNet 子结构、匹配式跳跃连接和渐进式特征增强改善尺度变化与细粒度结构表达。"
date: 2026-01-01
venue: "IEEE Transactions on Instrumentation and Measurement"
status: "第一作者"
image: "/images/publications/v2net-architecture.png"
citation: "Wenhao Liu. &quot;V2Net: A Nested Framework for Crack Segmentation Based on Multiscale Feature Learning.&quot; <i>IEEE Transactions on Instrumentation and Measurement</i>."
tags:
  - Crack Segmentation
  - Multiscale Learning
  - VNet
  - Industrial Vision
stats:
  - "Q1 / IF 5.9"
  - "66.51% IoU"
  - "+41.69% vs UNet"
links:
  - label: "GitHub"
    url: "https://github.com/nanxiang11/NxV2net"
---

V2Net 面向工业裂缝分割中目标尺度变化剧烈、细粒度结构易在多次下采样中丢失的问题，从特征组织结构层面分析 UNet / UNet++ 在多尺度建模上的冗余融合与语义错位问题。

## 网络结构图

<figure>
  <img src="/images/publications/v2net-architecture.png" alt="V2Net 网络结构图" loading="lazy">
  <figcaption>V2Net 网络结构图。</figcaption>
</figure>

主要贡献包括：

* 提出嵌套式多尺度特征学习框架，将网络拆解为多个 VNet 子结构，并通过匹配式跳跃连接实现跨尺度单元的语义对齐与特征复用。
* 设计面向裂缝方向性与细粒度几何特征的渐进式特征增强机制，缓解多尺度融合过程中的关键信息衰减。
* 在多个裂缝数据集上优于 UNet、UNet++ 等主流方法；在 KHANHHAS 数据集上，相较 UNet 基线提升 41.69% IoU，相较 CrackSAM 在 CSBSR 指标上分别提升 1.56% 与 1.21% IoU。
