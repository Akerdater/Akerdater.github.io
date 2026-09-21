---
layout: default
title: Willkommen
---
<img src="{{ site.baseurl }}/assets/Flageolett.webp" alt="Startbild" style="width: 100%; max-width: 100%; height: auto; display: block; margin-bottom: 2.5rem;">

<h1 style="margin-top: 0; margin-bottom: 20px; font-size: 2rem;">Herzlich Willkommen!</h1>

<h2 style="margin-top: 50px; margin-bottom: 15px; font-size: 1.5rem; font-weight: normal; color: #303030;">Aktuelle Beiträge:</h2>

<div class="posts">
  {% for post in site.posts %}
  <div class="post">
    
    <h3 class="post-title" style="margin-top: 15px !important; margin-bottom: 0 !important; font-size: 1.3rem; line-height: 1.2;">
      <!-- FIX: Das Link-Element darf nach unten keinen Abstand erzeugen -->
      <a href="{{ post.url | relative_url }}" style="margin-bottom: 0 !important; display: inline-block;">
        {{ post.title }}
      </a>
    </h3>
    
    <!-- Das Datum rückt über ein kleines margin-top jetzt ganz nah an den Text -->
    <span class="post-date" style="font-size: 0.85rem; color: #9a9a9a; display: block; margin-top: 2px !important;">
      {{ post.date | date: "%d.%m.%Y" }}
    </span>

  </div>
  {% endfor %}
</div>

<!-- DIESER TRICK HÄLT DEN ABSTAND ZWISCHEN DEN BEITRÄGEN COMPAKT -->
<style>
  .posts .post {
    margin-bottom: 15px !important;
    padding-bottom: 0 !important;
  }
</style>


