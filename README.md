# Crop Yield & Health Monitoring System

> UAV RGB-based Crop Health & Yield Monitoring System using spectral vegetation indices (ExG, VARI, GLI, RGB-NDVI) and OpenCV.

[Repository](https://github.com/SanyogSingh07/crop-yield-monitoring-)

---

## Overview

**Crop Yield & Health Monitoring System** is a computer vision and precision agriculture application designed to analyze aerial UAV (drone) RGB imagery to assess crop health, canopy coverage, and estimated yield potential.

---

## Methodology & Vegetation Indices

Standard consumer UAVs capture RGB visible imagery without specialized multispectral sensors. This system computes specialized visible-band vegetation indices:

1. **Excess Green Index (ExG)**: Highlights green vegetation contrast against soil background:
   $$\text{ExG} = 2g - r - b$$
2. **Visible Atmospherically Resistant Index (VARI)**: Minimizes atmospheric effects for canopy fraction estimation:
   $$\text{VARI} = \frac{g - r}{g + r - b}$$
3. **Green Leaf Index (GLI)**: Measures foliage chlorophyll density:
   $$\text{GLI} = \frac{2g - r - b}{2g + r + b}$$
4. **RGB-NDVI Proxy**: Approximates vegetation vigor from visible channels.

---

## Installation & Usage

```bash
git clone https://github.com/SanyogSingh07/crop-yield-monitoring-.git
cd crop-yield-monitoring-
pip install -r requirements.txt

# Launch Local Streamlit Dashboard
streamlit run app.py
```
