---
layout: index
permalink: /fr/
excerpt: "Salutations ! Je suis chercheur en informatique. J'explore comment l'informatique physiologique peut améliorer les interactions homme-machine et mener à de nouveaux canaux de communication entre les personnes. J'en suis arrivé à la conclusion que le but de cette technologie est de contribuer à notre bien-être et de faciliter les relations humaines. Dumoins c'est la voie sur laquelle je tente de m'aventurer, bidouillant en chemin."
lang: fr
---

### Dernières brèves

<div class="tiles" id="news">

{% for post in site.posts %}
  <!-- only show posts of current language, only brief versions -->
  {% if post.lang == page.lang %}
    {% include post-list-short.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->

<!-- get to next line no matter what -->
<!--  <br style="clear: both" /> -->

### Derniers projets

<div class="tiles">

<!-- not really a "post", but it's the variable name used in the html, and it works the same for this kind of page -->
{% assign projects_fr = site.projects_fr | sort:"order"  %}
{% for post in projects_fr reversed %}
  <!-- avoid to show an index page -->
  {% if post.exclude != true %}
    {% include post-grid.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->
