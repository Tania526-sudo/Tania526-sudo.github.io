---
title: Research Project Planning & AI Experiments Management
summary: Manage your water AI research pipeline with mindmaps, Gantt charts, and scientific todo-lists.
date: 2025-06-14
authors:
  - Tetiana
tags:
  - Water AI
  - Hugo Blox
  - PINN
  - GNN
  - Project Management
image:
  caption: 'Image credit: [**Tetiana Starovoit**](https://github.com/Tania526-sudo)'
---

Effectively manage your **AI-driven research projects** for smart water networks — from ideation to simulation, paper writing, and presentations.

## Ideation (Mind Mapping)

Use Hugo Blox's **mindmap** extension to brainstorm ideas for a new hybrid AI model or grant proposal (e.g. Horizon Europe or Global Water Summit initiative):

```markmap {height="250px"}
- AquaTwin+ Project
  - Hybrid AI
    - GNN
    - PINN
    - Fuzzy Logic
  - SCADA Integration
  - Pollution Modelling
  - Leak Detection
  - DMA Zoning
  - Partners
    - TUHH
    - Hamburg Wasser
    - КПІ
    - Київводоканал
    - Siemens


gantt
dateFormat  YYYY-MM-DD
title Hybrid AI for Smart Water Networks

section Setup
Define Objectives    :done, 2025-05-01, 5d
Prepare Data         :done, 2025-05-06, 5d

section Development
GNN Modeling         :active, 2025-05-11, 10d
PINN Integration     :2025-05-21, 7d
Pollution Scenarios  :2025-05-28, 5d

section Dissemination
Prepare GitHub Repo  :2025-06-02, 2d
Global Summit Slides :2025-06-04, 2d


- [x] Import Walkerton EPANET model
- [x] Add base demand & chlorine decay config
- [x] Integrate PINN for unknown pipe zones
- [x] Train GNN on simulated leaks
- [ ] Implement RL agent for tariff control
- [ ] Deploy interactive dashboard (Streamlit/Leaflet)
- [ ] Prepare Horizon Europe proposal PDF

