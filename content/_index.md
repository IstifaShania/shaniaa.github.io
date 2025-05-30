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
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I explore the intersection of data science, AI, and real-world impact—with a strong focus on predictive modeling, machine learning, and decision intelligence for industry transformation.
        With a background in Electronics & Instrumentation and a Master's in Data Science & AI, my work often involves uncovering patterns in complex systems, optimizing processes, and developing scalable AI solutions—especially in the domains of energy, manufacturing, and digital transformation.

        My research combines quantitative modeling, AI system design, and behavioral insights to drive innovation, especially where sustainability and efficiency meet.

        ✨ I'm always open to collaboration, especially on projects that align with SDGs, intelligent automation, or human-centered AI.
    design:
      columns: '1'

  - block: collection
    id: papers
    draft: true  # Hidden but preserved for future use
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: recent-publications
    draft: true  # Hidden but preserved for future use
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      page_type: post
      count: 5
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      offset: 0
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]
---