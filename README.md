# Remote Patient Monitoring Readmission Prediction

This project explores how machine learning and business intelligence can be used to support decision-making in a Remote Patient Monitoring (RPM) program. The main goal was to predict the likelihood of hospital readmission and translate the model outputs into a practical Power BI dashboard for managerial and operational use.

The original dataset cannot be shared due to privacy and confidentiality restrictions. This repository focuses on the project methodology, model logic, dashboard design, and decision-support value without exposing patient-level data.

---

## Project Background

Remote Patient Monitoring programs generate valuable data from patient demographics, device readings, alerts, and clinical notes. However, this information is often spread across different sources and may not be immediately useful for identifying patients who are at higher risk of readmission.

This project was designed to turn those data sources into a structured analytics workflow that could help healthcare teams better understand readmission risk and support more proactive follow-up decisions.

---

## What This Project Covers

The project followed an end-to-end analytics process:

1. Reviewed clinical notes to identify readmitted patients, inaccurate readings, and alert-related issues.
2. Cleaned and combined patient, reading, alert, and note-based information.
3. Created device-level alert ratio features to better represent abnormal monitoring patterns.
4. Trained and evaluated Logistic Regression and Decision Tree models.
5. Extracted model coefficients and decision rules for interpretation.
6. Rebuilt the model logic inside Power BI using DAX measures.
7. Designed a dashboard to communicate risk scores, model outputs, and managerial insights.

---

## Key Features

- Clinical-note review for readmission and data-quality validation
- Alert ratio calculation for monitored devices
- Logistic Regression model for estimating readmission probability
- Decision Tree model for explainable readmission classification
- DAX-based implementation of model logic in Power BI
- Dashboard pages for risk interpretation, alert analysis, and recommendations
- Privacy-conscious project structure without confidential patient records

---

## Machine Learning Approach

Two models were used in this project:

### Logistic Regression

Logistic Regression was used to estimate the chance of readmission. The model coefficients were extracted and translated into DAX measures, allowing the dashboard to calculate readmission probability without requiring the original dataset.

### Decision Tree

The Decision Tree model was used to provide an interpretable classification of readmission status. The decision rules were extracted and implemented in Power BI so that users could understand how different risk factors contributed to the final prediction.

---

## Power BI Dashboard

The Power BI dashboard was created to make the model outputs easier to understand and use. Instead of displaying confidential patient-level data, the dashboard represents the model logic through calculated measures, decision rules, and interactive inputs.

The dashboard includes sections for:

- Project overview
- Alert ratio calculation
- Readmission risk estimation using Logistic Regression
- Readmission status prediction using Decision Tree rules
- Managerial insights and recommendations

This makes the dashboard a practical decision-support tool rather than only a technical modeling exercise.

---

## Data Privacy

The original RPM dataset is not included in this repository.

To protect confidentiality, this repository does not contain:

- patient-level records
- clinical notes
- raw device readings
- raw alert files
- identifiable patient information
- original confidential extracts

The shared materials are intended to demonstrate the project workflow, modeling logic, dashboard design, and analytical thinking behind the solution.

---

## Repository Structure

```text
remote-patient-monitoring-readmission/
│
├── README.md
│
├── dashboard/
│   ├── dashboard_screenshots/
│   └── dashboard_documentation.md
│
├── docs/
│   ├── methodology.md
│   ├── feature_definitions.md
│   ├── model_interpretation.md
│   └── privacy_statement.md
│
└── src/
    ├── preprocessing_template.py
    ├── feature_engineering_template.py
    └── model_training_template.py
