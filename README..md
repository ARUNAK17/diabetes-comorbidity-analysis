# Diabetes Comorbidity & Readmission Analysis  
### Interpretable Phenotyping Using Association Rule Mining

## Overview
This project investigates **why diabetic patients are readmitted to hospitals** by applying **Association Rule Mining (ARM)** instead of black-box predictive models.  
The goal is to uncover **clinically interpretable patient phenotypes** that explain different readmission mechanisms.

This work was completed as part of my **MSc in Data Analytics** and emphasizes **explainability, transparency, and applied healthcare analytics**.

---

## Problem Motivation
Most healthcare readmission studies focus on *predicting* readmission risk, offering limited insight into the **underlying clinical reasons** behind readmissions.  
Such models often lack interpretability, reducing their usefulness for clinicians and healthcare decision-makers.

This project addresses that gap by using **rule-based analytics** to explain readmission patterns at a **subgroup (phenotype) level**.

---

## Methodology
- Association Rule Mining using **FP-Growth**
- ICD-9 diagnostic codes reclassified into clinically meaningful categories
- Hospital encounters transformed into transactional data
- Rules filtered using **support, confidence, and lift**
- Recurrent rule patterns grouped into interpretable patient phenotypes

Framework used: **CRISP-DM**

---

## Dataset
- 101,766 hospital encounters  
- 130 U.S. hospitals  
- Public UCI Diabetes Readmission dataset  
- Analysis focused on readmitted encounters for clearer pattern discovery

---

## Results: Identified Readmission Phenotypes

| Phenotype | Distinguishing Pattern |
|---------|------------------------|
| **Cardiometabolic & Multi-System Comorbidity** | Cardiovascular and endocrine condition clusters with multiple systemic complications |
| **Chronic Care Complexity** | Recurrent follow-up visits, long-term care markers, and prolonged treatment pathways |
| **Acute Metabolic Instability** | Insulin adjustments combined with metabolic disruptions preceding short-term readmissions |

These phenotypes represent **distinct readmission mechanisms**, demonstrating that diabetic readmission is not a single homogeneous process.

---

## Key Insights
- Readmissions arise from **different clinical pathways**, not a single risk profile
- Rule-based phenotyping provides **transparent and explainable insights**
- Results can support:
  - Discharge planning
  - Targeted follow-up strategies
  - Healthcare resource prioritization

---

## Technologies Used
- Python (Jupyter Notebook)
- Pandas, NumPy
- MLxtend (FP-Growth)
- Scikit-Learn
- Matplotlib, Seaborn

---

## Repository Contents
- Jupyter Notebook implementing the full ARM workflow
- Preprocessed dataset
- Association rule outputs
- Phenotype mapping and analysis

---

## Academic Context
This project was submitted in partial fulfilment of the **MSc in Data Analytics** degree and focuses on **interpretability over prediction**, aligning analytics with real-world healthcare decision-making.

---

## Disclaimer
This analysis is exploratory and non-causal.  
Results are intended to support healthcare analytics and research, not replace clinical judgment.

## Repository Structure
- `dataset/` – Input dataset used for analysis
- `notebook_file/` – Jupyter notebook implementing the full ARM workflow
- `result dataset/` – Exported association rule and itemset results
