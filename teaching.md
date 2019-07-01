---
layout: page
title: Teaching Experience
permalink: /teaching/
---

<ul class="posts">
  {% for proj in site.data.teaching %}
    {% if proj.date %}
      <h4><li>{{ proj.workplace }} &raquo; <small>{{ proj.date }}</small></li></h4>
    {% else %}
      <h4><li>{{ proj.workplace }}</li></h4>
    {% endif %}
    <ul>
    {% for proj_spec in proj.projs %}
      {% if proj_spec.date %}
       <li><strong>{{ proj_spec.title}}</strong> &raquo; {{ proj_spec.date }}</li>
      {% else %}
        <li><strong>{{ proj_spec.title}}</strong></li>
      {% endif %}
      
      <p style="margin-left:10px">{{ proj_spec.description}} </p>
    {% endfor %}
    </ul>
  {% endfor %}
</ul>