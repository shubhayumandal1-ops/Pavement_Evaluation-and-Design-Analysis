# Vehicle Damage Factor Analysis & Pavement Design for a National Highway Section

## 📌 Overview

This repository documents the analysis and design work carried out for a selected stretch of a **National Highway (NH)**, focusing on determining the **Vehicle Damage Factor (VDF)** from axle load data and using it to design the pavement structure (flexible/rigid) as per **IRC (Indian Roads Congress)** guidelines.

The Vehicle Damage Factor is a critical input in pavement design — it converts the traffic mix of commercial vehicles into an equivalent number of standard axle load repetitions (ESAL), which directly governs the thickness and material composition of the pavement layers.

---

## 🎯 Objectives

- To conduct/analyze traffic volume and axle load survey data for the selected NH stretch.
- To classify commercial vehicles by axle configuration (single, tandem, tridem axles).
- To compute the **Vehicle Damage Factor (VDF)** using the fourth power law.
- To estimate the **design traffic (cumulative ESAL)** over the design life.
- To design the pavement (flexible or rigid) using IRC codes (IRC:37, IRC:58, or IRC:SP:84 as applicable).
- To document assumptions, calculations, and final design recommendations.

---

## 🛣️ Study Area

- **Highway Section:** *[NH number / chainage / route name]*
- **Length of stretch analyzed:** *[X km]*
- **Terrain type:** *[Plain / Rolling / Hilly]*
- **Traffic category:** *[e.g., >450 CVPD]*

---

## 🧮 Methodology

1. **Traffic Data Collection**
   - Classified traffic volume count (7-day/24-hour survey)
   - Axle load survey using weigh-in-motion (WIM) or axle load survey data

2. **Vehicle Damage Factor Computation**
   - Axle load spectrum analysis for each vehicle class
   - Application of the **fourth power law**:
     
     VDF = Σ (Axle Load / Standard Axle Load)⁴

   - Weighted average VDF derived from the observed axle load distribution

3. **Design Traffic Estimation**
   - Traffic growth rate projection
   - Lane distribution factor and directional distribution factor
   - Cumulative Standard Axles (CSA) calculation over design life (e.g., 15/20 years)

4. **Pavement Design**
   - Flexible pavement design as per **IRC:37-2018** (using CBR value of subgrade and design traffic)
   - OR Rigid pavement design as per **IRC:58-2015** (using flexural strength of concrete and design traffic)
   - Layer-wise thickness determination (subgrade, sub-base, base, surface course)

---

## 🏗️ Architecture / Workflow Diagram


*Pipeline: field data collection (traffic + axle load surveys) → data processing → VDF computation → design traffic (CSA) estimation → flexible/rigid pavement design → final layer thicknesses and drawings.*

---

## 📊 Key Parameters Used

| Parameter | Value |
|---|---|
| Design life | *[e.g., 15 years]* |
| Traffic growth rate | *[e.g., 5–6% p.a.]* |
| Vehicle Damage Factor (VDF) | *[computed value]* |
| Design CBR of subgrade | *[value %]* |
| Cumulative Standard Axles (CSA) | *[value in msa]* |
| Pavement type | *[Flexible / Rigid]* |

---

## 🧰 Tools & Software Used

- Microsoft Excel / Python (for data analysis and VDF computation)
- IRC design charts/nomograms or IITPAVE / KENPAVE software (if used for flexible pavement analysis)
- AutoCAD / QGIS (for alignment and cross-section drawings, if applicable)

---

## 📁 Repository Structure

```
├── data/                  # Raw and processed traffic & axle load survey data
├── calculations/          # VDF and ESAL computation sheets/scripts
├── design/                # Pavement design calculations and layer thickness outputs
├── drawings/              # Cross-sections, typical pavement design drawings
├── report/                # Final project report / documentation
└── README.md
```

---

## 📈 Results Summary

*[Brief summary of the final VDF value obtained, design traffic in msa, and the recommended pavement composition — e.g., total pavement thickness, layer-wise breakdown.]*

---

## 📚 References

- IRC:37-2018 — *Guidelines for the Design of Flexible Pavements*
- IRC:58-2015 — *Guidelines for the Design of Plain Jointed Rigid Pavements for Highways*
- IRC:SP:84 — *Manual of Specifications and Standards for Two-laning of Highways*
- Ministry of Road Transport and Highways (MoRTH) Specifications

---

## 👤 Author

*Shubhayu Mandal*
*Civil Engineering Undergrad at NIT Rourkela*

---

## 📄 License

This project is for academic/research purposes. Feel free to fork and adapt with attribution.
