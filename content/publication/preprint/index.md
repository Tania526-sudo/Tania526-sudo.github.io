---
title: "Preprint: Fuzzy-GNN and PINN-based Modeling of Water Infrastructure under SCADA Blackout Conditions"

authors:
- tetiana-starovoyt

date: "2025-06-10T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2025-06-14T00:00:00Z"

publication_types: ["article"]

publication: ""
publication_short: ""

abstract: >
  This working paper introduces an integrated hybrid modeling pipeline combining fuzzy graph neural networks (F-GNN), physics-informed neural networks (PINNs), and multi-objective optimization for adaptive water network control. The model addresses uncertainties due to partial SCADA blackout and proposes mechanisms for inferring missing hydraulic data. The framework was evaluated using a modified Walkerton EPANET model and synthetic fault scenarios. The results highlight the effectiveness of integrating PINNs with fuzzy logic to maintain system observability and resilience during data loss.

summary: >
  A preprint presenting an adaptive hybrid GNN+PINN+fuzzy model for resilient water infrastructure under SCADA data loss.

tags:
- Fuzzy GNN
- PINN
- SCADA
- Hybrid AI
- Critical Infrastructure
- Water Networks
- Optimization
- Preprint

featured: true

links:
- name: GitHub (public components)
  url: 

url_pdf: ""
url_code: ""
url_dataset: "#"
url_poster: ""
url_project: "hybrid-fuzzy-gnn-water"
url_slides: ""
url_source: ""
url_video: ""

image:
  caption: 'Graph-based fuzzy PINN structure for adaptive modeling of blackout zones in water distribution'
  focal_point: "center"
  preview_only: false

projects:
- hybrid-fuzzy-gnn-water

slides: ""

---

This preprint builds upon the results of our previous published work on GIS-ANFIS-based accident prediction in water networks.

{{% callout warning %}}
Due to the critical nature of infrastructure data and the wartime conditions in Ukraine, **full access to source code and datasets is restricted**. Only general architecture and anonymized examples are shared publicly.
{{% /callout %}}

The proposed model includes:

- Fuzzy membership layers on top of graph node attributes
- Integration of PINN for physical constraint modeling (e.g., Darcy–Weisbach)
- Compensation mechanisms for missing SCADA sensor inputs
- NSGA-II multi-objective optimization for valve control

This approach is applicable in utility AI systems that must remain resilient even during cyber-physical or war-induced infrastructure disruptions.
