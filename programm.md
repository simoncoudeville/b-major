---
section: line-up
layout: line-up
title: Programma
title_en: line-up
permalink: "/programma/"
permalink_en: "/line-up/"
---

{% for concert in site.concerts %}
  <h2>{% if site.lang == "en" and concert.title_en != blank %}{{ concert.title_en }}{% else %}{{ concert.title }}{% endif %}</h2>
{% endfor %}
