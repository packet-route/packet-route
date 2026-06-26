---
layout: page
title: "Class 2025-2026"
permalink: /packet-feed/2025-2026/
---

{% assign year_posts = site.posts | where: "class", "2025-2026" %}
{% for post in year_posts %}
<article style="margin-bottom: 1.5em;">
  <h3 style="margin-bottom: 0.2em;">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h3>
  <p style="color: #666; font-size: 0.9em; margin: 0;">
    {% if post.author %}{{ post.author }}{% endif %}
  </p>
</article>
{% endfor %}
