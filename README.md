# Heart Disease Analysis with Tableau

A data analytics project that explores key lifestyle and clinical indicators of heart disease and presents the findings through interactive Tableau dashboards and stories, embedded in a lightweight Flask web application.

## demo Link : https://drive.google.com/file/d/1udTTlsVybba_fxRgQDEcwi4NYnJviWrN/view?usp=sharing
## Overview

Heart disease remains one of the leading causes of death worldwide, and many of its risk factors — smoking, physical inactivity, poor sleep, BMI, diabetes, and more — are observable in everyday health data. This project analyzes a patient-level health survey dataset to uncover patterns and relationships between these indicators and the presence of heart disease, then communicates the insights through visual dashboards rather than a predictive model.

## Dataset

**File:** [`5. Project Development Phase/Heart_new2.csv`](5.%20Project%20Development%20Phase/Heart_new2.csv)

The dataset contains 4,500 patient-level records with the following 18 demographic, lifestyle, and clinical fields:

| Column | Description |
|---|---|
| `HeartDisease` | Whether the patient has heart disease (Yes/No) |
| `BMI` | Body Mass Index |
| `Smoking` | Smoking status |
| `AlcoholDrinking` | Alcohol consumption status |
| `Stroke` | History of stroke |
| `PhysicalHealth` | Days of poor physical health (last 30 days) |
| `MentalHealth` | Days of poor mental health (last 30 days) |
| `DiffWalking` | Difficulty walking/climbing stairs |
| `Sex` | Patient sex |
| `AgeCategory` | Age bracket |
| `Race` | Race/ethnicity |
| `Diabetic` | Diabetes status |
| `PhysicalActivity` | Physical activity in the last 30 days |
| `GenHealth` | Self-reported general health |
| `SleepTime` | Average hours of sleep |
| `Asthma` | Asthma status |
| `KidneyDisease` | Kidney disease status |
| `SkinCancer` | Skin cancer status |

## Tech Stack

| Layer | Technology |
|---|---|
| Data preparation & analysis | Tableau Desktop |
| Data visualization & KPIs | Tableau Calculated Fields, Dashboards, Story Points |
| Dashboard publishing | Tableau Public (cloud) |
| Web application logic | Python, Flask |
| Frontend | HTML5, CSS3, Bootstrap, JavaScript |
| Data storage | CSV dataset (local file system) |

**Architecture:** a three-tier design — a data layer (CSV dataset processed and visualized in Tableau), a visualization layer (Tableau dashboards/stories published to Tableau Public), and a presentation layer (a Flask + Bootstrap web app that embeds the published dashboards for end users).

## Business Questions Explored

The dashboards and story were built to answer questions such as:

- Which age category has the highest prevalence of heart disease?
- Does smoking increase the risk of heart disease?
- Which gender is more affected by heart disease?
- How does BMI relate to diabetic status?
- What impact does physical activity have on heart disease risk?
- Which demographic factors are most strongly associated with heart disease?

The published dashboards include KPI cards (total records, heart disease cases, stroke cases, average BMI, high-risk patients, obese patients), 10 visualizations, 7 interactive filters, and a 6-point Tableau Story.

## Project Structure

This repository follows a phase-based project structure:

```
1. Brainstorming & Ideation/     Problem statement, idea prioritization, empathy map
2. Requirement Analysis/         Customer journey map, data flow diagrams, solution
                                  requirements, technology stack
3. Project Design Phase/         Problem-solution fit, proposed solution, solution
                                  architecture
4.Project Planning Phase/        Project planning template
5. Project Development Phase/    Dataset (Heart_new2.csv) and data preparation /
                                  dashboard & story documentation
6. Performance Testing/          Tableau performance testing documentation
7.Doc and Demo/                  Final project report and demo video link
```

## Key Deliverables

- **Dataset:** [`5. Project Development Phase/Heart_new2.csv`](<5. Project Development Phase/Heart_new2.csv>)
- **Data preparation & business questions:** [`5. Project Development Phase/1st PDF Data Preparation and Business Questions with Visuals.pdf`](<5. Project Development Phase/1st PDF Data Preparation and Business Questions with Visuals.pdf>)
- **Dashboard & story:** [`5. Project Development Phase/2nd PDF for Project Dash and Story.pdf`](<5. Project Development Phase/2nd PDF for Project Dash and Story.pdf>)
- **Final report:** [`7.Doc and Demo/Final Report.pdf`](<7.Doc and Demo/Final Report.pdf>)
- **Demo video:** see [`7.Doc and Demo/Demo link.pdf`](<7.Doc and Demo/Demo link.pdf>)

## How It Works

1. The heart disease dataset is cleaned and prepared in Tableau Desktop.
2. Calculated fields and KPIs are derived to analyze relationships between lifestyle/clinical factors and heart disease.
3. Interactive dashboards and a guided story are built to surface the insights.
4. The dashboards and story are published to Tableau Public.
5. A Flask web application (Bootstrap-based UI) embeds the published Tableau visualizations so end users can explore project information, dashboards, and developer details through a single web interface.

## Notes

- This repository is the **documentation and deliverables archive** for the internship project (phase reports, dataset, and final report). The runnable Flask web application that embeds the Tableau dashboards lives in a separate GitHub repository referenced in the Final Report: [`Heart-Disease-Analysis-with-Tableau`](https://github.com/thiragatisuryasri-analyst/Heart-Disease-Analysis-with-Tableau).
- This project is a data-visualization/analytics deliverable (SmartBridge/SmartInternz-style internship project) rather than a machine-learning prediction system — its goal is to surface and communicate insights about heart disease risk factors through Tableau dashboards, not to serve predictions. Predictive ML models and cloud deployment are listed as future scope in the Final Report.
- Live Tableau Public dashboard/story links and further project details are available in the [Final Report](<7.Doc and Demo/Final Report.pdf>).
