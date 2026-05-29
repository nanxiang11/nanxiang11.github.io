---
layout: archive
title: "竞赛"
permalink: /competitions/
author_profile: true
---

{% include base_path %}

<section class="lw-page-intro">
  <p class="lw-eyebrow">Competitions</p>
  <h1>比赛专项</h1>
  <p>竞赛经历按具身智能、AI 算法、数学建模和视觉任务组织，突出排名、角色和技术关键词。</p>
</section>

{% assign featured = site.data.competitions | where: "featured", true %}
{% for item in featured %}
<section class="lw-competition-hero">
  <div>
    <p class="lw-eyebrow">Featured Competition</p>
    <h2>{{ item.title }}</h2>
    <p>{{ item.detail }}</p>
    <div class="lw-tags">
      <span>{{ item.subtitle }}</span>
      <span>{{ item.focus }}</span>
    </div>
    <div class="lw-card-actions">
      {% for link in item.links %}
        <a href="{{ link.url }}" target="_blank" rel="noopener">{{ link.label }}</a>
      {% endfor %}
    </div>
  </div>
  <aside>
    <span class="lw-rank-label">Result</span>
    <strong>{{ item.result }}</strong>
    <p>{{ item.role }} · {{ item.date }}</p>
    {% if item.metrics %}
      <div class="lw-mini-stats">
        {% for metric in item.metrics %}
          <span>{{ metric }}</span>
        {% endfor %}
      </div>
    {% endif %}
  </aside>
</section>
{% endfor %}

<div class="lw-competition-grid">
  {% for item in site.data.competitions %}
    {% unless item.featured %}
    <article class="lw-competition-card">
      <div class="lw-card-meta">
        <span>{{ item.date }}</span>
        <span>{{ item.role }}</span>
      </div>
      <h2>{{ item.title }}</h2>
      <p class="lw-competition-subtitle">{{ item.subtitle }}</p>
      <strong>{{ item.result }}</strong>
      <p>{{ item.detail }}</p>
      <div class="lw-tags">
        <span>{{ item.focus }}</span>
      </div>
    </article>
    {% endunless %}
  {% endfor %}
</div>
