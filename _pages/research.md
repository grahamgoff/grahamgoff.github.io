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

## Software

<div class="software-list">
  <div class="software-card">
    <div class="software-card__logo">
      <a href="https://grahamgoff.github.io/DAGassist/">
        <img src="/software/DAGassist.png" alt="DAGassist hex logo">
      </a>
    </div>
    <div class="software-card__body">
      <p class="software-card__title">
        <a href="https://grahamgoff.github.io/DAGassist/">DAGassist</a>: Test Robustness with Directed Acyclic Graphs
      </p>
      <p class="software-card__authors">(with <a href="https://mikedenly.com/">Mike Denly</a>)</p>
      <p class="software-card__desc">Classifies variables by causal roles, recovers a target estimand, and generates a report comparing the original model with DAG-derived adjustment sets.</p>
      <p class="software-card__links">
        <a href="https://cran.r-project.org/package=DAGassist">CRAN</a> &middot;
        <a href="https://grahamgoff.github.io/DAGassist/">Website</a> &middot;
        <a href="https://github.com/grahamgoff/DAGassist/">GitHub</a>
      </p>
    </div>
  </div>
</div>


## Prior Academic Publications

- **[Kafala as Fatal Strategy: A Historical and Critical Analysis of the Qatari Kafala System](/files/kafala.pdf)** (with L.E. Chenault). *Consumption Markets & Culture*, 2025, 28(4): 286–298.
- **[Ascetic Protestantism as Fatal Strategy](/files/fatal-strategy.pdf).** *Consumption Markets & Culture*, 2024, 27(3): 284–294.
