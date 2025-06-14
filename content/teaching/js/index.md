---
title: "Hybrid AI for Water Infrastructure: GNN + PINN + SCADA"
summary: Learn how to build adaptive models for water networks using Graph Neural Networks, Physics-Informed Neural Networks, and SCADA integration.
date: 2025-06-14
type: docs
math: true
tags:
  - GNN
  - PINN
  - SCADA
  - EPANET
  - GIS
image:
  caption: 'Example: Interactive GNN model of a water distribution system with SCADA inputs.'
---

This tutorial introduces a hybrid modeling approach combining:

- **Graph Neural Networks (GNN)** for spatial reasoning over EPANET-modeled water networks.
- **Physics-Informed Neural Networks (PINN)** to model hydraulic equations (e.g., Darcy–Weisbach) under constraints.
- **SCADA data streams** for real-time signal integration.
- Optional **GIS layers** to enhance spatial inference and visualization.

## Demo Video

{{< youtube D2vj0WcvH5c >}}

## Audio Sample (SCADA alert classification)

{{< audio src="ambient-piano.mp3" >}}

## Code Example

```python
import wntr
wn = wntr.network.WaterNetworkModel("Walkerton_v1.inp")
sim = wntr.sim.EpanetSimulator(wn)
results = sim.run_sim()
