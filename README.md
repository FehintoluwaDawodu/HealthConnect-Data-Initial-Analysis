# 🏥 HealthConnect Clinic: Appointment Attendance & No-Show Analysis

## Project Overview

This project is part of my **HealthConnect Data Analytics Track** and focuses on analysing appointment attendance, cancellations, and no-show patterns.

The project began in **Week 4** with an initial assessment of the business problem, dataset, data quality, business questions, potential KPIs, assumptions, limitations, risks, and dependencies.

In **Week 5**, the project progressed from initial planning to **data preparation, exploratory data analysis (EDA), KPI development, visualisation, business insights, and recommendations**.

The overall objective is to identify patterns and factors associated with missed appointments and generate insights that can support improved appointment attendance and clinic operations.

> **Important:** The analysis identifies associations and patterns; it does not establish causation.

---

##  Problem Statement

HealthConnect Clinic is experiencing a high level of missed appointments, which can affect appointment-slot utilisation, clinic operations, and patient access to care.

### Key Question

> **What factors are associated with patients attending, cancelling, or missing their scheduled appointments?**

---

#  Dataset Overview

The HealthConnect Appointment Dataset contains:

- **5,000 appointment records**
- **1,696 unique patients**
- **18 variables**
- Patient demographic information
- Appointment characteristics
- Previous appointment history
- Reminder information
- Distance to clinic
- Waiting time
- Appointment outcomes

### Appointment Outcomes

| Outcome | Number | Percentage |
|---|---:|---:|
| Attended | 2,314 | 46.28% |
| No-Show | 2,423 | 48.46% |
| Cancelled | 263 | 5.26% |
| **Total** | **5,000** | **100%** |

---

#  Week 4: Initial Analysis

The Week 4 analysis focused on understanding the HealthConnect business problem and preparing for exploratory analysis.

### Key Observations

- **No-Show was the largest appointment outcome**, accounting for **48.46%** of appointments.
- **46.28%** of appointments were attended.
- **5.26%** of appointments were cancelled.
- **90 records** had missing values for Distance to Clinic.
- **60 records** had missing values for Waiting Time.
- The dataset contained both reminded and non-reminded appointments.
- Previous appointment and no-show history could be explored to determine whether previous behaviour was associated with future attendance.
- Booking lead time was identified as a relevant factor for further investigation.

---

#  Week 5: Data Preparation

During Week 5, the dataset was prepared for exploratory analysis.

### Data Quality Checks

The following were reviewed:

- Data types
- Missing values
- Duplicate records
- Inconsistent values
- Relevant variables for analysis
- Potential extreme values

### Missing Values

Missing values were identified in:

- **Distance to Clinic:** 90 records
- **Waiting Time:** 60 records
- **Reminder Channel:** Blank values represented appointments where no reminder was sent.

Distance and waiting-time variables were reviewed for extreme values before missing values were addressed using **mean imputation** for the analysis.

The original dataset was not overwritten.

---

#  Week 5: Exploratory Data Analysis

The exploratory analysis investigated patterns in appointment attendance and no-shows across:

- Age groups
- Appointment type
- Reminder status
- Reminder channel
- Previous no-show history
- Booking lead time
- Distance to clinic
- Waiting time
- Appointment day
- Appointment characteristics

### Key EDA Findings

#### 1. No-Shows Represent a Major Operational Issue

No-shows accounted for **48.46%** of all appointments, making missed appointments the largest appointment outcome in the dataset.

This suggests that reducing missed appointments should be an important area of focus for HealthConnect.

#### 2. Attendance Was Below Half of Scheduled Appointments

Only **46.28%** of appointments were attended.

This highlights an opportunity to investigate factors associated with appointment attendance and improve appointment utilisation.

#### 3. Previous No-Show History

Patients with previous no-shows showed different patterns of future attendance.

This suggests that **previous no-show history may be an important variable for further analysis**.

#### 4. Reminder Patterns

Differences were observed in attendance patterns based on reminder status and reminder channel.

This suggests that reminder practices may warrant further investigation.

#### 5. Booking Lead Time

**Booking lead time showed a notable relationship with attendance rate** during the exploratory analysis.

This made booking lead time an important factor for further investigation and potential inclusion in future predictive analysis.

> These findings represent observed associations and should not be interpreted as proof that any factor directly causes a patient to miss an appointment.

---

# KPI Development

Three core KPIs were calculated during Week 5.

| KPI | Definition | Result |
|---|---|---:|
| **Appointment No-Show Rate** | No-show appointments ÷ total appointments × 100 | **48.46%** |
| **Appointment Attendance Rate** | Attended appointments ÷ total appointments × 100 | **46.28%** |
| **Appointment Cancellation Rate** | Cancelled appointments ÷ total appointments × 100 | **5.26%** |

### Why These KPIs Matter

**Appointment No-Show Rate**

Measures the proportion of scheduled appointments that are missed. It is important for understanding the scale of the clinic's missed-appointment problem.

**Appointment Attendance Rate**

Measures the proportion of scheduled appointments that are successfully attended and provides a direct view of appointment utilisation.

**Appointment Cancellation Rate**

Measures the proportion of appointments cancelled and helps distinguish planned cancellations from unplanned no-shows.

---

#  Power BI Dashboard

An initial analytical dashboard was developed in **Power BI** to communicate the main appointment patterns and KPIs.

### Dashboard Areas

The dashboard explores:

- Appointment outcomes
- Outcomes by age group
- Outcomes by gender
- Outcomes by appointment type
- Attendance by reminder channel
- Attendance rate by booking lead days
- No-show rate by previous no-shows
- Distance-related attendance patterns
-  Attendance rate by reminder sent


The dashboard provides an interactive view of appointment attendance and no-show patterns and supports further investigation of the identified factors.

---

#  Key Business Insights

The Week 5 analysis produced the following key insights:

### 1. No-shows are the largest appointment outcome

Almost half of scheduled appointments were missed, indicating that no-show reduction should be a major operational priority.

### 2. Attendance remains below 50%

With an attendance rate of **46.28%**, there is considerable opportunity to improve appointment utilisation.

### 3. Previous no-show history is associated with future attendance patterns

Patients with previous no-shows displayed different attendance patterns, suggesting that historical appointment behaviour may provide useful information for further analysis.

### 4. Reminder status/channel is associated with attendance patterns

Differences across reminder groups suggest that HealthConnect should further investigate reminder coverage and channel effectiveness.

### 5. Booking lead time is an important factor

Booking lead time showed a notable relationship with attendance rate and emerged as an important variable for further analysis.

---

#  Cross-Track Collaboration

## Data Analytics → Data Science

During Week 5, I interacted with the **Data Science track** to compare findings from the exploratory/KPI analysis with their baseline no-show prediction work.

I shared findings related to:

- Booking lead time
- Reminder status
- Previous no-show history
- Appointment attendance patterns

The Data Science track shared their initial modelling findings and discussed potential predictive features.

### Why This Was Relevant

The interaction helped connect **business-level analytics and KPIs with predictive modelling**.

### What Changed

Through the collaboration and comparison of findings, **booking lead time emerged as a major factor associated with attendance rate** and was highlighted as an important feature for further investigation and potential predictive modelling.

This demonstrated how Data Analytics findings can support feature selection and interpretation within a multidisciplinary HealthConnect project.

---

#  Assumptions, Limitations, Risks & Dependencies

## Assumptions

- The dataset represents appointment activity accurately within the fictional HealthConnect environment.
- The appointment outcome variable accurately represents attended, cancelled, and no-show appointments.
- Patient and appointment records can be analysed without exposing personally identifiable information.
- The available variables are sufficient for the initial exploratory analysis.

## Limitations

- The dataset is fictional and may not fully represent real-world patient behaviour.
- Some variables contain missing values.
- The dataset does not contain every factor that may influence appointment attendance.
- Mean imputation was used for selected missing values, meaning the imputed values are estimates rather than actual observations.
- The analysis identifies associations and patterns but does not establish causation.

## Risks

- Missing data may influence findings.
- Mean imputation may affect analyses involving distance and waiting time.
- Findings may be overgeneralised beyond the fictional dataset.
- Observed associations could be incorrectly interpreted as causal relationships.

## Dependencies

The analysis depends on:

- HealthConnect Appointment Dataset
- HealthConnect Data Dictionary
- Accurate understanding of appointment outcome definitions
- Consistent data preparation
- Accurate KPI calculations
- Power BI visualisation and analysis

### How These Issues Should Be Addressed

- Improve completeness of data collection.
- Document all data-cleaning and imputation steps.
- Validate important findings using additional data.
- Avoid causal claims when interpreting observational findings.
- Include additional variables that may explain appointment attendance.
- Continue monitoring the identified KPIs.

---

#  Business Recommendations

Based on the Week 5 findings, HealthConnect should consider:

### 1. Prioritise No-Show Reduction

Develop targeted strategies to reduce the high proportion of missed appointments.

### 2. Review Reminder Practices

Investigate reminder coverage and channel performance to determine how appointment reminders can better support attendance.

### 3. Monitor Previous No-Show Patterns

Use appointment history as an area for further analysis and consider targeted patient engagement strategies, while avoiding stigmatisation.

### 4. Investigate Booking Lead Time

Further examine how the timing between booking and appointment date relates to attendance and whether scheduling practices can be improved.

### 5. Improve Data Completeness

Strengthen the collection of distance, waiting time, and other potentially relevant variables to support more reliable analysis.

### 6. Continue KPI Monitoring

Regularly monitor:

- No-Show Rate
- Attendance Rate
- Cancellation Rate

to evaluate whether interventions lead to improvements over time.

---

#  Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Data inspection, validation and data-quality assessment |
| **SQL** | Data querying and exploration |
| **Power BI** | Data modelling, DAX, KPI development and visualisation |

### Resources

- HealthConnect Appointment Dataset
- HealthConnect Data Dictionary

---

#  Analytical Workflow

The project followed the workflow:

**Understand → Prepare → Explore → Measure → Visualise → Interpret → Recommend**

### Week 4
**Understand → Assess → Plan**

- Understand the business problem
- Review the dataset
- Assess data quality
- Develop business questions
- Identify potential KPIs
- Define the analytical approach

### Week 5
**Prepare → Explore → Measure → Visualise → Interpret**

- Prepare the dataset
- Conduct exploratory analysis
- Calculate KPIs
- Develop Power BI visualisations
- Identify business insights
- Develop recommendations
- Collaborate with the Data Science track

---

#  Project Status

**Current Stage:** Week 5 – Exploratory Analysis, KPI Development & Business Insights

### Completed

- [x] Business problem definition
- [x] Dataset review
- [x] Data-quality assessment
- [x] Data preparation
- [x] Exploratory data analysis
- [x] KPI calculation
- [x] Power BI dashboard development
- [x] Business insights
- [x] Recommendations
- [x] Limitations and risk assessment
- [x] Cross-track collaboration

### Next Focus

- Further investigate booking lead time
- Explore reminder effectiveness
- Analyse previous no-show patterns in greater depth
- Validate important findings with additional analysis
- Support further predictive modelling where appropriate

---

#  Project Documentation

### Week 4

[Initial Data Analysis Document](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/DAWODU%20FEHINTOLUWA%20TRACK%20SPECIFIC%20RESPONSE.docx)

[Week 4 Project Summary](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20Week%204%20Project%20summary.pptx)

### Week 5
![Week 5 Project Summary](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20Week%205%20Project%20summary.pptx)
![Week 5 Analytical Dashboard](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/HealthConnect%20Week%205.png)
[Week 5 Track-Specific Response](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20week%205%20Track%20Response.docx)

---

#  Key Takeaway

> **The Week 5 analysis showed that missed appointments are a major operational issue, while booking lead time, reminder patterns, and previous no-show history provide important areas for further investigation.**

The project demonstrates how healthcare data analytics can move from **data-quality assessment to exploratory analysis, KPI development, visualisation, and actionable insights** that can support evidence-based decision-making.
