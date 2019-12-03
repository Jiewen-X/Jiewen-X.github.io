---
layout: default
title: Researches and Publications
---

# Researches & Publications

{% for post in site.posts %}

### <a href="{{ post.url }}">{{ post.title }}</a>

> <time datetime="{{ post.date | date_to_xmlschema }}">
>     {{ post.date | date: "%b %-d, %Y" }}
> </time>

{{ post.excerpt |  markdownify }}

{% endfor %}
