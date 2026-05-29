---
permalink: /
title: "刘文豪"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<section class="lw-hero">
  <p class="lw-eyebrow">AI Algorithm Engineer · Embodied AI · Multimodal Perception</p>
  <h1>把具身智能、多模态模型和视觉感知落到真实任务里。</h1>
  <p class="lw-hero-lead">上海工程技术大学电子信息硕士，研究方向聚焦 VLA/具身智能系统、轻量化语义分割、多尺度特征建模与工业视觉感知。我更关注模型结构、数据闭环和工程落地之间的连接。</p>
  <div class="lw-actions">
    <a class="btn" href="https://github.com/nanxiang11">GitHub</a>
    <a class="btn" href="/portfolio/">查看项目</a>
  </div>
</section>

<section class="lw-metrics" aria-label="关键成果">
  <div class="lw-metric">
    <span class="lw-metric-value">2</span>
    <span class="lw-metric-label">第一作者科研工作</span>
  </div>
  <div class="lw-metric">
    <span class="lw-metric-value">76+</span>
    <span class="lw-metric-label">CodeLab_LLM GitHub Stars</span>
  </div>
  <div class="lw-metric">
    <span class="lw-metric-value">Top 8</span>
    <span class="lw-metric-label">RoboChallenge ICRA 2026</span>
  </div>
  <div class="lw-metric">
    <span class="lw-metric-value">99.7%</span>
    <span class="lw-metric-label">图像质量分类测试准确率</span>
  </div>
</section>

<section class="lw-section">
  <div class="lw-section-head">
    <p class="lw-eyebrow">Research Focus</p>
    <h2>研究方向</h2>
  </div>
  <div class="lw-focus-grid">
    <article class="lw-card">
      <h3>具身智能与 VLA</h3>
      <p>视觉-语言-动作建模、遥操作数据采集、指令到动作序列决策，以及真实系统联调。</p>
    </article>
    <article class="lw-card">
      <h3>多模态大模型</h3>
      <p>图文联合推理、视觉 token 融合、MoE/LoRA 训练推理闭环，以及 LLM 情绪到 TTS 控制链路。</p>
    </article>
    <article class="lw-card">
      <h3>视觉感知算法</h3>
      <p>裂缝分割、轻量化语义分割、旋转检测、人体分割与工业场景数据闭环。</p>
    </article>
  </div>
</section>

<section class="lw-section">
  <div class="lw-section-head">
    <p class="lw-eyebrow">Selected Work</p>
    <h2>精选成果</h2>
  </div>
  <div class="lw-feature-list">
    {% assign featured_video_projects = site.portfolio | sort: "order" %}
    {% for post in featured_video_projects %}
      {% if post.videos %}
        <article class="lw-feature lw-feature--video">
          <div>
            <p class="lw-feature-type">{{ post.type }} · Video Demo</p>
            <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
            <p>{{ post.excerpt | strip_html }}</p>
            {% if post.stats %}
              <div class="lw-mini-stats">
                {% for stat in post.stats %}
                  <span>{{ stat }}</span>
                {% endfor %}
              </div>
            {% endif %}
          </div>
          <div class="lw-feature-video-strip" aria-label="{{ post.title }} 视频预览">
            {% for video in post.videos %}
              <div class="lw-mini-video-card">
                <video autoplay muted loop playsinline preload="metadata" poster="{{ video.poster }}">
                  <source src="{{ video.src }}" type="video/mp4">
                </video>
                <span>{{ video.title }}</span>
              </div>
            {% endfor %}
          </div>
          <a class="lw-feature-link" href="{{ post.url }}#robot-demos">详情</a>
        </article>
      {% endif %}
    {% endfor %}
    <article class="lw-feature">
      <div>
        <p class="lw-feature-type">Publication</p>
        <h3><a href="/publication/v2net-crack-segmentation">V2Net: Nested Multiscale Crack Segmentation</a></h3>
        <p>面向工业裂缝分割的嵌套式多尺度特征学习框架，第一作者发表于 <em>IEEE TIM</em>。</p>
      </div>
      <a class="lw-feature-link" href="https://github.com/nanxiang11/NxV2net">Code</a>
    </article>
    <article class="lw-feature">
      <div>
        <p class="lw-feature-type">Project</p>
        <h3><a href="https://github.com/nanxiang11/CodeLab_LLM">CodeLab_LLM / 星语 MoE</a></h3>
        <p>从零实现 LLaMA 核心模块、MoE-FFN、预训练、SFT 与 LoRA，形成大模型最小闭环。</p>
      </div>
      <a class="lw-feature-link" href="/portfolio/">Projects</a>
    </article>
    <article class="lw-feature">
      <div>
        <p class="lw-feature-type">Competition</p>
        <h3><a href="/competitions/">RoboChallenge ICRA Competition 2026</a></h3>
        <p>Dexmal WBC Track 第 8 名，任务聚焦零售超市场景中的指令理解、导航和抓取操作。</p>
      </div>
      <a class="lw-feature-link" href="https://robochallenge.cn/competition/icra">Official</a>
    </article>
  </div>
</section>

<section class="lw-section">
  <div class="lw-section-head">
    <p class="lw-eyebrow">Experience</p>
    <h2>工程经历</h2>
  </div>
  <div class="lw-timeline">
    <article>
      <span>2025.04 - 2025.11</span>
      <h3>商汤科技 SenseTime · 算法实习生</h3>
      <p>参与具身智能无人零售系统、图像质量分类、人体分割数据生成引擎和商品货架旋转检测优化，覆盖数据构建、模型训练、推理评估到系统联调。</p>
    </article>
    <article>
      <span>2025.12 - 2026.01</span>
      <h3>首形科技 · 具身智能算法实习生</h3>
      <p>研发多模态情感交互系统，基于 Qwen3 微调、情感提示词体系和 LLM 到 TTS 的情绪向量控制链路完成工程落地。</p>
    </article>
  </div>
</section>
