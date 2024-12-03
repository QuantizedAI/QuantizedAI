---
layout: default
title: "Blog"
---

# Blog
Welcome to our blog. Stay updated with the latest trends in deep learning quantization.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>

