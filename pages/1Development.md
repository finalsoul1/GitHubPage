---
layout: page
title: Development
---
<br>

<div class="message">
- Linux<br>
  {% for post in site.posts %}
  {% if post.tag == "Linux" %}
  <a href="{{ post.url }}">{{ post.title }}</a><br>
  {% endif %}
  {% endfor %}
</div>

<div class="message">
- JavaScript<br>
  {% for post in site.posts %}
  {% if post.tag == "javascript" %}
  <a href="{{ post.url }}">{{ post.title }}</a><br>
  {% endif %}
  {% endfor %}
</div>

<div class="message">
- Mac<br>
  {% for post in site.posts %}
  {% if post.tag == "mac" %}
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
