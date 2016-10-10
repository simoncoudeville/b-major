---
title: Line-up
permalink: "/en/line-up/"
section: line-up
layout: line-up
lang: en
---

{% for concert in site.en_concerts %}
  <h2>
    <a href="{{ site.baseurl }}{{ concert.url }}">
        {{ concert.title }}
    </a>
  </h2>
{% endfor %}
