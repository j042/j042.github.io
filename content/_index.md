---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      #button:
      #  text: Download CV
      #  url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: collection
    content:
      title: Publications
      text: ""
      filters:
        folders:
          - publication
    design:
      view: citation
  - block: collection
    content:
      title: Talks
      text: ""
      filters:
        folders:
          - talks
    design:
      view: citation
  - block: collection
    content:
      title: Projects
      count: 0
      filters:
        folders:
          - project
    design:
      view: article-grid
      fill_image: false
      columns: 3
  - block: collection
    content:
      title: Advised Theses
      text: ""
      filters:
        folders:
          - advised_theses
    design:
      view: citation
---
