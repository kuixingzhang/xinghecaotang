---
title: "詩稿"
permalink: /shigao/
layout: single
author_profile: false
---

{% assign poems = site.shigao | sort: "date" | reverse %}

{% for poem in poems %}

## [{{ poem.title }}]({{ poem.url | relative_url }})

{% if poem.image %}
[![{{ poem.title }}]({{ poem.image | relative_url }})]({{ poem.url | relative_url }})
{% endif %}

{% endfor %}
