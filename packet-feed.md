---
layout: page
title: Packet Feed
permalink: /packet-feed/
---

Student-created artifacts, archived by class year.

{% assign posts_by_class = site.posts | group_by: "class" %}
{% for year in posts_by_class %}
## Class {{ year.name }}
<ul>
{% for post in year.items %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.tags %}<em>({{ post.tags | join: ", " }})</em>{% endif %}
  </li>
{% endfor %}
</ul>
{% endfor %}
