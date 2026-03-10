---
title: ''
cms_exclude: true
type: landing

# Optional header image (relative to `static/media/` folder).
banner:
  caption: ''
  image: ''

design:
  spacing: '6rem'

sections:
  - block: collection
    content:
      title: Publications
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    content:
      title: Working Papers
      filters:
        folders:
          - working-papers
    design:
      view: citation
  - block: collection
    content:
      title: Works in Progress
      text: Ongoing research and drafts.
      filters:
        folders:
          - works-in-progress
    design:
      view: card
---