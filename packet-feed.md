---
layout: page
title: Packet Feed
permalink: /packet-feed/
---

Student-created artifacts, archived by class year.

{% assign posts_by_class = site.posts | group_by: "class" %}
<ul>
{% for year in posts_by_class %}
  <li><a href="{{ '/packet-feed/' | append: year.name | relative_url }}">Class {{ year.name }}</a></li>
{% endfor %}
</ul>
