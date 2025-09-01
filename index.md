---
layout: single
title: "Welcome"
permalink: /
author_profile: true
---

Hi! I'm **Your Name**, a researcher at ... This is my academic homepage.

## News
<ul>
{%- for item in site.news limit:5 -%}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a> — {{ item.date | date: "%b %-d, %Y" }}</li>
{%- endfor -%}
</ul>

## Selected Publications
<p>Here are a few selected papers from my full <a href="{{ '/publications/' | relative_url }}">publications list</a>.</p>
<ol>
{%- assign selected = site.scholar.bibliography | default: site.data.bibliography -%}
{%- bibliography --query @*[keyword=selected] --max 5 -%}
</ol>
