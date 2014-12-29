---
layout: index
permalink: /fr/
excerpt: "Salutations ! Je suis doctorant en informatique. Ma thèse combine évaluation des interactions homme-machine et enregistrements électro-encéphalographiques. Plus souvent que ne le souhaiteraient mes directeurs, j'aime aussi jouer avec les capteurs physiologiques et avec le machine learning."
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
{% for post in site.projects_fr %}
  <!-- avoid to show an index page -->
  {% if post.exclude != true %}
    {% include post-grid.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->
