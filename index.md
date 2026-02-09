---
layout: default
title: Home
---

# {{ site.title }}

{{ site.description }}

---

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
<small>{{ post.date | date: "%d.%m.%Y" }}</small>

{{ post.excerpt }}

---
{% endfor %}
