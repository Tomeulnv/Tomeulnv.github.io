---
title: "Research"
type: landing

design:
  spacing: '1rem'
  # you can customise other design options here
sections:
  - block: markdown
    id: publications
    content:
      title: "Publications"
      text: |-
        Nothing here yet, hopefully something will come up soon :)
    design:
      columns: '1'

  - block: markdown
    id: working-papers
    content:
      title: "Working papers"
      text: |-
        {{< simplecite pdf="" code="" bib="" 
        abstract="Returns to education have long been a central focus of social science research due to their implications for productivity, social mobility, and inequality. A persistent challenge in this literature is the inability to fully account for heterogeneity in skills and initial endowments, which may confound estimates of causal returns. This paper addresses this limitation by incorporating genetic information—specifically, the Educational Attainment Polygenic Index (EA PGI)—to study the role of genetic predisposition in shaping the returns to education. We develop a novel extension of the Marginal Treatment Effects (MTE) framework that introduces a categorical moderator, building on a monotone ''warp'' mapping that aligns group-specific resistance ranks to a common pooled scale. This allows for valid comparisons of marginal returns across genetic groups with different selection patterns. Exploiting the mid-20th-century expansion of university access in the United Kingdom, we compute the reduction in distance to university as an instrument for college and find a significant negative gene-environment interaction. Causal returns to college are substantially higher for individuals with low genetic predisposition to education compared to those with high predisposition. Using a Shapley-based decomposition, we show that this gap is driven almost entirely by heterogeneity in returns (GxE) rather than by differences in sorting into college (rGE). These findings suggest that higher education acts as an equalizer, playing a compensatory role that mitigates genetic inequality." >}}
        
        <span class="pub-title">
          Genetically Informed Estimation of Marginal Returns to Education
        </span>

        <span class="pub-authors">
        P. Biroli, E. De Cao, R. Pinto
        </span>

        <span class="pub-venue">
          <span class="pub-journal"> </span>
          <span class="pub-status">[Draft available upon request]</span>
        </span>

        {{< /simplecite >}}

        {{< simplecite pdf="https://arxiv.org/abs/2601.04066" code="https://github.com/Tomeulnv/wncc_sims" bib="/working-papers/wncc/cite.bib" abstract="Nested case-control (NCC) studies are a widely adopted design in epidemiology to investigate exposure-disease relationships. This paper examines weighted analyses in NCC studies, focusing on two prominent weighting methods: Kaplan-Meier (KM) weights and Generalized Additive Model (GAM) weights. We consider three target estimands: log-hazard ratios, conditional survival, and associations between exposures. While KM- and GAM-weights are generally robust, we identify specific scenarios where they can lead to biased estimates. We demonstrate that KM-weights can lead to biased estimates when a proportion of the originating cohort is effectively ineligible for NCC selection, particularly with small case proportions or numerous matching factors. Instead, GAM-weights can yield biased results if interactions between matching factors influence disease risk and are not adequately incorporated into weight calculation. Using Directed Acyclic Graphs (DAGs), we develop a framework to systematically determine which variables should be included in weight calculations. We show that the optimal set of variables depends on the target estimand and the causal relationships between matching factors, exposures, and disease risk. We illustrate our findings with both synthetic and real data from the European Prospective Investigation into Cancer and nutrition (EPIC) study. Additionally, we extend the application of GAM-weights to ''untypical'' NCC studies, where only a subset of cases are included. Our work provides crucial insights for conducting accurate and robust weighted analyses in NCC studies." >}}

        <span class="pub-title">
          On the Estimation of Inclusion Probabilities for Weighted Analyses of Nested Case Control Studies
        </span>

        <span class="pub-authors">
          <a class="author-link" href="https://tomeulnv.github.io/">T. López-Nieto Veitch</a>,
          <a class="author-link" href="https://rosselladesabbata.github.io/">R. De Sabbata</a>,
          <a class="author-link" href="https://example.com/kim">R. Kim</a>,
          S. O. Samuelsen,
          N. C. Støer,
          <a class="author-link"href="https://sites.google.com/site/vivianviallon/"> V. Viallon</a>
        </span>

        <span class="pub-venue">
          <span class="pub-journal">arXiv preprint</span>
          <span class="pub-status">[submitted, under revision]</span>
        </span>

        {{< /simplecite >}}


        {{< simplecite pdf="" code="" bib="" >}}
        <span class="pub-title">
          Early Career Researcher-Led Best Practices for Social Science and Behavioural Genetics
        </span>

        <span class="pub-authors">
        V. Straub, N. Harerimana, L. Alajääskö, T. López-Nieto-Veitch, S. Ordóñez, A. Bülbül, Q. Peng, R. De Sabbata, M. Talens
        </span>

        <span class="pub-venue">
          <span class="pub-journal"> Nature Human Behaviour </span><span class="pub-note">(comment)</span>
          <span class="pub-status"> [invited minor revision] </span>
        </span>

        {{< /simplecite >}}
    design:
      columns: '1'
  - block: markdown
    id: works-in-progress
    content:
      title: "Works in progress"
      text: |-
        {{< simplecite pdf="" slides="" code="" bib="" >}}
        <span class="pub-title">
          The Impact of Educational Reforms on Assortative Mating
        </span>
        <span class="pub-authors">
          with <a class="author-link" href="https://nicolaumartinbassols.com/">Nicolau Martin-Bassols</a>
        </span>
        {{< /simplecite >}}

        {{< simplecite pdf="" slides="" code="" bib="" >}}
        <span class="pub-title">
          UK University Expansion and Fertility
        </span>
        <span class="pub-authors">
          with <a class="author-link" href="https://elisabettadecao.com//">Nicola Barban, Elisabetta De Cao and Marco Francesconi </a>
        </span>
        {{< /simplecite >}}
    design:
      columns: '1'

  # - block: markdown
  #   content:
  #     title: "Other Work"
  #     text: |-
  #       Here you can add additional items manually, notes, or descriptions.

  #       - A draft on something else (title and details manually typed.)

  #       <!--
  #         Feel free to add more entries below.
  #       -->
  #   design:
  #     columns: '1'
---

