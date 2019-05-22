---
layout: default
title: Blog
---

# Recent blog posts:

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
* [{{ post.title }}]({{ post.url }})
  {%- endfor %}
{% endif %}
