---
layout: page
title: jeqo's blog
tagline: posts
---
{% include JB/setup %}

<ul>
  {% for post in site.posts %}
    <li>
    <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
