#  HealthConnect Clinic: Appointment Attendance & No-Show Analysis

## Project Overview

This project is part of the **HealthConnect Data Analytics Track** within the **AnalystLab Africa Experience Lab Internship Programme**.

The project focuses on analysing appointment attendance, cancellations, and no-show patterns to identify factors associated with missed appointments and generate insights that can support improved appointment attendance and clinic operations.

### Project Progression

- **Week 4:** Problem Understanding & Solution Planning
- **Week 5:** Exploratory Analysis, KPI Development & Initial Implementation
- **Week 6:** Advanced Analysis, Integration & Validation
- **Week 7:** Testing, Refinement & End-to-End Validation
- **Week 8:** Final Integration & Presentation

> **Important:** The analysis identifies patterns and associations. It does not establish causation.

---

#  Problem Statement

HealthConnect Clinic is experiencing a high level of missed appointments, which may affect appointment-slot utilisation, clinic operations, and patient access to care.

### Key Question

> What factors are associated with patients attending, cancelling, or missing their scheduled appointments, and how can these insights support better appointment management?

---

#  Dataset Overview

The HealthConnect Appointment Dataset contains:

- **5,000 appointment records**
- **1,696 unique patients**
- Patient characteristics
- Appointment characteristics
- Previous appointment history
- Previous no-show history
- Reminder information
- Booking lead time
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

#  Week 4 — Initial Analysis

### Focus

- Understand the business problem
- Review available resources
- Assess dataset quality
- Define business questions
- Identify potential KPIs
- Develop the initial analytical approach

### Key Observations

- No-Show was the largest appointment outcome.
- Attendance was below 50%.
- Distance and waiting-time variables contained missing values.
- Previous no-show history was identified for further investigation.
- Booking lead time was identified as a relevant factor for further analysis.

### Deliverables

- [Week 4 Track-Specific Response](INSERT_LINK)
- [Week 4 Project Summary](INSERT_LINK)

---

#  Week 5 — Exploratory Analysis & KPI Development

### Focus

- Data preparation
- Data-quality assessment
- Exploratory data analysis
- KPI development
- Power BI visualisation
- Business insights
- Initial recommendations

### Data Preparation

Reviewed:

- Data types
- Missing values
- Duplicate records
- Inconsistent values
- Potential extreme values
- Relevant analytical variables

### Missing Values

| Variable | Missing Records |
|---|---:|
| Distance to Clinic | 90 |
| Waiting Time | 60 |
| Reminder Channel | 1,366* |

\*Blank reminder-channel values represented appointments where no reminder was sent.

### Week 5 KPIs

| KPI | Result |
|---|---:|
| Appointment No-Show Rate | **48.46%** |
| Appointment Attendance Rate | **46.28%** |
| Appointment Cancellation Rate | **5.26%** |

### Key Findings

- No-shows represented the largest appointment outcome.
- Attendance remained below 50%.
- Previous no-show history showed an important pattern.
- Reminder status/channel showed differences in attendance patterns.
- Booking lead time showed a notable relationship with attendance.

### Deliverables

- [Week 5 Track-Specific Response](INSERT_LINK)
- [Week 5 Project Summary](INSERT_LINK)
- [Week 5 Dashboard](INSERT_LINK)

---

#  Week 6 — Advanced Analysis, Integration & Validation

### Focus

Week 6 built on the Week 5 analysis by moving from initial exploration to **advanced analysis, validation, dashboard improvement, and cross-track integration**.

### Objectives

- Investigate important Week 5 findings in greater depth
- Validate key KPIs
- Analyse relevant segments
- Refine previous conclusions
- Improve the Power BI dashboard
- Translate findings into decision-support actions
- Integrate Data Analytics findings with Data Science modelling

---

##  Advanced Analysis

### Previous No-Show History

| Previous No-Shows | No-Show Rate |
|---:|---:|
| 0 | ~46.3% |
| 1 | ~55.9% |
| 2 | ~62.1% |
| 3 | ~69.7% |

### Reminder Status

| Reminder Status | No-Show Rate |
|---|---:|
| No Reminder | ~54.6% |
| Reminder Sent | ~49.9% |

### Reminder Pattern by Appointment Type

Diagnostic Tests showed the largest observed difference:

- **~61.1% no-show** without reminders
- **~49.3% no-show** when reminders were sent

### Booking Lead Time

Further analysis showed that attendance decreased as booking lead days increased, while the no-show pattern moved in the opposite direction.

This made booking lead time an important candidate feature for further investigation and predictive modelling.

> These findings represent observed associations and should not be interpreted as causal relationships.

---

#  KPI Validation

The Week 5 KPIs were reviewed during Week 6.

| KPI | Week 5 | Week 6 |
|---|---:|---|
| No-Show Rate | 48.46% | ✅ Validated |
| Attendance Rate | 46.28% | ✅ Validated |
| Cancellation Rate | 5.26% | ✅ Validated |

---

#  Dashboard Improvement

The Power BI dashboard was improved to provide greater decision-support value.

### Improvements

- Improved KPI presentation
- Clearer attendance/no-show rate visuals
- Grouped booking lead-time categories
- Improved previous no-show visualisation
- Improved reminder-status labels
- Additional distance/waiting-time analysis
- Improved chart titles and sorting
- Greater emphasis on high-impact findings
- Removal of less useful raw tables

### Decision-Support Focus

The improved dashboard aims to answer:

> **Which patterns are most important, have they remained meaningful after deeper analysis, and what should HealthConnect do about them?**

---

#  Cross-Track Integration

## Data Analytics → Data Science

During Week 6, the Data Analytics findings were integrated with the **Data Science track's predictive modelling work**.

### Data Analytics Contribution

Shared findings related to:

- Booking lead time
- Previous no-show history
- Reminder status
- Reminder patterns by appointment type
- Attendance patterns

### Data Science Contribution

The Data Science track compared:

- Logistic Regression
- Random Forest
- Gradient Boosting

### Model Improvement

Gradient Boosting produced the strongest overall performance:

| Metric | Result |
|---|---:|
| Accuracy | ~65% |
| No-Show Recall | ~65% |
| F1-Score | ~65% |
| ROC-AUC | 0.68 |

The improvement over Logistic Regression was modest.

### Integration Impact

The collaboration strengthened the focus on:

- Previous no-show history
- Booking lead time
- Reminder-related variables

as candidate features for further predictive analysis.

This connected:

**Data Analytics → Analytical Findings → Predictive Modelling → Decision Support**

---

#  Key Business Insights

### 1. No-shows remain a major operational issue

Almost half of scheduled appointments were missed.

### 2. Previous no-show history is an important signal

No-show rates increased as previous no-show history increased.

### 3. Booking lead time requires further investigation

Longer booking lead times were associated with lower attendance in the analysed data.

### 4. Reminder patterns warrant further investigation

Reminder status was associated with differences in no-show rates, with variation across appointment types.

### 5. Some variables were less informative

Age group and appointment day did not show sufficiently meaningful differences to become major decision drivers in the current analysis.

---

#  Recommendations

Based on the analysis, HealthConnect should consider:

1. **Prioritising no-show reduction**
2. **Investigating previous no-show patterns**
3. **Reviewing booking lead-time patterns**
4. **Evaluating reminder coverage and channels**
5. **Improving data completeness**
6. **Continuing KPI monitoring**
7. **Further evaluating predictive modelling approaches**

---

#  Assumptions & Limitations

### Assumptions

- The dataset represents appointment activity accurately within the fictional HealthConnect environment.
- Appointment outcomes are correctly defined.
- Available variables are sufficient for the current analysis.
- No personally identifiable information is required for the analysis.

### Limitations

- The dataset is fictional.
- Some potentially important variables are unavailable.
- Distance and waiting-time variables contain missing values.
- Mean imputation was used for selected missing values.
- Imputed values are estimates rather than observed values.
- Associations do not establish causation.
- Predictive model performance remains moderate.

### Risks

- Missing data may influence findings.
- Imputation may affect distance/waiting-time analysis.
- Associations may be incorrectly interpreted as causal.
- Model performance may not generalise beyond the current dataset.

---

#  Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Data inspection and preparation |
| **SQL** | Data querying and exploration |
| **Power BI** | Data modelling, DAX, KPI development and dashboarding |
| **Python** | Predictive modelling through cross-track Data Science work |

---

#  Project Workflow

```text
Understand
    ↓
Prepare
    ↓
Explore
    ↓
Measure
    ↓
Visualise
    ↓
Analyse Further
    ↓
Validate
    ↓
Integrate
    ↓
Recommend
    ↓
Test & Refine
````

---

#  Project Status

### Completed

* [x] Business problem definition
* [x] Dataset review
* [x] Data-quality assessment
* [x] Data preparation
* [x] Exploratory data analysis
* [x] KPI development
* [x] Power BI dashboard development
* [x] Business insights
* [x] Recommendations
* [x] Advanced Week 6 analysis
* [x] KPI validation
* [x] Dashboard improvement
* [x] Data Science cross-track integration
* [x] Model comparison findings
* [x] Review and refinement of Week 5 conclusions

### Next Focus — Week 7

* [ ] Test analytical findings
* [ ] Further validate important relationships
* [ ] Test predictive-model outputs
* [ ] Conduct error analysis
* [ ] Validate dashboard calculations
* [ ] Refine recommendations
* [ ] Conduct end-to-end validation

---

#  Project Documentation

## Week 4

### Week 4

[Initial Data Analysis Document](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/DAWODU%20FEHINTOLUWA%20TRACK%20SPECIFIC%20RESPONSE.docx)

[Week 4 Project Summary](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20Week%204%20Project%20summary.pptx)

### Week 5
* ![Week 5 Project Summary](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20Week%205%20Project%20summary.pptx)
* ![Week 5 Analytical Dashboard](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/HealthConnect%20Week%205.png)
* ![Week 5 Track-Specific Response](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20week%205%20Track%20Response.docx)

---
## Week 6

* ![Week 6 Track-Specific Response](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20Week%206%20Track%20response.docx)
* ![Week 6 Project Summary](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Dawodu%20Fehintoluwa%20B%20Week%206%20summary.pptx)
* ![Updated Power BI Dashboard]((https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Healthconnect%20week%206.pbix))
* ![Dashboard](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Week%206.png)
* ![Cross-Track Integration Evidence](https://github.com/FehintoluwaDawodu/HealthConnect-Data-Initial-Analysis/blob/main/Progress%20from%20cross%20track%20integration.png)

---

#  Project Progression

| Week       | Focus                            | Key Output                                                                        |
| ---------- | -------------------------------- | --------------------------------------------------------------------------------- |
| **Week 4** | Problem Understanding & Planning | Business questions, KPIs and analytical approach                                  |
| **Week 5** | EDA & Initial Development        | KPIs, dashboard, insights and recommendations                                     |
| **Week 6** | Integration & Validation         | Advanced analysis, validated KPIs, improved dashboard and cross-track integration |
| **Week 7** | Testing & Refinement             | Analytical/predictive testing and validation                                      |
| **Week 8** | Final Integration                | Final solution and presentation                                                   |

---

#  Key Takeaway

> **The HealthConnect project demonstrates how healthcare data can move from data-quality assessment and exploratory analysis to KPI development, advanced analysis, validation, predictive modelling integration, and evidence-based decision support.**

The Week 6 work strengthened the evidence around **previous no-show history, booking lead time, and reminder patterns**, while refining less meaningful findings and improving the dashboard for decision support.

---
#  HealthConnect Clinic: Appointment Attendance & No-Show Analysis Week 7 Update

## Project Overview

This project is part of my **HealthConnect Data Analytics Track** and focuses on analysing appointment attendance, cancellations, and no-show patterns.

The project progressed from **business problem definition and data-quality assessment in Week 4**, to **exploratory analysis and KPI development in Week 5**, and then to **analytical testing, KPI validation, dashboard refinement, and cross-track collaboration in Week 7**.
---


#  Week 7 — Analytical Testing & Validation

Week 7 focused on testing whether the Week 5/6 findings remained supported and connecting the Data Analytics findings with Data Science modelling.

### Week 7 Objectives

* Validate core KPIs.
* Retest important analytical findings.
* Compare Power BI, Excel and SQL results.
* Validate booking lead-time patterns.
* Investigate previous no-show history.
* Refine the Power BI dashboard.
* Integrate relevant Data Science findings.

---

#  KPI Validation

Power BI and Excel produced consistent results for the core KPIs:

| KPI               |     Result |
| ----------------- | ---------: |
| Attendance Rate   | **46.28%** |
| No-Show Rate      | **48.46%** |
| Cancellation Rate |  **5.26%** |

A difference was identified during the SQL cross-check and requires **denominator/query reconciliation** before the SQL result can be considered fully validated.

### Validation Approach

**Recheck → Reconcile → Document → Retest**

---

#  Previous No-Show Analysis

Week 7 further examined the relationship between previous no-show history and subsequent no-show rates.

| Previous No-Shows | No-Show Rate |
| ----------------: | -----------: |
|                 0 |        46.3% |
|                 1 |        55.9% |
|                 2 |        62.1% |
|                 3 |        68.4% |
|                 4 |        66.7% |
|                 5 |        100% |

### Observation

> **No-show rate increased as previous no-show history increased.**

This makes previous appointment behaviour an important variable for continued analysis and potential predictive modelling.

---

#  Booking Lead-Time Analysis

Data Science requested validation of the underlying no-show rates for two booking lead-time groups.

| Booking Lead Time | No-Show Rate |
| ----------------- | -----------: |
| **≤30 days**      |   **36.59%** |
| **>30 days**      |   **60.31%** |

### Finding

Appointments booked more than 30 days ahead had a higher observed no-show rate than appointments booked within 30 days.

This provided an underlying-data check for the pattern identified during the Data Science modelling work.

> **No-show rate and model recall are different measures.** No-show rate describes the underlying appointment data, while recall measures how well a predictive model identifies no-shows.

---

#  Cross-Track Collaboration — Data Science

The Data Analytics track collaborated with the **Data Science track** to compare descriptive findings with predictive modelling results.

### Information Received

The Data Science track reported:

* **Previous no-show history:** 78% recall for patients with previous no-shows vs 58% without.
* **Booking lead time:** 94% recall for appointments booked >30 days ahead vs 23% for ≤30 days.
* **Diagnostic Tests:** 80% recall.
* **Specialist Consultations:** 53% recall.
* **Tuned Gradient Boosting:** AUC **0.72**, recall **67%**, F1 **67%**.

### Information Provided

Data Analytics provided the underlying booking lead-time no-show rates:

* ≤30 days → **36.59%**
* > 30 days → **60.31%**

### Why the Collaboration Was Relevant

The collaboration helped distinguish:

**Descriptive analysis**
→ What patterns exist in the appointment data?

from

**Predictive modelling**
→ How well can a model identify future no-shows?

### Integration Outcome

The booking lead-time analysis provided evidence from the underlying data that could be compared with the Data Science model's performance across the same segments.

---

#  Data Analytics vs Data Science

| Data Analytics                    | Data Science                                                      |
| --------------------------------- | ----------------------------------------------------------------- |
| Identified descriptive patterns   | Tested predictive performance                                     |
| Analysed booking lead time        | Compared model recall across lead-time groups                     |
| Examined previous no-show history | Tested predictive performance among patients with/without history |
| Analysed appointment types        | Compared recall across appointment types                          |
| Validated underlying rates        | Evaluated model performance                                       |

> **Data Analytics identified important patterns; Data Science tested their predictive usefulness.**

---

#  Power BI Dashboard

The Power BI dashboard was refined to provide a clearer view of:

* Appointment KPIs
* Appointment outcomes
* Previous no-show history
* Booking lead time
* Reminder patterns
* Appointment type
* Attendance and no-show patterns

The dashboard supports interactive exploration of the factors identified during the analysis.

---

#  Key Week 7 Insights

### 1. Previous No-Show History

No-show rates increased as previous no-show history increased.

### 2. Booking Lead Time

Appointments booked **>30 days ahead had a 60.31% no-show rate**, compared with **36.59% for ≤30 days**.

### 3. Data Science Validation

The Data Science model also showed substantial differences in recall across booking lead-time groups.

### 4. Model Performance Varies by Appointment Group

Model recall differed between Diagnostic Tests and Specialist Consultations.

### 5. KPI Validation Requires Consistency Across Tools

Power BI and Excel were aligned, while the SQL result requires further reconciliation.

---

#  Assumptions, Limitations & Risks

### Limitations

* The dataset is fictional.
* Some variables contain missing values.
* Reasons for missed appointments are not fully captured.
* Available variables may not represent every factor influencing attendance.
* Some findings require additional validation.
* Associations should not be interpreted as causal relationships.

### Technical Risk

Different SQL and Power BI/Excel calculations may produce different results if denominators or filtering logic are inconsistent.

### Response

**Recheck → Reconcile → Document → Retest**

---

#  Business Implications

The findings suggest areas HealthConnect could investigate further:

* Monitor patients with previous no-show history.
* Investigate appointment scheduling patterns and booking lead time.
* Review reminder strategies.
* Examine appointment-type differences.
* Improve data completeness.
* Use validated KPIs to monitor appointment performance.

Any intervention should be evaluated carefully rather than assuming that an observed association represents a causal effect.

---

#  Tools & Technologies

| Tool                      | Purpose                                                           |
| ------------------------- | ----------------------------------------------------------------- |
| **Excel**                 | Data inspection, validation and KPI cross-checking                |
| **SQL / MySQL Workbench** | Data querying and analytical validation                           |
| **Power BI**              | Data modelling, DAX, KPI development, dashboard and visualisation |

### Resources

* HealthConnect Appointment Dataset
* HealthConnect Data Dictionary
* Data Science model outputs
* Power BI analytical dashboard

---

#  Project Progression

### Week 4

**Understand → Assess → Plan**

Business problem, data quality, business questions, KPIs and analytical approach.

### Week 5

**Prepare → Explore → Measure → Visualise**

Data preparation, EDA, KPI development, dashboard and business insights.

### Week 7

**Test → Validate → Collaborate → Refine**

KPI validation, deeper analysis, SQL cross-checking, Data Science collaboration and dashboard refinement.

---

#  Current Project Status

### Completed

* [x] Business problem definition
* [x] Dataset and data-quality assessment
* [x] Data preparation
* [x] Exploratory data analysis
* [x] KPI development
* [x] Power BI dashboard
* [x] Previous no-show analysis
* [x] Booking lead-time analysis
* [x] KPI cross-checking
* [x] Data Science collaboration
* [x] Cross-track validation
* [x] Limitations and risks review

### Next Steps

* [ ] Reconcile SQL and Power BI/Excel KPI calculations
* [ ] Continue testing booking lead time
* [ ] Further investigate previous no-show history
* [ ] Refine dashboard based on validated findings
* [ ] Integrate relevant predictive-model outputs
* [ ] Document final analytical conclusions

---

#  Key Takeaway

> **Week 7 moved the HealthConnect project from identifying patterns to testing, validating and integrating findings across descriptive and predictive analysis.**

The analysis shows that **previous no-show history and booking lead time are important areas for further investigation**, while collaboration with Data Science helped connect descriptive healthcare analytics with predictive modelling.

##  About Me

**Dawodu Fehintoluwa Bukola**
Health Data Analyst | Public Health & Healthcare Analytics

**Skills:** Excel | Power BI | SQL | Python | Healthcare Analytics | Data Visualisation

```





