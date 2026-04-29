---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% assign working = site.publications | where: "category", "working" | where_exp: "p", "p.listed != false" | sort: "date" | reverse %}
{% assign prior = site.publications | where: "category", "prior" | where_exp: "p", "p.listed != false" | sort: "date" | reverse %}

{% if working.size > 0 %}
## Working Papers

<div class="research-list">
  {% for post in working %}
    {% include archive-single-research.html %}
  {% endfor %}
</div>
{% endif %}

{% if prior.size > 0 %}
## Prior Publications

<div class="research-list research-list--text-only">
  {% for post in prior %}
    {% include archive-single-research.html text_only=true %}
  {% endfor %}
</div>
{% endif %}
