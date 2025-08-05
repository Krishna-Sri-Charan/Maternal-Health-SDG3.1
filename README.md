# Tracking Maternal Health Progress Toward SDG 3.1: A Global Data Analysis

## 📌 Overview
This repository documents the **capstone project** completed during the **IBM SkillsBuild 4-Week Internship on AI & Cloud Technologies**.  
The program is a collaborative initiative by the **Edunet Foundation**, **AICTE**, and **IBM SkillsBuild**.

The project focuses on **analyzing and predicting Maternal Mortality Ratio (MMR)** using the AI Kosh Sustainable Development Goals dataset to monitor progress toward **SDG 3.1** — reducing global MMR to **less than 70 per 100,000 live births by 2030**.

---

## 📝 Table of Contents
- [Intern Details](#-intern-details)
- [About the Internship](#-about-the-internship)
- [Project: Tracking Maternal Health Progress Toward SDG 3.1](#-project-tracking-maternal-health-progress-toward-sdg-31)
  - Problem Statement
  - Solution Overview
- [⚙️ Technology Stack](#%EF%B8%8F-technology-stack)
- [🚀 Project Workflow](#-project-workflow)
- [📊 Results](#-results)

---

## 👨‍💻 Intern Details
**Name:** Yerramsetti Krishna Sri Charan  
**Institute:** CMR College of Engineering and Technology  
**Department:** CSM Department  
**Duration:** 4 Weeks *(15th July 2025 – 7th August 2025)*

---

## 📖 About the Internship
The **4-week program** was designed to provide practical skills in **AI and Cloud Computing** using IBM SkillsBuild and IBM Cloud platforms. It included weekly virtual sessions, mentor guidance, and hands-on labs.

**Curriculum Outline:**
- **Week 1:** Internship Orientation, IBM Cloud Registration, Introduction to Artificial Intelligence  
- **Week 2:** Data Analytics concepts, Hands-On Labs, Cloud EDA  
- **Week 3 & 4:** AI/ML experiments on IBM Cloud using AutoAI, Project development, and Deployment

**Completion Requirements:**
- Active participation in sessions
- Completion of at least **two IBM SkillsBuild courses**
- Submission of the final capstone project

---

## 💡 Project: Tracking Maternal Health Progress Toward SDG 3.1

### Problem Statement
Despite global commitments to maternal health, the **maternal mortality ratio (MMR)** still exceeds the **SDG 3.1** target of 70 deaths per 100,000 live births by 2030 in many countries.  
Monitoring progress is difficult due to disparities in:
- Health infrastructure
- Antenatal care coverage
- Adolescent birth rates
- Skilled birth assistance  

A **data-driven analysis** is essential to identify high-risk areas and guide policy.

---

### Solution Overview
An **end-to-end AI-powered analytical system** was developed using **IBM Cloud AutoAI** that:
- Ingests multi-country health data from the AI Kosh SDG dataset
- Analyzes **key health indicators** affecting MMR
- Builds predictive models for estimating MMR
- Visualizes trends and highlights at-risk regions
- Deploys the best-performing model as a web service

---

## ⚙️ Technology Stack
**Cloud Platform:** IBM Cloud Lite  
**AI/ML Service:** IBM Watson Studio (AutoAI)  
**Deployment Service:** IBM Watson Machine Learning  

**Algorithms Used:**
- Decision Tree Regressor
- XGBoost Regressor *(Best Performing)*

**Core Features:**
- Antenatal Care Coverage (%)
- Skilled Birth Attendance (%)
- Adolescent Birth Rate
- Healthcare Expenditure
- Historical MMR data

---

## 🚀 Project Workflow
1. **Data Ingestion:**  
   AI Kosh SDG dataset uploaded to IBM Cloud Object Storage.
2. **Automated Model Building:**  
   AutoAI configured for regression, target = `DataValue` (MMR).
3. **Model Selection:**  
   AutoAI generated 9 pipelines → Best model: **XGBoost Regressor**.
4. **Deployment:**  
   Model deployed in IBM Watson Machine Learning for real-time predictions.
5. **Testing:**  
   Predictions validated with test data to ensure accuracy.

---

## 📊 Results
**Best Model:** Batched Tree Ensemble Regressor (XGBoost)  

| Metric | Holdout Score | Cross Validation Score |
|--------|--------------|------------------------|
| R² | 0.981 | 0.858 |
| RMSE | 26.665 | 84.564 |
| MAE | 14.343 | 26.763 |
| Explained Variance | 0.981 | 0.858 |

**Screenshots:**
- Progress Map → [Progress Map](results/progress_map.png)
- Model Metrics → [Model Metrics](results/model_metrics.png)
- Predictions → [Predictions](results/predictions.png)
