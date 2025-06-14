---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-06-14
type: landing

design:
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      username: tetiana-starovoyt
      text: |
        I am a researcher in hybrid artificial intelligence, resilient water infrastructure, and spatial optimization.  
        My work focuses on **GNN + PINN integration**, **SCADA-driven anomaly detection**, and **critical infrastructure AI** for utilities.  
        I collaborate with academic and industry partners across Europe within the Horizon framework.

        Let's build intelligent, adaptive water systems together.
      button:
        text: Download CV
        url: uploads/tetiana-starovoyt-cv.pdf
    design:
      css_class: dark
      background:
        color: "#000000"
        image:
          filename: banner/water-infra-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: markdown
    content:
      title: "Research Themes"
      subtitle: ""
      text: |-
        - **Hybrid Neural Models**: GNN, PINN, fuzzy logic  
        - **Water Network Optimization**: pressure zones, valve placement, leakage detection  
        - **GeoAI & GIS Integration**: spatial data pipelines with EPANET/WNTR  
        - **SCADA-aware Simulation**: anomaly detection under blackout scenarios  
        - **Metaheuristics**: NSGA-II, ACO, CMA-ES for adaptive control strategies  
        
        I’m currently building decision-support systems for water utilities using AI and digital twin concepts.

  - block: collection
    id: featured-papers
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
    id: all-papers
    content:
      title: Recent Publications
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1

  - block: collection
    id: news
    content:
      title: News & Updates
      page_type: post
      count: 5
      filters:
        exclude_featured: false
        exclude_future: false
        exclude_past: false
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]

  - block: cta-card
    content:
      title: Interested in collaboration?
      text: |
        I'm open to international cooperation under Horizon Europe, bilateral projects, and smart city initiatives.  
        My pipeline integrates **SCADA data, EPANET models, GNNs, PINNs, GIS, and evolutionary optimization** for resilient water infrastructure.

        Let's build the next generation of digital utilities together.
      button:
        text: Get in Touch
        url: /contact/
    design:
      card:
        css_class: "bg-primary-700"
        css_style: ""
---

