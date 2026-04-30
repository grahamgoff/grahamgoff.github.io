---
title: "Aligning Estimands, Identification, and Conclusions"
collection: publications
category: working
permalink: /research/aligning-estimands/
listed: true
date: 2025-01-01
authors: "with [Mike Denly](https://mikedenly.com)"
venue: "Under review"
venue_url: "https://www.cambridge.org/core/journals/american-political-science-review"
venue_full: "American Political Science Review"
presentations: "TexMeth; [Causal Data Science Meeting](https://www.causalscience.org)"
image: /publications/aligning-estimands.png
---

Regressions with control variables underpin observational social science, but control variable selection can change the estimands and inferences that models support. In this paper, we introduce a workflow that combines Directed Acyclic Graphs (DAGs) with automated empirical estimation to recover target estimands. To illustrate its utility, we re-examine all 2024 American Political Science Review (APSR) articles using observational regressions with controls. Incorporating author feedback on our DAGs, we find no colliders. However, 61% of articles include estimand-shifting mediators or their descendants, and 21% of articles interpret them as total effects without qualification. Removing DAG-inconsistent variables also meaningfully alters standard errors, coefficient magnitudes, and statistical significance. Reweighting to recover target estimands not only yields similar patterns for coefficient magnitudes and statistical significance but also some positivity failures. Our results suggest that diagnosing assumptions before drawing conclusions with our R package, [DAGassist](https://cran.r-project.org/web/packages/DAGassist/index.html), can improve empirical practice.