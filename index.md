---
layout: default
title: Age-Zero – Analysis
lang: ku-Arab
dir: rtl
---

<div class="index-page">

<h1>Age-Zero – Analysis</h1>
<p class="index-tagline">
  <span dir="ltr">Politik · Gesellschaft · Analysen</span>
  <span class="sep"> | </span>
  <span dir="rtl">سیاسەت · کۆمەڵگا · شیکاری</span>
</p>


<hr class="post-divider">

{% for post in site.posts %}
  {% if post.lang == "ku-Arab" %}
  <div class="index-post">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <time>{{ post.date | date: "%d.%m.%Y" }}</time>

    <div class="index-langs">
      {% if post.translations.de %}
        <a href="{{ post.translations.de }}">Deutsch</a>
      {% endif %}
      <a href="{{ post.url }}">کوردی</a>
    </div>

    <p>
      {% if post.description %}
        {{ post.description }}
      {% else %}
        {{ post.excerpt | strip_html | truncate: 150 }}
      {% endif %}
    </p>

  </div>
  <hr class="post-divider">
  {% endif %}

{% endfor %}

</div>
