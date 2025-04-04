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

# 🧠 Clinical Decision Rules (CDRs)

Below are two clinical decision rules developed and configured for use within a Clinical Decision Support System (CDSS) prototype in OpenEMR. These rules are evidence-based and aligned with current clinical guidelines for **Allergic Rhinitis** and **Glioblastoma** care pathways.

---

## 📌 1. Precision Allergen-Specific IgE Testing for Allergic Rhinitis

- **Author**: Poorva Reddy Vanga  
- **Status**: Active  
- **Source**:  
  Bousquet, J., Anto, J. M., Bachert, C., et al. (2020). *Allergic rhinitis*. Nature Reviews Disease Primers, 6(1).  
  [https://doi.org/10.1038/s41572-020-00227-0](https://doi.org/10.1038/s41572-020-00227-0)

### 🧬 Rule Logic:
- **Target Patient Population**:  
  Patients presenting with symptoms of Allergic Rhinitis **AND** for whom **Skin Prick Testing (SPT)** is contraindicated (e.g., due to severe eczema or antihistamine use).
  
- **Clinical Action**:  
  Recommend ordering **Allergen-Specific IgE** testing based on the patient’s clinical history and reported symptoms.

- **Purpose**:  
  Improve diagnostic accuracy in cases where SPT is not feasible, reducing diagnostic delay and enabling timely treatment planning.

---

## 📌 2. Monthly Monitoring of Temozolomide Therapy in Glioblastoma

- **Author**: Poorva Reddy Vanga  
- **Status**: Active  
- **Source**:  
  McKinnon, C., Nandhabalan, M., Murray, S. A., & Plaha, P. (2021). *Glioblastoma: Clinical presentation, diagnosis, and management*. BMJ, n1560.  
  [https://doi.org/10.1136/bmj.n1560](https://doi.org/10.1136/bmj.n1560)

### 🧬 Rule Logic:
- **Target Patient Population**:  
  Patients undergoing **adjuvant Temozolomide therapy** for ≥6 months post-surgery for glioblastoma.

- **Clinical Action**:  
  Trigger monthly alerts prompting the provider to:
  - Perform **complete blood count (CBC)** evaluations.
  - Monitor for **myelosuppression**, neutropenia, or thrombocytopenia.
  - Adjust Temozolomide dosage based on lab findings.

- **Purpose**:  
  Reduce risk of adverse effects, ensure treatment continuity, and personalize chemotherapy dosing for optimal efficacy and safety.

---

These rules were configured in OpenEMR using structured terminologies (ICD-10, SNOMED CT), and are part of a broader effort to integrate **real-time, evidence-based decision-making** into clinical workflows for personalized patient care.


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



