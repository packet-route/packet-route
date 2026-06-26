Student-created artifacts, archived by class year.

{% assign posts_by_class = site.posts | group_by: "class" %}
{% for year in posts_by_class %}
## Class {{ year.name }}

{% for post in year.items %}
<article style="margin-bottom: 1.5em;">
  <h3 style="margin-bottom: 0.2em;">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h3>
  <p style="color: #666; font-size: 0.9em; margin: 0;">
    {{ post.date | date: "%d/%m/%Y" }}
    {% if post.tags %} &middot; {{ post.tags | join: ", " }}{% endif %}
  </p>
  {% if post.author %}<p>{{ post.author }}</p>{% endif %}
</article>
{% endfor %}
{% endfor %}
