---
layout: single
title: "Talks"
permalink: /talks/
author_profile: true
---

Below is a list of talks. Click each for details.

<ul>
{%- for talk in site.talks -%}
  <li><a href="{{ talk.url | relative_url }}">{{ talk.title }}</a> — {{ talk.date | date: "%b %-d, %Y" }}</li>
{%- endfor -%}
</ul>
