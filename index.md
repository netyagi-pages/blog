---
layout: default
title: Home
---

<h1 class="home-title">記事一覧</h1>

<ul class="entry-list">
  <li class="entry-list__item">
    <a class="entry-list__link" href="{{ '/about/' | relative_url }}">このサイトについて</a>
  </li>
  {% for post in site.posts %}
    <li class="entry-list__item">
      <a class="entry-list__link" href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
