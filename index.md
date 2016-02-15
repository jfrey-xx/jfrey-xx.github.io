---
layout: index
permalink: /
excerpt: "Greetings! I'm a researcher in computer science. I explore how physiological computing can contribute to human-computer interaction and foster new communication channels among the general public. I came to think that the purpose of those technological artifacts is to enhance well being and facilitate human relationships on the whole. Or at least this is the path into which I try to venture, hacking my way."
---

### Last news

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

### Last projects

<div class="tiles">

<!-- not really a "post", but it's the variable name used in the html, and it works the same for this kind of page -->
{% assign projects = site.projects | sort:"order"  %}
{% for post in projects reversed %}
  <!-- avoid to show an index page -->
  {% if post.exclude != true %}
    {% include post-grid-simple.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->
