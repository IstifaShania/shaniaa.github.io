---
title: "Detection of Fluoride Content in Black Tea"
summary: "Slides from ICST 2023"
slides:
  theme: white
  highlight_style: github
  transition: slide
---

# Introduction

- Fluoride in black tea: benefit vs fluorosis risk
- Existing methods: expensive and limited
- E-nose used for classification, not concentration

---

# Research Goal

- Develop system to detect fluoride content in black tea using e-nose
- Estimate fluoride based on aroma trend and Rs/Ro ratio
- Apply Partial Least Squares Regression (PLSR)

---

# Scope

- Focus on software-based e-nose system under optimal conditions
- Sample from existing research
- Use of tea types: BOP, BP II, Bohea

---

# Tools & Materials

- E-nose with TGS832 sensor
- Jupyter Notebook, Excel
- Tea types (KW1, KW2, KW3)

---

# System Framework

1. Pre-processing data
2. Apply PLSR
3. Compare with reference concentration (Rs/Ro)

---

# Design of Experiment

- Use sensor response to build model
- Refer to Sabilla (2017) for Rs/Ro reference

---

# Results

### KW1
- R² = 0.986620
- RMSE = 0.004642

### KW2
- R² = 0.994791
- RMSE = 0.010772

### KW3
- R² = 0.994054
- RMSE = 0.005324

---

# Conclusion

- Model estimates fluoride concentration accurately using aroma
- System shows high performance on all tea qualities
- No observed correlation between tea quality and fluoride concentration

---

# Thank You!
