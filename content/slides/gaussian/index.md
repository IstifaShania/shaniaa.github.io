---
marp: true
theme: default
paginate: true
---

# Evaluating the Impact of Adding Gaussian Noise  
## as Data Augmentation on Electronic Nose  
## for Black Tea Quality Classification  
**Istifa Shania Putri, B.Sc.**  
Supervisor: Dr. Nur Ulfa Maulidevi, S.T., M.Sc.  
School of Electrical Engineering and Informatics  
Bandung Institute of Technology

---

## Background (1/3)

- Main attributes for black tea quality: aroma, color, taste  
- Traditional assessment relies on experts:  
  subjective, costly, time-consuming, hard to standardize  
- **Electronic Nose** as a solution

---

## Background (2/3)

- Model quality depends heavily on training data size  
- Challenges:
  - Collecting e-nose data is time-consuming  
  - Dependence on labeled samples limits generalization

---

## Background (3/3)

- Fang et al. (2022):  
  Feature-based algorithms may **lose key information**  
  → leads to reduced model performance

---

## Research Questions

- How to overcome data collection challenges and dependence on labeled samples in e-nose-based classification?  
- How to develop aroma recognition that is less reliant on domain expertise to reduce information loss?

---

## Research Objectives

- Develop a black tea quality classification model using electronic nose  
- Evaluate an **end-to-end learning** approach with  
  **data augmentation** and **CNN architecture**

---

## Problem Analysis

- Accuracy is highly influenced by the feature extraction method  
- Deep learning models perform poorly with small datasets  
- **Data augmentation is necessary** to enrich training samples

---

## Proposed Solution

- **Noise Levels:** 0.01, 0.03, 0.05, 0.1, 0.2, 0.3  
- **Scenario 1:**
  - KS test, MANOVA, Aroma Profile, LDA  
- **Scenario 2:**
  - Metric scores, Confusion Matrix  
- **Models:** ResNet18, ResNet34, ResNet50

---

## Dataset

- Electronic nose readings for 3 tea quality levels (Q1, Q2, Q3)  
- 12 gas sensors  
- 1550 rows per class  
- Train-test split:  
  - Without augmentation: 50:50  
  - With augmentation: 80:20

---

## Classification Models

- Deep CNN architectures used:
  - **ResNet18**
  - **ResNet34**
  - **ResNet50**

---

## Augmentation Results

- Visual comparison: original vs. augmented signals (noise 0.01 & 0.3)  
- Aroma profile evaluations: Q1, Q2, Q3  
- Feature separability via LDA

---

## 2D Classification Evaluation (1/2)

- Transfer learning significantly improves accuracy across all noise levels  
- Example:  
  - ResNet18 (noise 0.01): 34.71% → 92.66%  
  - ResNet34 shows best robustness at high noise (0.3 → 89.90%)

---

## 2D Classification Evaluation (2/2)

- **ResNet34 + Transfer Learning**:
  - Highest and most stable precision, recall, F1-score (~0.90 avg)  
- **ResNet50 without TL** drops sharply:  
  - F1-score: 0.49 vs. 0.71 (with TL)  
- Emphasizes importance of transfer learning under high noise

---

## Conclusion

- Adding Gaussian noise helps model generalization at low noise levels  
- Simulates real-world signal variation  
- Transfer learning greatly boosts robustness and accuracy  
- **ResNet34** offers the best trade-off between complexity and performance  
- **ResNet50** less stable under high noise

---

## Recommendations

- **Optimal noise level** found around 0.1  
- Future work: explore combining Gaussian noise with  
  other augmentation methods (e.g., scaling, linear interpolation)  
- High noise (> 0.15) decreases performance →  
  develop models with better **noise tolerance**

---
