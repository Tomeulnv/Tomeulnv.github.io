---
title: "On the estimation of inclusion probabilities for weighted analyses of nested case control studies"
authors:
  - me
  - rossella-de-sabbata
  - ryung-kim
  - sven-ove-samuelsen
  - nathalie-c-stoer
  - vivian-vallon
date: 2026-01-07T00:00:00Z      # actual write date
publishDate: 2026-01-07T00:00:00Z
publication_types:
  - preprint            # the `preprint` type is what makes it a “working paper”
publication: "arXiv preprint arXiv:2601.04066"
publication_short: "**arXiv preprint** [submitted, under revision]"
abstract: >
  Nested case-control (NCC) studies are a widely adopted design in epidemiology to investigate exposure–disease relationships. This paper examines weighted analyses in NCC studies, focusing on two prominent weighting methods: Kaplan–Meier (KM) weights and Generalized Additive Model (GAM) weights. We consider three target estimands: log-hazard ratios, conditional survival, and associations between exposures. While KM- and GAM-weights are generally robust, we identify specific scenarios where they can lead to biased estimates. We demonstrate that KM-weights can lead to biased estimates when a proportion of the originating cohort is effectively ineligible for NCC selection, particularly with small case proportions or numerous matching factors. Instead, GAM-weights can yield biased results if interactions between matching factors influence disease risk and are not adequately incorporated into weight calculation. Using Directed Acyclic Graphs (DAGs), we develop a framework to systematically determine which variables should be included in weight calculations. We show that the optimal set of variables depends on the target estimand and the causal relationships between matching factors, exposures, and disease risk. We illustrate our findings with both synthetic and real data from the European Prospective Investigation into Cancer and nutrition (EPIC) study. Additionally, we extend the application of GAM-weights to "untypical" NCC studies, where only a subset of cases are included. Our work provides crucial insights for conducting accurate and robust weighted analyses in NCC studies.
tags:
  - epidemiology
  - nested-case-control
  - inverse probability weights
links:
  - type: pdf
    url: "https://arxiv.org/abs/2601.04066"
  - type: code
    url: "https://github.com/Tomeulnv/wncc_sims"
draft: false            # set true while still editing
---