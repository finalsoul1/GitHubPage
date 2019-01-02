---
layout: page
title: Development
---

<div class="message">
- Linux<br>
  {% for post in site.posts %}
  {% if post.tag == "Linux" %}
  <a href="{{ post.url }}">{{ post.title }}</a><br>
  {% endif %}
  {% endfor %}
</div>

<div class="message">
- Etc<br>
  {% for post in site.posts %}
  {% if post.tag == "etc" %}
  <a href="{{ post.url }}">{{ post.title }}</a><br>
  {% endif %}
  {% endfor %}
</div>