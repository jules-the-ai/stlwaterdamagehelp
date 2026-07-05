---
title: St. Louis Water Damage Blog
h1: Water Damage Restoration Blog
kicker: Blog
description: Practical articles about flooded basements, water extraction, sewage backups, mold prevention, storm leaks, and restoration decisions in St. Louis.
---
<div class="blog-list">
{% for post in site.posts %}
  <article class="card post-card">
    <p class="eyebrow"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time></p>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.description }}</p>
    <a class="text-link" href="{{ post.url | relative_url }}">Read more</a>
  </article>
{% endfor %}
</div>
