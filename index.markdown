---
layout: default
title: Willkommen
---
<img src="{{ site.baseurl }}/assets/Flageolett.webp" alt="Startbild" style="width: 100%; max-width: 100%; height: auto; display: block; margin-bottom: 2rem;">

<div class="posts">
  {% for post in site.posts %}
  <div class="post" style="margin-bottom: 1.5rem;">
    <h2 class="post-title">
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </h2>
<span class="post-date" style="font-size: 0.85rem; color: #9a9a9a; display: block;">
  {{ post.date | date: "%d.%m.%Y" }}
</span>

  </div>
  {% endfor %}
</div>

