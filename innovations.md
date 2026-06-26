---
layout: page
title: Innovation Feed
permalink: /innovations/
---

Computing innovations covered in the AP CSP curriculum. Each entry examines a technology's purpose, the data it uses, and its beneficial and harmful effects.

<ul>
{% for item in site.innovations %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>
