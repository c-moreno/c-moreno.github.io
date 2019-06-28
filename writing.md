---
layout: page
title: Writing Samples
permalink: /writing/
---
# Technical Writing
<ul class="posts">
  {% for post in site.data.technical_writings %}
    <li><strong><a href="{{ post.url }}">{{ post.title }}</a> </strong>&raquo; {{ post.date }}</li>
    <p style="margin-left:20px">{{ post.description}} </p>
  {% endfor %}
</ul>

# Creative Writing
<ul class="posts">
  {% for post in site.data.creative_writings %}
    <li><strong><a href="{{ post.url }}">{{ post.title }}</a> </strong>&raquo; {{ post.date }}</li>
    <p style="margin-left:20px">{{ post.description}} </p>
  {% endfor %}
</ul>
