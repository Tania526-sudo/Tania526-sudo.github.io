---
# Leave the homepage title empty to use the site title
title: ""
type: landing
date: 2025-06-14


design:
  spacing: "6rem"

sections:
  - block: about
    content:
      title: "Tetiana Starovoyt"
      subtitle: "PhD Researcher in AI & Water Infrastructure"
      text: |
        I'm working on **hybrid GNN + PINN models**, digital twins, SCADA anomaly detection, and optimization of water infrastructure under uncertainty.
        Let's build the next generation of **smart utilities** together.
      image:
        filename: avatar.jpg
        alt_text: Tetiana Starovoyt
      actions:
        - label: "Download CV"
          url: uploads/tetiana-starovoyt-cv.pdf
          icon: file-pdf
          color: primary

  - block: markdown
    content:
      title: "Research Themes"
      text: |
        - **Hybrid Neural Models**: GNN, PINN, fuzzy logic  
        - **Water Network Optimization**: pressure zones, valve placement, leakage detection  
        - **GeoAI & GIS Integration**: spatial data pipelines with EPANET/WNTR  
        - **SCADA-aware Simulation**: anomaly detection under blackout scenarios  
        - **Metaheuristics**: NSGA-II, ACO, CMA-ES for adaptive control strategies

  - block: collection

    content:
      title: "Featured Publications"
      filters:
        folders: ["publication"]
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection

    content:
      title: "All Publications"
      filters:
        folders: ["publication"]
    design:
      view: citation

  - block: collection

    content:
      title: "Talks"
      filters:
        folders: ["event"]
    design:
      view: article
      columns: 1

  - block: collection

    content:
      title: "News & Updates"
      page_type: post
      count: 5

    design:
      view: date-title-summary
      

  - block: cta
    content:
      title: "Let's Collaborate"
      text: |
        Open for collaboration under Horizon Europe, bilateral projects, and innovation grants.  
        Let’s co-develop AI-powered digital twins for resilient urban systems.
      actions:
        - label: "Contact Me"
          url: /contact/
          color: success
---

