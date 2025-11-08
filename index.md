---
layout: page
title: "Ultimi articoli"
permalink: /
---

<div class="hero">
  <div class="hero__inner">
    <h1>Mattia Drago Board Games</h1>
    <p>Analisi di giochi da tavolo: origini & contesto, scelte di design, persone & storie, impatto sociale.</p>
    <a class="btn-cta" href="#post-list">Vai agli articoli</a>
  </div>
</div>

<h2 id="post-list" style="margin-top:0.5rem;">Ultimi articoli</h2>

<div class="posts-grid">
{% for post in site.posts limit: 12 %}
  <article class="post-card">
    <a class="post-card__link" href="{{ post.url | relative_url }}">
      <div class="post-card__thumb" style="--bg: url('{{ post.image | default: "/assets/cover-fallback.svg" }}')"></div>
      <div class="post-card__body">
        <div class="post-card__meta">{{ post.date | date: "%b %-d, %Y" }}</div>
        <h3 class="post-card__title">{{ post.title }}</h3>
        <p class="post-card__excerpt">
          {{ post.excerpt | default: post.content | strip_html | truncate: 140 }}
        </p>
      </div>
    </a>
  </article>
{% endfor %}
</div>
