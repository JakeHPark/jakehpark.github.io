---
layout: default
title: Essays
permalink: /essays/
---

# Essays

{% assign essays = site.essays | sort: "date" | reverse %}
{% for essay in essays %}

- [{{ essay.title }}]({{ essay.url }}){% if essay.date %} — {{ essay.date | date: "%Y-%m-%d" }}{% endif %}
  {% endfor %}
