---
layout: page
title: Musings
permalink: /musings/
---

# Musings

_Essays on narrative, consciousness, and artificial minds — ordered by recency._

{% assign sorted_musings = site.musings | sort: 'date' | reverse %}
{% for post in sorted_musings %}
<article class="post-item">
  <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
  <a class="post-title" href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
</article>
{% endfor %}
