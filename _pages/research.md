---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% assign working = site.publications | where: "category", "working" | where_exp: "p", "p.listed != false" | sort: "date" | reverse %}

{% if working.size > 0 %}
## Working Papers

<div class="research-grid">
  {% for post in working %}
    {% include archive-single-research.html %}
  {% endfor %}
</div>
{% endif %}

## Prior Publications

- **[Kafala as Fatal Strategy: A Historical and Critical Analysis of the Qatari Kafala System](/files/kafala.pdf)** (with L.E. Chenault). *Consumption Markets & Culture*, 2025, 28(4): 286–298.
- **[Ascetic Protestantism as Fatal Strategy](/files/fatal-strategy.pdf).** *Consumption Markets & Culture*, 2024, 27(3): 284–294.
