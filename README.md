# 🏥 HealthConnect Clinic: Appointment Attendance & No-Show Analysis

##  Project Overview

This project is part of my **HealthConnect Data Analytics Track** and focuses on understanding appointment attendance and no-show patterns.

The Week 4 stage focused on understanding the business problem, reviewing the dataset, assessing data quality, identifying relevant business questions and KPIs, and defining an initial analytical approach.

The overall objective is to identify factors associated with missed appointments and generate insights that can support improved appointment attendance and clinic operations.

![Initial Data Analysis Document](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/DAWODU%20FEHINTOLUWA%20TRACK%20SPECIFIC%20RESPONSE.docx)![Project Summary](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20Week%204%20Project%20summary.pptx)
---

## Problem Statement

HealthConnect Clinic is experiencing a high level of missed appointments, which can affect appointment-slot utilisation, clinic operations and patient access to care.

### Key Question

> **What factors are associated with patients attending, cancelling, or missing their scheduled appointments?**

---

## Dataset Overview

The HealthConnect Appointment Dataset contains:

* **5,000 appointment records**
* **1,696 unique patients**
* **18 variables**
* Patient demographic information
* Appointment characteristics
* Previous appointment history
* Reminder information
* Distance to clinic
* Waiting time
* Appointment outcomes

### Appointment Outcomes

| Outcome   |    Number | Percentage |
| --------- | --------: | ---------: |
| Attended  |     2,314 |     46.28% |
| No-Show   |     2,423 |     48.46% |
| Cancelled |       263 |      5.26% |
| **Total** | **5,000** |   **100%** |

---

##  Week 4 Key Observations

The initial review of the dataset revealed:

* **No-Show was the largest appointment outcome**, accounting for **48.46%** of appointments.
* **46.28%** of appointments were attended.
* **5.26%** of appointments were cancelled.
* Missing values were identified in **Distance to Clinic (90 records)**.
* **Waiting Time had 60 missing records**.
* The dataset contains both reminded and non-reminded appointments.
* Previous appointment and no-show history can be explored to determine whether previous behaviour is associated with future attendance.

These observations provide the foundation for the next stage of analysis.


---

## 📈 Proposed KPIs

| KPI                               | Business Question                                                            |
| --------------------------------- | ---------------------------------------------------------------------------- |
| **Appointment No-Show Rate**      | What proportion of appointments are missed?                                  |
| **Appointment Attendance Rate**   | What proportion of scheduled appointments are attended?                      |
| **Appointment Cancellation Rate** | What proportion of appointments are cancelled?                               |
| **Repeat No-Show Rate**           | Are patients with previous no-shows more likely to miss future appointments? |
| **Reminder Attendance Rate**      | Is attendance different when patients receive reminders?                     |

> **Note:** The KPIs were identified during Week 4. Detailed calculation, analysis and visualisation will be completed in subsequent stages.

---

## ❓ Business Questions

The analysis will explore:

* Does age influence appointment attendance?
* Does appointment type influence attendance?
* Does distance from the clinic affect attendance?
* Is previous no-show history associated with future no-shows?
* Does receiving a reminder influence attendance?
* Does the reminder channel influence attendance?
* Does booking lead time affect appointment compliance?
* Do appointment day and time influence attendance?

---

## Tools & Technologies

| Tool         | Purpose                                                         |
| ------------ | --------------------------------------------------------------- |
| **Excel**    | Initial data inspection, validation and data-quality assessment |
| **SQL**      | Data querying and exploration                                   |
| **Power BI** | Data modelling, DAX, KPI development and visualisation          |

### Resources

* HealthConnect Appointment Dataset
* HealthConnect Data Dictionary

---

##  Initial Analysis Approach

The proposed workflow is:

**Understand → Clean → Explore → Measure → Visualise → Recommend**

### 1. Data Quality Assessment

Review missing values, duplicates, data types, inconsistencies and potential outliers.

### 2. Data Cleaning & Transformation

Prepare the dataset for analysis while maintaining data integrity.

### 3. Exploratory Analysis

Investigate appointment outcomes across patient and appointment characteristics.

### 4. KPI Development

Calculate and compare the selected appointment KPIs.

### 5. Visualisation

Develop Power BI visuals to communicate important patterns.

### 6. Insights & Recommendations

Translate findings into evidence-based recommendations for improving appointment attendance.

---

## ⚠️ Key Considerations

### Data Limitations

* Missing or incomplete information may affect some analyses.
* The dataset may not capture all reasons for missed appointments.
* The dataset is fictional and may not fully represent real-world patient behaviour.

### Technical Considerations

* Data preparation must be consistent across Excel, SQL and Power BI.
* Variable definitions and appointment outcomes must be interpreted consistently.

### Project Risks

* Incorrect treatment of missing values may affect findings.
* Association between variables should not automatically be interpreted as causation.
* Reminder-related findings require careful interpretation.

### Ethical Considerations

* Avoid stigmatising patients based on attendance behaviour.
* Report findings at an appropriate aggregate level.
* Recommendations should focus on improving patient support and healthcare services.

---

## Week 5 Focus

The next stage will focus on:

* Data cleaning and transformation
* Investigation of identified missing values
* Exploratory data analysis
* KPI calculation
* Analysis of factors associated with appointment outcomes
* Initial Power BI visualisations

### Week 5 Goal

> **Move from understanding the data to identifying patterns and factors associated with missed appointments.**

---

## 📌 Project Status

**Current Stage:** Week 4 – Initial Analysis & Project Planning

**Next Stage:** Week 5 – Data Cleaning, Exploratory Analysis & KPI Development

---

## 💡 Key Takeaway

> **Good data analysis starts with understanding the problem and asking the right questions before building the dashboard.**

This project demonstrates how healthcare data analytics can be used to investigate operational challenges and generate evidence to support better patient-centred decision-making.
