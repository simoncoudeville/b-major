---
title: Programma
permalink: "/programma/"
section: line-up
layout: line-up
lang: nl
---

{% for concert in site.nl_concerts %}
  {% capture day %}{{ concert.concert_date | date: "%d" }}{% endcapture %}
  {% if day == "02" %}
  <h2>
    <a href="{{ site.baseurl }}{{ concert.url }}">
        {{ concert.title }}
    </a>
  </h2>
  <p>
    {{ concert.concert_date | date: '%B %d, %Y' }}
  </p>
  {% endif %}
  {% if day == "01" %}
  <h2>
    <a href="{{ site.baseurl }}{{ concert.url }}">
        {{ concert.title }}
    </a>
  </h2>
  <p>
    {{ concert.concert_date | date: '%B %d, %Y' }}
  </p>
  {% endif %}
{% endfor %}
