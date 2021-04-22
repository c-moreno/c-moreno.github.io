---
layout: page
title:
permalink: /writing/
---
<h1 class="post-title">Technical Writing</h1>

<ul class="posts">
  {% for post in site.data.creative_writings %}
    <li><strong><a href="{{ post.url }}">{{ post.title }}</a> </strong>&raquo; {{ post.date }}</li>
    <p style="margin-left:20px">{{ post.description}} </p>
  {% endfor %}
</ul>

<br />
<h1 class="post-title">Creative Writing</h1>

<ul class="posts">
  {% for post in site.data.technical_writings %}
    <li><strong><a href="{{ post.url }}">{{ post.title }}</a> </strong>&raquo; {{ post.date }}</li>
    <p style="margin-left:20px">{{ post.description}} </p>
  {% endfor %}
</ul>
