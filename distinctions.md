---
layout: page
title:
permalink: /distinctions/
---

<h1 class="post-title">Awards</h1>

<ul class="posts">
  {% for aw in site.data.awards %}
    {% if aw.date %}
      <h4><li>{{ aw.title }} &raquo; <small>{{ aw.date }}</small></li></h4>
    {% else %}
      <h4><li>{{ aw.title }}</li></h4>
    {% endif %}
    {% if aw.description %}
      <p style="margin-left:20px">{{ aw.description}} </p>
    {% endif %}
  {% endfor %}
</ul>

<br />
<h1 class="post-title">Conferences</h1>

<ul class="posts">
  {% for conf in site.data.conferences %}
    {% if conf.date %}
      <h4><li>{{ conf.title }} &raquo; <small>{{ conf.date }}</small></li></h4>
    {% else %}
      <h4><li>{{ conf.title }}</li></h4>
    {% endif %}
    {% if conf.description %}
      <p style="margin-left:20px">{{ conf.description}} </p>
    {% endif %}

  {% endfor %}
</ul>
