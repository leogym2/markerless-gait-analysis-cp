# Markerless Gait Analysis for Cerebral Palsy — HMR Benchmarking

Master's Thesis · ETH Zürich · SCAI Lab  
**ScAIt — Scalable AI for Gait**  
Leonardo Palestra

---

## Overview

This repository contains the evaluation pipeline developed for WP1.2 of the ScAIt project: benchmarking state-of-the-art **Human Mesh Recovery (HMR)** models on RGB gait data from patients with **Cerebral Palsy (CP)**.

Seven models are evaluated against SMPL-X ground truth captured at ETH's Volumetric Capture Lab:

| Model | Type |
|---|---|
| CameraHMR | Single-frame |
| TokenHMR | Single-frame |
| WHAM | Video-based |
| TRAM | Video-based |
| GENMO | Video-based |
| NLF-L | Single-frame |
| SAM 3D Body | Video-based |

---

## Metrics

- **PA-MPJPE** — Procrustes Aligned Mean Per Joint Position Error (mm)
- **PVE** — Per Vertex Error (mm)
- **PA-MPVPE** — Procrustes Aligned Mean Per Vertex Position Error (mm)

---

## Dataset

**AIT-CP-GAIT** — 15 CP subjects, ~150k frames, multi-camera RGB setup.  
> ⚠️ The dataset is not included in this repository (medical data, ETH agreements).

---

## Status

- [x] Evaluation pipeline — all 7 models
- [ ] Fine-tuning
- [ ] Deployment (FastAPI / ONNX)

---

## Affiliation

SCAI Lab · ETH Zürich · [Rehabilitation Engineering Laboratory](https://relab.ethz.ch/)
