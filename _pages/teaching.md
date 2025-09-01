---
layout: single
title: "Teaching"
permalink: /teaching/
author_profile: true
---

Courses I've taught or assisted:

<ul>
{%- for course in site.teaching -%}
  <li><a href="{{ course.url | relative_url }}">{{ course.title }}</a> — {{ course.term }}</li>
{%- endfor -%}
</ul>
