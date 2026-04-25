---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

A list of pages on this site.

<h2>Pages</h2>
{% for post in site.pages %}
  {% if post.title %}<a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a><br/>{% endif %}
{% endfor %}

<h2>Publications</h2>
{% for post in site.publications %}
  <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a><br/>
{% endfor %}
