# CDSS-Project
# Clinical Decision Support System (CDSS) Framework for Allergic Rhinitis & Glioblastoma

This repository presents a comprehensive Clinical Decision Support System (CDSS) framework developed to enhance diagnostic precision and treatment outcomes for two distinct yet high-impact conditions: **Allergic Rhinitis (AR)** and **Glioblastoma (GBM)**. 

This project was completed as part of the **INFO-B 642: Clinical Decision Support Systems** course at the **Luddy School of Informatics, Computing, and Engineering**, Indiana University Indianapolis, under the guidance of **Dr. Josette Jones (RN, Ph.D., FAMIA)**.

---

## 📌 Project Overview

### 🎯 Objective
To develop a dual-purpose CDSS capable of:
- Assisting clinicians in the **accurate diagnosis of Allergic Rhinitis**, especially in complex or comorbid cases.
- Supporting **personalized treatment planning for Glioblastoma**, using molecular markers and therapy monitoring.

### 🧠 Clinical Focus Areas
- **Allergic Rhinitis (AR)**: Incorporates diagnostic pathways using Skin Prick Tests (SPT), Allergen-Specific IgE, Basophil Activation Test (BAT), and RAST, with context-aware rules for asthma comorbidity and seasonal allergen exposure.
- **Glioblastoma (GBM)**: Features treatment recommendations for Temozolomide, Bevacizumab, radiotherapy, and Tumor Treating Fields (TTFs), with biomarkers like MGMT methylation and MRI data integration.

---

## Key Components

### Literature Review
In-depth synthesis of evidence-based clinical guidelines and diagnostic tools using PubMed and ClinicalKey to inform Clinical Decision Rules (CDRs) and CDSS architecture.

### Cohort Creation with ATLAS (OHDSI)
- Developed patient cohorts for AR and GBM using standardized terminologies (ICD-10, SNOMED CT).
- Applied inclusion/exclusion criteria with real-world characteristics (e.g., age range, comorbidities, treatment history).
- Exported cohorts used to inform rule-based alerts and care pathways.

###  OpenEMR Integration
- Configured **custom rule categories and alerts** for AR and GBM within OpenEMR.
- Integrated patient demographics, diagnosis codes, treatment timelines, and clinical triggers for real-time decision support.
- Enabled follow-up reminders and outcome tracking aligned with clinical workflows.


### 🌳 Decision Trees & Prototype
- Designed visual decision trees mapping stepwise diagnostic and therapeutic guidance for both conditions.
- Developed a functional prototype simulating clinician-CDSS interaction with dynamic rule logic and alert triggers.

---

## 🛠️ Technologies & Tools
- **Platforms**: OHDSI/ATLAS, OpenEMR  
- **Terminologies**: SNOMED CT, LOINC, ICD-10  
- **Modeling & Analytics**: Bayesian Networks, Markov Chains, Predictive Analytics  
- **Compliance**: HIPAA, IRB principles  

---



