# 🌊 Potential Environmental Drivers of Algal Blooms & LANDSAT Characterization of the James River

**Dennie Truong · Colby College '24 · SARP East Undergraduate Research**

[![Research](https://img.shields.io/badge/Project-Environmental%20Research-2f6f8f)](https://github.com/)
[![Remote Sensing](https://img.shields.io/badge/Focus-LANDSAT%208-4c956c)](https://www.usgs.gov/landsat-missions/landsat-8)
[![Study Period](https://img.shields.io/badge/Data-2013--2022-6c757d)](https://www.usgs.gov/landsat-missions/landsat-8)

> **Investigating the environmental factors associated with phytoplankton blooms in the James River and evaluating the utility of LANDSAT 8 data for characterizing algal blooms.**

---

## 📌 Project Overview

Algal blooms can have significant ecological and public-health consequences, including dissolved oxygen depletion, fish kills, toxin production, wildlife mortality, and challenges for water treatment facilities.

This project investigates the environmental factors associated with phytoplankton growth in the **James River** and explores whether satellite-based observations from **LANDSAT 8** can be used to characterize algal blooms across the river.

The analysis combines long-term **in-situ water-quality observations** with statistical modeling and remotely sensed spectral data.

---
## 🔬 Research Questions

* What environmental factors are driving algal blooms?
* How effectively can LANDSAT 8 characterize algal blooms?

## 🗺️ Data

Analyzed water-quality and phytoplankton data from **5 sampling stations** along the James River from **2013–2022**.

**Variables:**

* Chlorophyll-a (Chl-a)
* Ammonium (NH₄⁺)
* Phosphate (PO₄³⁻)
* Turbidity
* Water temperature

## 📊 Methods

### Generalized Additive Model (GAM)

Used GAM to evaluate relationships between chlorophyll-a and environmental variables over time.

**Model performance:**

| Metric             |    Result |
| ------------------ | --------: |
| Explained Deviance | **71.7%** |
| R²                 | **0.709** |
| RMSE               |  **7.83** |
| MAE                |  **5.43** |

## 🛰️ LANDSAT 8

Used LANDSAT 8 spectral data to estimate and spatially characterize chlorophyll-a across the James River.

**Bands used:**
`Coastal Aerosol` · `Blue` · `Green` · `Red` · `Near Infrared`

A **PCA-based chlorophyll model** was used to generate spatial predictions for:

* July 27, 2019 — Pre-pandemic
* July 13, 2020 — During pandemic
* August 4, 2022 — Post-pandemic

## 📈 Key Findings

* **Ammonium and phosphate** availability were important factors associated with phytoplankton growth.
* The James River appeared to be primarily **nitrogen limited or nitrogen/phosphorus co-limited**.
* Increasing **water temperature** was associated with increasing chlorophyll-a.
* Increasing **turbidity** was associated with decreasing chlorophyll-a.
* The **head of the James River** experienced higher average phytoplankton bloom volumes than the mouth.
* Algal-bloom trends did not appear to be substantially affected during **2020**.
* LANDSAT 8 provided a way to extend chlorophyll-a observations spatially beyond individual sampling stations.

## 🌎 Applications

The project demonstrates how **environmental monitoring, statistical modeling, and satellite remote sensing** can be combined to study algal blooms and support broader harmful algal bloom monitoring efforts.

## 📁 Repository

```text
├── Code/                        # Analysis scripts
├── Data/                        # Project datasets
├── References/                  # Project references/sources
├── SARPEast2023_DTruong.pdf     # Research poster
└── README.md
```

## 👤 Author

**Dennie Truong**
Colby College '24
Environmental Science · Biology · Mathematics

### Acknowledgments

Gina Ralph · Susanne Craig · Ian Carroll · Bob Swap · Isha Chinniah
**SARP East Undergraduate Research Program**

---

## 🔑 Keywords

`Environmental Science` · `Algal Blooms` · `Phytoplankton` · `James River` · `Chesapeake Bay` · `LANDSAT 8` · `Remote Sensing` · `Chlorophyll-a` · `Generalized Additive Models` · `GAM` · `Water Quality` · `Environmental Data Analysis` · `Harmful Algal Blooms`

---

> **Research takeaway:** Combining long-term environmental monitoring with satellite remote sensing provides a promising approach for understanding the environmental drivers and spatial distribution of algal blooms.
