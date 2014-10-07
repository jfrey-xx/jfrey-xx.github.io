---
layout: index
permalink: /
excerpt: "Greetings! I'm a PhD student in computer science. My thesis brings together the evaluation of human-computer interaction and electroencephalography recordings. More often than my advisers would like, I also toy with physiological sensors and machine learning."
---

### Last news

<div class="tiles">

{% for post in site.posts %}
  <!-- only show posts of current language, only brief versions -->
  {% if post.lang == page.lang %}
    {% include post-list-short.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->

<!-- get to next line no matter what -->
<!--  <br style="clear: both" /> -->

### Last projects

<div class="tiles">

<!-- not really a "post", but it's the variable name used in the html, and it works the same for this kind of page -->
{% for post in site.projects %}
  <!-- avoid to show an index page -->
  {% if post.exclude != true %}
    {% include post-grid.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->
