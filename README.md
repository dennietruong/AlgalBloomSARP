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

The project focuses on two primary questions:

1. **What environmental factors are driving algal blooms?**
2. **What is the efficacy of LANDSAT 8 data in characterizing algal blooms?**

---

## 🗺️ Study Site & Data

The study examines a section of the **James River** using observations from **five sampling stations** collected between:

**January 2013 – December 2022**

Monthly monitoring data were collected through collaborative efforts involving:

* Maryland Department of Natural Resources
* Morgan State University
* Old Dominion University
* Virginia Department of Environmental Quality (VDEQ)

### Variables of Interest

The primary environmental variables examined were:

| Variable                  | Role in Analysis                                                    |
| ------------------------- | ------------------------------------------------------------------- |
| **Chlorophyll-a (Chl-a)** | Proxy for phytoplankton/algal biomass                               |
| **Ammonium (NH₄⁺)**       | Nitrogen source                                                     |
| **Phosphate (PO₄³⁻)**     | Phosphorus source                                                   |
| **Turbidity**             | Indicator associated with sediments/detritus and light availability |
| **Water Temperature**     | Environmental factor influencing biological activity                |

Chlorophyll-a was used as a proxy for phytoplankton abundance and algal-bloom activity.

---

## 📊 Statistical Analysis

A **Generalized Additive Model (GAM)** was used to investigate relationships between chlorophyll-a and environmental variables over time.

The model incorporated:

* Ammonium
* Phosphate
* Turbidity
* Water temperature
* Temporal trends across the study period

### Model Performance

The resulting model explained approximately **71.7% of the deviance**.

| Metric                 | Value |
| ---------------------- | ----: |
| **R²**                 | 0.709 |
| **RMSE**               |  7.83 |
| **MAE**                |  5.43 |
| **Explained Deviance** | 71.7% |

---

## 🌱 Environmental Drivers

The analysis suggests that **nutrient availability and water temperature** are important factors associated with phytoplankton growth in the James River.

### Nitrogen — Ammonium

Ammonium appears to be an important inorganic nitrogen source for phytoplankton. The analysis indicates that the relative importance of nitrogen and phosphorus limitation changes depending on nutrient availability.

### Phosphorus — Phosphate

Phytoplankton can utilize phosphate as a source of phosphorus. Model predictions indicate that phosphorus limitation is particularly apparent under lower ammonium conditions.

### Nutrient Limitation

Using the TN/TP framework described by Guildford and Hecky, the James River appears to be primarily:

* **Nitrogen limited**, or
* **Nitrogen and phosphorus co-limited**

The model's marginal predictions also suggest a shift in limiting nutrients as ammonium availability increases.

---

## 🌡️ Water Temperature

Increasing water temperature was associated with **increasing chlorophyll-a**.

One possible explanation is that warmer conditions may increase biological activity and support photosynthetic processes.

The project notes that algal blooms in the Chesapeake Bay have been observed within a temperature range of approximately **18.0–26.1°C**.

---

## 🌫️ Turbidity

Increasing turbidity was associated with **decreasing chlorophyll-a**.

One possible explanation is that highly turbid conditions may restrict phytoplankton growth by reducing available light.

The relationship may also be bidirectional: phytoplankton growth itself can contribute to turbidity by increasing shading within the water column.

---

## 🛰️ LANDSAT 8 Remote Sensing

The second component of the project evaluates the potential of **LANDSAT 8** data to characterize algal blooms across the James River.

LANDSAT 8 launched on **February 11, 2013** and provides multispectral imagery at **30-meter resolution** across a **185 km swath**.

### Spectral Bands Used

The chlorophyll model incorporated LANDSAT spectral information from:

* Coastal aerosol
* Blue
* Green
* Red
* Near infrared (NIR)

A chlorophyll model developed using **principal component analysis (PCA)** was used to derive chlorophyll-a estimates from LANDSAT spectral bands.

These estimates were then used to visualize predicted chlorophyll-a spatially along the James River.

---

## 🗓️ Spatial Characterization of Blooms

The LANDSAT-based chlorophyll model was used to examine conditions across the James River during three periods:

| Period              | LANDSAT Observation |
| ------------------- | ------------------- |
| **Pre-pandemic**    | July 27, 2019       |
| **During pandemic** | July 13, 2020       |
| **Post-pandemic**   | August 4, 2022      |

The resulting maps provide a spatial perspective that complements the long-term in-situ monitoring data.

---

## 🦠 COVID-19 Period

The analysis examined whether algal-bloom trends changed during the COVID-19 pandemic.

The results suggest that **algal-bloom trends were not substantially affected in 2020**, consistent with both the GAM and chlorophyll models.

---

## 📈 Key Findings

### 1. Nutrient availability is an important driver

The results suggest that **ammonium and phosphate availability** play important roles in phytoplankton growth.

### 2. Water temperature is positively associated with chlorophyll-a

Higher water temperatures were associated with increased chlorophyll-a concentrations.

### 3. Turbidity shows a negative association

Increasing turbidity was associated with decreasing chlorophyll-a, potentially because high turbidity limits light availability.

### 4. Bloom activity varies along the river

The **head of the James River experienced higher volumes of phytoplankton blooms on average compared with the mouth** of the river.

### 5. LANDSAT provides a means of spatial characterization

LANDSAT spectral data can be used to derive spatial estimates of chlorophyll-a, providing a way to extend observations beyond individual sampling stations.

### 6. Pandemic-era trends were relatively consistent

The analysis did not identify a substantial change in algal-bloom trends during 2020.

---

## ⚠️ Variables Excluded from the Analysis

Several potentially important environmental variables were excluded because of data availability:

* **Light** — necessary for photosynthesis
* **Carbon** — important for photosynthetic growth
* **Silica** — required for the growth of diatoms
* **Salinity** — influences the distribution of freshwater and marine plankton species

These variables represent potential areas for future analysis.

---

## 🧩 Conceptual Framework

The project considers algal-bloom dynamics as the result of interactions among environmental conditions:

```text
             Nutrient Availability
              /              \
             /                \
       Ammonium              Phosphate
             \                /
              \              /
               ↓            ↓
              Phytoplankton
                   ↓
             Chlorophyll-a
                   ↑
                   │
          Water Temperature
                   
          Turbidity ↔ Light Availability
```

Together, these relationships help explain the environmental conditions associated with phytoplankton growth in the James River.

---

## 🌎 Broader Applications

The findings may provide a foundation for:

* Identifying potential algal-bloom drivers in other aquatic systems
* Using environmental variables alongside satellite spectral data to identify blooms
* Expanding monitoring beyond fixed sampling stations
* Supporting monitoring programs for **harmful algal blooms (HABs)**
* Developing more spatially comprehensive approaches to aquatic ecosystem monitoring

The project therefore demonstrates how **field observations, statistical modeling, and satellite remote sensing** can be combined to investigate environmental change.

---

## 🛠️ Research Approach

```text
Long-Term Monitoring Data
          │
          ▼
   Data Exploration
          │
          ▼
 Generalized Additive
       Modeling
          │
          ├───────────────┐
          ▼               ▼
Environmental Drivers   Temporal Trends
          │               │
          └───────┬───────┘
                  ▼
          Chlorophyll-a
                  │
                  ▼
       LANDSAT 8 Analysis
                  │
                  ▼
     Spatial Bloom Mapping
```

---

## 📚 Project Context

This research was conducted through the **SARP East Undergraduate Research Program**, with support from researchers and mentors at VIMS and NASA Goddard.

### Acknowledgments

Special thanks to:

* **Gina Ralph** — VIMS
* **Susanne Craig** — NASA Goddard
* **Ian Carroll** — NASA Goddard
* **Bob Swap** — NASA Goddard
* **Isha Chinniah** — SARP East Undergraduate Research

And to the **SARP East program** for providing the opportunity, resources, and support for this research.

---

## 👤 Author

**Dennie Truong**
Colby College '24

Environmental Science · Biology · Mathematics

---

## 🔑 Keywords

`Environmental Science` · `Algal Blooms` · `Phytoplankton` · `James River` · `Chesapeake Bay` · `LANDSAT 8` · `Remote Sensing` · `Chlorophyll-a` · `Generalized Additive Models` · `GAM` · `Water Quality` · `Environmental Data Analysis` · `Harmful Algal Blooms`

---

> **Research takeaway:** Combining long-term environmental monitoring with satellite remote sensing provides a promising approach for understanding the environmental drivers and spatial distribution of algal blooms.
