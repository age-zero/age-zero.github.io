---
layout: default
title: Age-Zero – Analysis
lang: de
---

# Age-Zero – Analysis

_Politik · Gesellschaft · Analysen_

---

## Deutsch

{% for post in site.posts %}
  {% if post.lang == "de" %}
### [{{ post.title }}]({{ post.url }})
<small>{{ post.date | date: "%d.%m.%Y" }}</small>

{{ post.excerpt | strip_html | truncate: 220 }}

---
  {% endif %}
{% endfor %}

## کوردی

{% for post in site.posts %}
  {% if post.lang == "ku-Arab" %}
### [{{ post.title }}]({{ post.url }})
<small>{{ post.date | date: "%d.%m.%Y" }}</small>

{{ post.excerpt | strip_html | truncate: 220 }}

---
  {% endif %}
{% endfor %}
