---
layout: page
title: News
permalink: /news/
---

<ul class="post-list">
  {% assign news_posts = site.posts | where_exp: "p", "p.categories contains 'news'" %}
  {% for post in news_posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title }}
        </a>
      </h3>
      {% if post.excerpt %}
        <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
      {% endif %}
    </li>
  {% endfor %}
  {% if news_posts == empty %}
    <p>No news yet. Check back soon.</p>
  {% endif %}
</ul>
