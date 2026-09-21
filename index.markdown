---
layout: default
title: Willkommen
---
<img src="{{ site.baseurl }}/assets/Flageolett.webp" alt="Startbild" style="width: 100%; max-width: 100%; height: auto; display: block; margin-bottom: 2rem;">

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h1 class="post-title">
        <a href="{{ post.url | relative_url }}">
          {{ post.title }}
        </a>
      </h1>
      <time datetime="{{ post.date | date_to_xmlschema }}" class="post-date">
        {{ post.date | date_to_string }}
      </time>
      {{ post.content }}
    </article>
  {% endfor %}
</div>



