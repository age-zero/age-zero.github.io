---
layout: default
title: Age-Zero – Analysis
lang: de
---

<div class="index-page">

<h1>Age-Zero – Analysis</h1>
<p class="index-tagline">Politik · Gesellschaft · Analysen</p>

<hr class="post-divider">

{% assign german_posts = site.posts | where: "lang", "de" %}

{% for post in german_posts %}
<div class="index-post">

  <h2>{{ post.title }}</h2>
  <time>{{ post.date | date: "%d.%m.%Y" }}</time>

  <div class="index-langs">
    <a href="{{ post.url }}">Deutsch</a>

    {% if post.translations.ku %}
      · <a href="{{ post.translations.ku }}">کوردی</a>
    {% endif %}
  </div>

  <p>
    {{ post.excerpt | strip_html | truncate: 240 }}
  </p>

</div>

<hr class="post-divider">
{% endfor %}

</div>
