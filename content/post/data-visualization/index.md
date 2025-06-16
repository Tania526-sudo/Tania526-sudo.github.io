---
title: Visualizing Smart Water Systems with AI & GIS
summary: How I combine Plotly, Mermaid, and structured data to explain GNN-PINN models and SCADA behavior in water distribution.
date: 2025-04-30
authors:
  - admin
tags:
  - AI for Water
  - GNN
  - SCADA
  - Plotly
  - GIS
  - HugoBlox
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/8b1cWDyvT7Y)'
---

In my recent work on **hybrid AI models for water infrastructure**, I needed ways to effectively explain system behavior, learning outcomes, and detected anomalies. Here are tools I used with **HugoBlox** to communicate those insights interactively and clearly.

## Interactive Charts with Plotly

I used [Plotly](https://plot.ly/) for dynamic visualizations of:

- Predicted vs actual pressure across nodes
- Leak probability heatmaps over time
- Consumption anomalies from SCADA time series

Save a Plotly `.json` file (e.g., `leak-probability.json`) in your page folder and display it like this:

```go
{{< chart data="leak-probability" >}}


graph TD
A[SCADA Data] --> B(GNN Inference)
B --> C{Leak Detected?}
C -->|Yes| D[Trigger Alert]
C -->|No| E[Continue Monitoring]


sequenceDiagram
SCADA->>GNN: Feed pressure data
GNN->>PINN: Pass edge/node outputs
PINN-->>SCADA: Simulated parameters
Note right of PINN: Feedback to SCADA control

