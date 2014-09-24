---
layout: index
permalink: /
title: "Latest Posts"
excerpt: "I'm a PhD student in computer science and so on"
---

### Last news

<div class="tiles">

{% for post in site.posts %}
  <!-- only show posts of current language -->
  {% if post.lang == page.lang %}
    {% include post-grid.html %}
  {% endif %}
{% endfor %}
</div><!-- /.tiles -->

<!-- get to next line no matter what -->
<br style="clear: both" />

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
