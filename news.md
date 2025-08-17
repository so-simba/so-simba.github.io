---
layout: page
title: News
permalink: /news/
---

{% assign news_posts = site.posts | where_exp: "p", "p.categories contains 'news'" %}
{% for post in news_posts %}
  <article class="news-entry">
    <h3>{{ post.title }}</h3>
    <p class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</p>
    <div class="post-content">
      {{ post.content }}
    </div>
  </article>
{% endfor %}

{% if news_posts == empty %}
  <p>No news yet. Check back soon.</p>
{% endif %}
