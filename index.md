---
layout: default
title: Age-Zero – Analysis
lang: de
---

<div class="index-page">

  <div class="index-intro">
    <h1>Age-Zero – Analysis</h1>
    <p class="index-subtitle">Politik · Gesellschaft · Analysen</p>
  </div>

  <hr class="index-divider">

  <section class="index-section">
    <!-- <h2>Deutsch</h2> -->
    {% for post in site.posts %}
      {% if post.lang == "de" %}
      <article class="index-post">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <time>{{ post.date | date: "%d.%m.%Y" }}</time>
        <p>{{ post.excerpt | strip_html | truncate: 220 }}</p>
      </article>
      {% endif %}
    {% endfor %}
  </section>

  <section class="index-section" dir="rtl">
    <!--<h2>کوردی</h2>-->
    {% for post in site.posts %}
      {% if post.lang == "ku-Arab" %}
      <article class="index-post">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <time>{{ post.date | date: "%d.%m.%Y" }}</time>
        <p>{{ post.excerpt | strip_html | truncate: 220 }}</p>
      </article>
      {% endif %}
    {% endfor %}
  </section>

</div>
