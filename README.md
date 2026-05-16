# Remote Patient Monitoring Readmission Prediction

This project looks at how machine learning and Power BI can be used to support readmission risk analysis in a Remote Patient Monitoring program. The goal was to identify patients with a higher chance of hospital readmission and present the results in a dashboard that could be understood by both technical and non-technical users.

The original dataset cannot be shared because it contains confidential healthcare information. For that reason, this repository focuses on the workflow, model logic, dashboard design, and the business value of the project without including patient records.

---

## Project Background

Remote Patient Monitoring programs collect different types of information, including patient details, device readings, alerts, and clinical notes. These sources can be useful for understanding patient risk, but they usually need to be cleaned, connected, and summarized before they can support decision-making.

This project was built to turn those separate data sources into a structured process for predicting readmission risk and presenting the results in a practical way.

---

## Project Workflow

The project followed these main steps:

1. Reviewed clinical notes to identify readmitted patients, inaccurate readings, and issues with alerts.
2. Cleaned and combined patient information, readings, alerts, and findings from the notes.
3. Calculated alert ratios for each monitoring device, such as blood pressure, oxygen, and weight.
4. Built and tested Logistic Regression and Decision Tree models.
5. Used Logistic Regression coefficients to estimate the chance of readmission.
6. Converted Decision Tree outputs into readable decision rules.
7. Recreated the model logic in Power BI using DAX measures.
8. Designed a dashboard to present risk estimates, predicted status, and recommendations.

---

## Key Components

- Review of clinical notes to support readmission tracking and data validation
- Calculation of alert ratios for monitored readings
- Logistic Regression model to estimate readmission probability
- Decision Tree model to provide clear prediction rules
- DAX measures to reproduce model logic inside Power BI
- Dashboard pages for risk estimation, alert ratio calculation, model output, and recommendations
- Project structure designed to share the work without exposing confidential data

---

## Machine Learning Approach

Two models were used in this project.

### Logistic Regression

Logistic Regression was used to estimate the probability of readmission. After the model was trained, the coefficients were extracted and used in Power BI so that the dashboard could calculate the chance of readmission directly through DAX measures.

### Decision Tree

The Decision Tree model was used to classify readmission status in a more explainable way. Its decision rules were extracted and implemented in Power BI so that users could see how different inputs affected the final prediction.

---

## Power BI Dashboard

The Power BI dashboard was created to make the model outputs easier to use. Instead of showing confidential patient data, the dashboard uses DAX measures, input fields, and model rules to demonstrate how readmission risk can be estimated.

The dashboard includes pages for:

- Project overview
- Alert ratio calculation
- Readmission risk estimation using Logistic Regression
- Readmission status prediction using Decision Tree rules
- Managerial insights and recommendations

The dashboard connects the technical model results to decisions that managers and care teams may need to make.
