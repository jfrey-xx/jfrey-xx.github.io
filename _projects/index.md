---
permalink: /projects/
title: "List of projects"
exclude: true
layout: archive
---

<div class="tiles">

<!-- not really a "post", but it's the variable name used in the html, and it works the same for this kind of page -->
{% assign projects = site.projects | sort:"order"  %}
{% for post in projects reversed %}
  <!-- avoid to show an index page -->
  {% if post.exclude != true %}
    {% include post-grid.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->
