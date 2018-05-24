---
permalink: /fr/projets/
title: "Liste des projets"
exclude: true
layout: archive
lang: fr
---

<div class="tiles">

<!-- not really a "post", but it's the variable name used in the html, and it works the same for this kind of page -->
{% assign projects_fr = site.projects_fr | sort:"order"  %}
{% for post in projects_fr reversed %}
  <!-- avoid to show an index page -->
  {% if post.exclude != true %}
    {% include post-grid-simple.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->
