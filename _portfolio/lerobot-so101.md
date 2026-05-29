---
title: "LeRobot pi0.5 + SO-101：双任务机械臂操作"
excerpt: "基于 LeRobot 与 pi0.5 策略框架，在 SO-101 机械臂上完成叠毛巾与清理桌面两个真实桌面操作任务，验证从数据采集、策略学习到实体执行的闭环。"
collection: portfolio
order: 35
type: "Embodied AI"
status: "Robot Demo"
image: "/images/project-lerobot-so101.svg"
stats:
  - "2 Real Tasks"
  - "SO-101 Arm"
  - "LeRobot / pi0.5"
tags:
  - LeRobot
  - pi0.5
  - SO-101
  - Robot Manipulation
---

该项目围绕真实桌面场景下的机器人操作展开，使用 LeRobot 的数据与训练流程，结合 pi0.5 策略框架，在 SO-101 机械臂上完成两个不同类型的任务：叠毛巾与清理桌面。项目重点不是单一动作演示，而是验证“采集数据 - 训练策略 - 实体执行 - 观察误差”的完整闭环。

* 叠毛巾任务关注柔性物体操作，需要机械臂在接触不确定、布料形变明显的情况下完成抓取、拖拽、对齐与折叠。
* 清理桌面任务关注杂物场景中的目标定位和连续抓取，需要机械臂将桌面上的分散物体移动到指定区域。
* 两个任务共同覆盖了刚性物体整理与柔性物体操作，能够更全面地检验策略的空间泛化、动作连续性和真实执行稳定性。

<section class="lw-video-showcase" aria-label="LeRobot SO-101 video demonstrations">
  <div class="lw-section-head">
    <p class="lw-eyebrow">Robot Demos</p>
    <h2>真实机械臂任务演示</h2>
  </div>
  <div class="lw-video-grid">
    <article class="lw-video-card">
      <div class="lw-video-frame">
        <video controls playsinline preload="metadata" poster="/images/projects/lerobot-so101-towel-folding.jpg">
          <source src="/files/videos/lerobot-so101-towel-folding.mp4" type="video/mp4">
        </video>
      </div>
      <div class="lw-video-body">
        <p class="lw-feature-type">Task 01</p>
        <h3>叠毛巾</h3>
        <p>面向柔性物体的桌面操作任务，机械臂需要在布料形变和接触误差存在的情况下完成抓取、牵引和折叠动作。</p>
        <div class="lw-tags">
          <span>Deformable Object</span>
          <span>Contact-rich Manipulation</span>
          <span>SO-101</span>
        </div>
      </div>
    </article>
    <article class="lw-video-card">
      <div class="lw-video-frame">
        <video controls playsinline preload="metadata" poster="/images/projects/lerobot-so101-table-cleaning.jpg">
          <source src="/files/videos/lerobot-so101-table-cleaning.mp4" type="video/mp4">
        </video>
      </div>
      <div class="lw-video-body">
        <p class="lw-feature-type">Task 02</p>
        <h3>清理桌面</h3>
        <p>面向非结构化桌面的整理任务，机械臂根据目标物体位置执行连续抓取与放置，将分散物体移动到指定区域。</p>
        <div class="lw-tags">
          <span>Tabletop Manipulation</span>
          <span>Sequential Grasping</span>
          <span>Real Robot</span>
        </div>
      </div>
    </article>
  </div>
</section>

<section class="lw-section">
  <div class="lw-section-head">
    <p class="lw-eyebrow">Implementation Notes</p>
    <h2>技术要点</h2>
  </div>
  <div class="lw-focus-grid">
    <article class="lw-card">
      <h3>数据闭环</h3>
      <p>围绕真实机械臂采集任务数据，关注动作序列、末端执行器状态和视觉观测之间的对齐关系。</p>
    </article>
    <article class="lw-card">
      <h3>策略执行</h3>
      <p>基于 LeRobot / pi0.5 训练与推理流程，将桌面任务从离线样本推进到实体机械臂执行。</p>
    </article>
    <article class="lw-card">
      <h3>任务泛化</h3>
      <p>通过清理桌面和叠毛巾两个任务，分别覆盖刚性物体移动和柔性物体操作两类典型挑战。</p>
    </article>
  </div>
</section>
