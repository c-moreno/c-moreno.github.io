---
layout: page
title: Distinctions
permalink: /distinctions/
---

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