---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
<link rel="icon" type="image/png" href="https://raw.githubusercontent.com/senanindya/senanindya.github.io/main/favicon.ico">
{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
 
<script src="https://bibbase.org/show?bib=https%3A%2F%2Fbibbase.org%2Fnetwork%2Ffiles%2FZQjAwoCiJazh4HZ3b&noBootstrap=1&jsonp=1"></script> 

