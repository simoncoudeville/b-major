---
title: Programma
permalink: "/programma/"
section: line-up
layout: line-up
title_en: line-up
permalink_en: "/line-up/"
---

{% assign concerts=site.concerts | where:"lang", site.lang %}
{% for concert in concerts %}
  <h2>
    <a href="{{ site.baseurl }}{{ concert.url }}">
        {{ concert.title }}
    </a>
  </h2>
{% endfor %}
