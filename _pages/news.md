---
layout: single
title: "News"
permalink: /news/
author_profile: true
---

Updates and announcements.

<ul>
{%- for item in site.news -%}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a> — {{ item.date | date: "%b %-d, %Y" }}</li>
{%- endfor -%}
</ul>
