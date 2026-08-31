---
title: "Control Variables, Estimands, and Conclusions in Observational Regression Analyses"
collection: publications
category: working
permalink: /research/aligning-estimands/
listed: true
date: 2025-01-01
authors: "with [Mike Denly](https://mikedenly.com)"
venue: "Under review"
venue_url: "https://www.tandfonline.com/journals/uasa20"
venue_full: "Journal of the American Statistical Association"
presentations: "TexMeth; [Causal Data Science Meeting](https://www.causalscience.org)"
image: /publications/aligning-estimands.png
---

Regressions with observational data often depend on control variable selection decisions. Most researchers base these decisions on omitted variable bias concerns, but control variable selection can also change the estimands that regressions support. We advance a workflow for aligning regressions with target estimands and assessing when misalignment changes inferential conclusions. Four criteria underpin our assessments: covariate-role alignment, estimand recovery, sample support, and causal structure dependence. We demonstrate the workflow's utility by constructing Directed Acyclic Graphs (DAGs) and reanalyzing all possible articles using observational regressions with controls in the 2024 edition of the flagship American Political Science Review. Incorporating author feedback on the DAGs, we find that 64% of articles (18/28) exhibit estimand or interpretation misalignment. By the same token, only 29% (8/28) have inferentially vulnerable main conclusions under estimand recovery, sample support, or causal structure dependence. The results distinguish widespread estimand ambiguity from a smaller set of vulnerable conclusions affecting roughly three in ten articles. Our open-source R package, [DAGassist](https://cran.r-project.org/web/packages/DAGassist/index.html), implements the workflow with only two required inputs: a user-supplied DAG and regression call.