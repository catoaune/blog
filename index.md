---
layout: page
title: jeqo's blog
tagline: posts
---
{% include JB/setup %}
<div class="row-fluid">
  <div class="span9">
    <ul>
      {% for post in site.posts %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
          <p>{{ post.excerpt }}</p>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>
