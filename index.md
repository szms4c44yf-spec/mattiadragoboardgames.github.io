---
layout: page
title: "Ultimi articoli"
permalink: /
---

<div class="hero">
  <div class="hero__inner">
    <h1>Mattia Drago Board Games</h1>
    <p>Analisi dei giochi da tavolo: origini &amp; contesto, scelte di design, persone &amp; storie, impatto sociale.</p>
    <a class="btn btn-cta" href="#articoli">Vai agli articoli</a>
  </div>
</div>

## Ultimi articoli {#articoli}

<div class="posts-grid">
{% for post in site.posts limit: 12 %}
  <a class="post-card__link" href="{{ post.url | relative_url }}">
    <article class="post-card">
      <div class="post-card__thumb" style="--bg: url('{{ post.image | default: '/assets/cover-fallback.svg' | relative_url }}');"></div>
      <div class="post-card__body">
        <p class="post-card__meta">{{ post.date | date: "%b %e, %Y" }}</p>
        <h3 class="post-card__title">{{ post.title }}</h3>
        {% if post.excerpt %}
          <p class="post-card__excerpt">{{ post.excerpt | strip_html | truncate: 120 }}</p>
        {% endif %}
      </div>
    </article>
  </a>
{% endfor %}
</div>

<div class="scales-footer"></div>
