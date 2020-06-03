---
layout: default
---

<div class="intro">
  <img src="images/avatar.png" alt="Ian Kynnersley">

  <h1>Hello,<br>I'm Ian</h1>
</div>

I'm an experienced technical leader and startup CTO who helps organisations big and small use technology to make great things.

[You can read more about me here](/about).

## Work

I specialise in turning business ideas into beautiful products. Here are some of the projects I've been working on in recent years:

* &raquo; Technical Lead at Overlay (2019 - 2020) – case study coming soon
* &raquo; [CTO at Provenance](/case_studies/provenance) (2014 - 2019)
* &raquo; [Product strategy at Raremark](/case_studies/raremark) (2015)
* &raquo; [Product Owner at Adaptive Lab](/case_studies/adaptive_lab) (2014 - 2015)
* &raquo; [Freelance CTO at Doing Something](/case_studies/doing_something) (2014)

## Writing

Occasional thoughts about startups and technology, usually intended for small tech business owners:

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
* &raquo; [{{ post.title }}]({{ post.url }})
  {%- endfor %}
{% endif %}
