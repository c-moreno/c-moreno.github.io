---
layout: page
title:
permalink: /projects/
---
<h1 class="post-title">Research</h1>

<ul class="posts">
  {% for proj in site.data.research %}
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

<br />
<h1 class="post-title">Industry</h1>

<ul class="posts">
  {% for proj in site.data.industry %}
    {% if proj.date %}
      <h4><li>{{ proj.workplace }} &raquo; <small>{{ proj.date }}</small></li></h4>
    {% else %}
      <h4><li>{{ proj.workplace }}</li></h4>
    {% endif %}
    <ul>
    {% for proj_spec in proj.projs %}
      {% if proj_spec.title %}
        {% if proj_spec.date %}
         <li><strong>{{ proj_spec.title}}</strong> &raquo; {{ proj_spec.date }}</li>
        {% else %}
          <li><strong>{{ proj_spec.title}}</strong></li>
        {% endif %}
        <p style="margin-left:10px">{{ proj_spec.description}} </p>
      {% else %}
        <li><p style="margin-left:10px">{{ proj_spec.description}} </p></li>
      {% endif %}
    {% endfor %}
    </ul>
  {% endfor %}

<br />
</ul><h1 class="post-title">School</h1>

<ul class="posts">
  {% for proj_spec in site.data.school %}
      {% if proj_spec.date %}
       <li><strong>{{ proj_spec.title}}</strong> &raquo; {{ proj_spec.date }}</li>
      {% else %}
        <li><strong>{{ proj_spec.title}}</strong></li>
      {% endif %}

      <p style="margin-left:10px">{{ proj_spec.description}} </p>
  {% endfor %}
</ul>
