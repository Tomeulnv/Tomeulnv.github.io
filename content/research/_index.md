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
        {{< simplecite pdf="https://www.nature.com/articles/s41562-026-02469-6.pdf" code="" bib="/research/early-career-best-practices/cite.bib" abstract="Social science and behavioural genetics has long rejected eugenic associations, yet a growing market promotes embryo selection for IQ while the research community response remains muted. We call for unified best practices, updated training and participatory ethics so the field accounts for its historical legacy and present-day impact." >}}
        <span class="pub-title">
          Early Career Researcher-Led Best Practices for Social Science and Behavioural Genetics
        </span>

        <span class="pub-authors">
        V. Straub, N. Harerimana, L. Alajääskö, T. López-Nieto-Veitch, S. Ordóñez, A. Bülbül, Q. Peng, R. De Sabbata, M. Talens
        </span>

        <span class="pub-venue">
          <span class="pub-journal"> Nature Human Behaviour </span><span class="pub-year"> (2026)</span><span class="pub-note"></span>
          <span class="pub-status"><a class="pub-doi" href="https://doi.org/10.1038/s41562-026-02469-6" target="_blank" rel="noopener noreferrer">(doi:10.1038/s41562-026-02469-6)</a></span>
        </span>

        {{< /simplecite >}}
    design:
      columns: '1'

  - block: markdown
    id: working-papers
    content:
      title: "Working papers"
      text: |-
        {{< simplecite label="JOB MARKET PAPER" pdf="/uploads/JMP_TomeuLNV.pdf" slides="/uploads/mte_JM.pdf" code="" bib=""
        abstract="Does higher education amplify or compensate for inequalities associated with genetic predisposition to education? Because individuals with different genetic predispositions also select differently into university, comparisons across genetic groups can conflate differences in the gains from university with differences in who self-selects into it. To separate these returns and selection components, we extend the marginal treatment effect (MTE) framework by aligning, via a mapping function, group-specific returns at a common level of unobserved resistance to attending university, even when the distribution of resistance differs across groups. We apply the framework to the post-war expansion of university access in the United Kingdom, combining UK Biobank data with a newly constructed geocoded dataset of higher-education institutions. We use the reduction in distance to the nearest university between birth and adolescence as an instrument for obtaining a university degree and measure genetic predisposition using the Educational Attainment Polygenic Index (EA PGI). We estimate that returns to a university degree are approximately 0.36 log points higher among individuals in the lowest EA PGI tertile than among those in the highest, although the cross-group contrast is imprecise. Our decomposition suggests that this gap is primarily driven by differences in returns at comparable levels of resistance, with little contribution from differential sorting into university. These findings highlight the potential for expanding access to university to compensate for earnings inequalities associated with genetic predisposition to education." >}}
        
        <span class="pub-title">
          Genetically Informed Estimation of Marginal Returns to Education
        </span>

        <span class="pub-authors">
        Tomeu López-Nieto-Veitch, Pietro Biroli, Elisabetta De Cao, Rodrigo Pinto
        </span>

        <span class="pub-venue">
          <span class="pub-journal"> </span>
        </span>

        {{< /simplecite >}}

        {{< simplecite pdf="/uploads/Degree_of_Attraction.pdf" slides="/uploads/AM_IGSS.pdf" code="" bib="" abstract="Expanding access to higher education may reshape assortative mating by changing who individuals meet and partner with. However, establishing whether education changes who matches with whom is difficult, because observed spouse characteristics may themselves change within a given match. To isolate changes in partner composition, we use polygenic indices (PGIs) of the eventual spouse for education and cognition. These measures predict economically consequential characteristics but are fixed at conception and therefore cannot themselves respond to the focal individual's education. We exploit the post-war expansion of the British university system, linking the UK Biobank to a geocoded history of university provision, to instrument college attainment with the reduction in distance to the nearest university between birth and adolescence. We find that, among individuals induced to obtain a degree by improved geographic access, college attainment leads them to match with spouses whose Educational Attainment PGI is 0.68 standard deviations higher, with similarly large differences in PGIs for cognitive performance and mathematics. It also substantially increases spouse college attainment and occupation-based wages. By contrast, we find little evidence of systematic changes in within-couple similarity. Our results provide causal evidence that obtaining a college degree changes whom individuals match with, as revealed by the genetic characteristics of their spouses. The resulting matches also differ substantially in education and wages." >}}
        <span class="pub-title">
          A Degree of Attraction: Access to College and Partner Choice
        </span>
        <span class="pub-authors">
          Tomeu López-Nieto-Veitch, <a class="author-link" href="https://nicolaumartinbassols.com/">Nicolau Martin-Bassols</a>
        </span>
        {{< /simplecite >}}

        {{< simplecite pdf="https://arxiv.org/abs/2601.04066" code="https://github.com/Tomeulnv/wncc_sims" bib="/working-papers/wncc/cite.bib" abstract="Nested case-control (NCC) studies are a widely adopted design in epidemiology to investigate exposure-disease relationships. This paper examines weighted analyses in NCC studies, focusing on two prominent weighting methods: Kaplan-Meier (KM) weights and Generalized Additive Model (GAM) weights. We consider three target estimands: log-hazard ratios, conditional survival, and associations between exposures. While KM- and GAM-weights are generally robust, we identify specific scenarios where they can lead to biased estimates. We demonstrate that KM-weights can lead to biased estimates when a proportion of the originating cohort is effectively ineligible for NCC selection, particularly with small case proportions or numerous matching factors. Instead, GAM-weights can yield biased results if interactions between matching factors influence disease risk and are not adequately incorporated into weight calculation. Using Directed Acyclic Graphs (DAGs), we develop a framework to systematically determine which variables should be included in weight calculations. We show that the optimal set of variables depends on the target estimand and the causal relationships between matching factors, exposures, and disease risk. We illustrate our findings with both synthetic and real data from the European Prospective Investigation into Cancer and nutrition (EPIC) study. Additionally, we extend the application of GAM-weights to ''untypical'' NCC studies, where only a subset of cases are included. Our work provides crucial insights for conducting accurate and robust weighted analyses in NCC studies." >}}

        <span class="pub-title">
          On the Estimation of Inclusion Probabilities for Weighted Analyses of Nested Case Control Studies
        </span>

        <span class="pub-authors">
          <a class="author-link" href="https://tomeulnv.github.io/">Tomeu López-Nieto-Veitch</a>,
          <a class="author-link" href="https://rosselladesabbata.github.io/">Rossella De Sabbata</a>,
          <a class="author-link" href="https://einsteinmed.edu/es/faculty/11813/ryung-s-kim">Ryung Kim</a>,
          Sven Ove Samuelsen,
          Nathalie C. Støer,
          <a class="author-link" href="https://sites.google.com/site/vivianviallon/">Vivian Viallon</a>
        </span>

        <span class="pub-venue">
          <span class="pub-journal">arXiv preprint</span>
          <span class="pub-status">[submitted, under revision]</span>
        </span>

        {{< /simplecite >}}
    design:
      columns: '1'
  - block: markdown
    id: works-in-progress
    content:
      title: "Works in progress"
      text: |-
        {{< simplecite pdf="" slides="" code="" bib="" abstract="University expansion transforms women's educational opportunities, with potentially lasting consequences for family formation. Whether these consequences extend beyond delayed motherhood, and how they vary with genetic propensity for education, remains uncertain. To address these questions, we combine UK Biobank data with a newly constructed geocoded history of British higher-education institutions and instrument college attainment with reductions in distance to the nearest university during childhood. Among women whose attainment responds to improved access, college increases childlessness by around 24 percentage points and reduces completed fertility by an estimated 0.64 children, although the latter estimate is less precise. First births shift from the twenties into the thirties, alongside a lower probability of eventual motherhood. The Educational Attainment Polygenic Index (EA PGI) strongly predicts college attainment and is associated with later motherhood, but does not detectably predict heterogeneity in the fertility effects of college. The interaction estimates nevertheless remain imprecise, so substantial genetic moderation cannot be ruled out. Socioeconomic subgroup estimates suggest greater increases in later first births among women from disadvantaged birth districts, whereas women from advantaged districts experience more persistent reductions in entry into motherhood. We find no statistically detectable effects on men's completed fertility or childlessness. Overall, expanding access to higher education can have persistent demographic consequences, with suggestive evidence that these differ across birth-district socioeconomic conditions." >}}
        <span class="pub-title">
          College Education, Fertility and Genetics: Evidence from the Expansion of British Universities
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
