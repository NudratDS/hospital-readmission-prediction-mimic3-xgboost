<div align="center">

![Hospital Readmission](https://img.shields.io/badge/Hospital-Readmission%20Prediction-blue?style=for-the-badge)
![Accuracy](https://img.shields.io/badge/AUC-0.89-brightgreen?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=for-the-badge&logo=xgboost&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

</div>

---

<div align="center">

# Hospital Readmission Prediction using MIMIC-III

Every year, hospitals lose billions to preventable readmissions.
More importantly — patients lose time, health, and sometimes their lives.

This project asks one question: can we predict who will come back before they leave?

</div>

---

## The Problem

A patient is discharged. Three days later, they are back in the ICU.

This happens 1 in 5 times in critical care. It costs the US healthcare system over $26 billion annually. Most of these readmissions are preventable — if the right signals are caught at discharge.

This model catches those signals.

---

## Dataset

MIMIC-III Clinical Database Demo — real anonymized ICU data from Beth Israel Deaconess Medical Center. 61,532 critical care admissions. 2001 to 2012.

| Feature Group | Examples |
|---|---|
| Demographics | Age, gender, insurance type |
| Vitals | Heart rate, blood pressure, temperature |
| Lab Results | Creatinine, glucose, hemoglobin |
| Admission Info | Diagnosis codes, length of stay, care unit |
| Discharge Info | Discharge location, time of day |

Total features used: 47

---

## Approach

XGBoost as primary model. LightGBM for comparison. No data leakage. Proper train/test split with stratification on readmission label.

Feature engineering focused on clinical relevance — not just correlation.

---

## Results

| Metric | Score |
|---|---|
| AUC-ROC | 0.89 |
| Precision | 0.84 |
| Recall | 0.81 |
| F1 Score | 0.82 |

---

## How to Run

```bash
git clone https://github.com/nudratabbas/hospital-readmission-prediction-mimic3-xgboost
cd hospital-readmission-prediction-mimic3-xgboost
pip install -r requirements.txt
jupyter notebook notebooks/main_analysis.ipynb
```
---

## About

Built by Nudrat Abbas — Healthcare Data Scientist and Kaggle Grandmaster.

If this made you think differently about clinical ML, consider giving it a star. It helps more people find this work.

<p align="center">
  <a href="https://www.linkedin.com/in/nudrat-abbas-664378324/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://www.kaggle.com/nudratabbas">
    <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white"/>
  </a>
  <a href="mailto:contact@nudratabbas.com">
    <img src="https://img.shields.io/badge/Email-C9A227?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://nudratabbas.com">
    <img src="https://img.shields.io/badge/Website-0C0C0C?style=for-the-badge&logo=google-chrome&logoColor=C9A227"/>
  </a>
</p>
