---
title: "Research 2"
type: landing

design:
  spacing: '6rem'
  # you can customise other design options here
sections:
  - block: markdown
    content:
      title: "Publications"
      text: |-
        Here are some of my publications listed manually, but still using the
        citation shortcode so visitors can export references and view PDF/code links.
    design:
      columns: '1'

  - block: markdown
    content:
      title: "Working papers"
      text: |-
        {{< simplecite pdf="https://arxiv.org/abs/2601.04066" code="https://github.com/Tomeulnv/wncc_sims" bib="/working-papers/wncc/cite.bib" >}}

        <span class="pub-title">
          "On the estimation of inclusion probabilities for weighted analyses of nested case control studies"
        </span>

        <span class="pub-authors">
          <a class="author-link" href="https://tomeulnv.github.io/">T. López-Nieto Veitch</a>,
          <a class="author-link" href="https://example.com/desabbata">R. De Sabbata</a>,
          <a class="author-link" href="https://example.com/kim">R. Kim</a>,
          S. O. Samuelsen, N. C. Støer, V. Viallon (2026).
        </span>

        <span class="pub-venue">
          <span class="pub-journal">arXiv preprint</span>
          <span class="pub-status">[submitted, under revision]</span>.
        </span>

        {{< /simplecite >}}

        {{< simplecite pdf="" code="" bib="" >}}
        V. J. Straub, N. V. Harerimana, L. I. A. Alajääskö, T. López-Nieto Veitch, S. Ordóñez Beltrán, A. Bülbül, Q. Peng, R. De Sabbata, M. Talens (2026). *Early career researcher-led best practices for social science and behavioural genetics*. <strong>Nature Human Behaviour</strong> (comment) [invited minor revision].
        {{< /simplecite >}}
    design:
      columns: '1'
  - block: markdown
    content:
      title: "Works in progress"
      text: |-
        {{< simplecite pdf="" code="" bib="" >}}
        T. López-Nieto Veitch, N. Martin-Bassols (2026). *The Impact of Educational Reforms on Assortative Mating*. Draft exploring how changes in education policy affect partner sorting.
        {{< /simplecite >}}
    design:
      columns: '1'

  - block: markdown
    content:
      title: "Other Work"
      text: |-
        Here you can add additional items manually, notes, or descriptions.

        - A draft on something else (title and details manually typed.)

        <!--
          Feel free to add more entries below.
        -->
    design:
      columns: '1'
---

