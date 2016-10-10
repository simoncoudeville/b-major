---
title: Programma
permalink: "/programma/"
section: line-up
layout: line-up
lang: nl
---

{% for concert in site.nl_concerts %}
  <h2>
    <a href="{{ site.baseurl }}{{ concert.url }}">
        {{ concert.title }}
    </a>
  </h2>
{% endfor %}
