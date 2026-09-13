# 🏥 Hospital Performance & Quality Analytics

## 📊 Power BI Capstone Project

An interactive **Power BI dashboard** designed to analyze hospital performance and quality measures across the United States. The project transforms hospital-level data into meaningful insights around **overall ratings, mortality, safety, readmissions, geographic performance, hospital characteristics, and improvement scenarios**.

The dashboard helps users understand where hospital performance is strong, identify areas of variation, and explore how targeted improvements could influence overall performance.

## 🎯 Project Objectives

The main objectives of this project are to:

* Analyze overall hospital performance and quality ratings.
* Identify performance differences across states.
* Evaluate hospital quality across **Mortality, Safety, and Readmissions** domains.
* Compare hospital-level performance against national benchmarks.
* Provide interactive hospital-level drill-down analysis.
* Identify areas requiring quality improvement.
* Use What-If parameters to model potential improvement scenarios.
* Convert healthcare data into actionable, data-driven insights.

## 📁 Dataset Overview

The project uses a **Hospital General Information dataset** containing information about hospitals, their characteristics, ownership, location, ratings, and quality measures.

### Dataset Snapshot

| Metric               |                           Value |
| -------------------- | ------------------------------: |
| Total Hospitals      |                           5,384 |
| Hospital Types       |                               6 |
| Ownership Categories |                              12 |
| Quality Domains      |                               3 |
| Quality Domains      | Mortality, Safety, Readmissions |
| Overall Rating Scale |                       1–5 Stars |

The dataset includes fields related to:

* Hospital demographics
* Hospital type
* Hospital ownership
* State and geographic information
* Emergency service availability
* Birthing-friendly designation
* Overall hospital rating
* Mortality measures
* Safety measures
* Readmission measures
* Patient experience measures
* Timely and effective care measures

## 🛠️ Tools & Technologies

* **Power BI**
* **Power Query**
* **DAX**
* **Microsoft Excel / CSV**
* **Data Modeling**
* **Star Schema**
* **What-If Parameters**
* **Data Visualization**
* **Business Intelligence**

## 🏗️ Project Architecture

The project follows a structured **data modeling and BI approach**:

```text
Raw Hospital Dataset
        ↓
Data Cleaning & Transformation
        ↓
Power Query
        ↓
Data Modeling
        ↓
Star Schema
        ↓
DAX Measures & Calculations
        ↓
Interactive Power BI Dashboard
        ↓
Insights & What-If Analysis

The model is designed around a central **Hospital** table supported by dimensional tables such as:

* State
* County
* Hospital Type
* Hospital Ownership

This structure improves filtering, analysis, and maintainability of the Power BI model.

# 📄 Dashboard Pages

## 1. Project Overview

Provides an introduction to the project, dataset, objectives, and analytical scope.

### Key Focus

* Project objectives
* Dataset overview
* Hospital coverage
* Quality domains
* Analytical approach

## 2. Executive Overview

Provides a high-level view of hospital performance across the dataset.

### Key KPIs

* **Total Hospitals:** 5,384
* **Average Hospital Rating:** 3.14 / 5
* **High-Performing Hospitals:** 21.1%
* **Birthing-Friendly Hospitals:** 41.4%

### Rating Distribution

The dashboard analyzes hospitals across:

* ⭐ 1 Star
* ⭐⭐ 2 Stars
* ⭐⭐⭐ 3 Stars
* ⭐⭐⭐⭐ 4 Stars
* ⭐⭐⭐⭐⭐ 5 Stars

The analysis shows that **3-star hospitals form the largest rating group**, while 4-star and 5-star hospitals represent a significant portion of high-performing facilities.

## 3. Geographic Analysis

This page analyzes hospital performance across different states.

### Key Analysis

* Average hospital rating by state
* State-level performance comparison
* Top-performing states
* Hospital distribution across geographic areas

### Top States by Average Rating

| Rank | State        | Average Rating |
| ---: | ------------ | -------------: |
|    1 | Utah         |           4.29 |
|    2 | South Dakota |           4.23 |
|    3 | Colorado     |           4.02 |
|    4 | Minnesota    |           3.95 |
|    5 | Wisconsin    |           3.89 |
|    6 | Idaho        |           3.88 |
|    7 | Montana      |           3.81 |
|    8 | Ohio         |           3.61 |
|    9 | Delaware     |           3.57 |
|   10 | Nebraska     |           3.56 |

This geographic analysis helps identify high-performing states that can potentially serve as benchmarks for other regions.

## 4. Performance Measure Details

This page evaluates hospital performance across three major quality domains:

### 🩺 Mortality

Measures related to hospital mortality and death-rate performance.

* **Better:** 4%
* **No Different:** 94%
* **Worse:** 2%

The majority of mortality measures show no significant difference from the benchmark.

### 🛡️ Safety

Measures related to patient safety and complications.

* **Better:** 17%
* **No Different:** 80%
* **Worse:** 3%

Safety has the highest percentage of measures performing better than the benchmark.

### 🔄 Readmissions

Measures related to patients returning to the hospital, including 30-day readmission performance.

* **Better:** 5%
* **No Different:** 87%
* **Worse:** 8%

Readmissions have the highest percentage of measures performing worse than the benchmark, making them an important area for improvement.

# 🏥 5. Hospital Details

The Hospital Details page provides an interactive drill-down into an individual hospital.

Users can select a hospital from the dataset and view:

* Hospital name
* Overall star rating
* Hospital type
* State
* Mortality performance
* Safety performance
* Readmission performance

The selected hospital can be compared with national benchmarks to understand its relative performance.

# 🎛️ 6. Scenario Insights — What-If Analysis

The Scenario Insights page allows users to simulate potential improvement scenarios.

Two interactive parameters are used:

### Rating Threshold

Allows users to define the star rating considered **high-performing**.

### Measure Improvement %

Allows users to simulate an improvement in hospital performance measures.

These parameters dynamically affect the scenario outputs.

### Key Scenario Outputs

#### Projected High-Performing Hospitals

Estimates the number of hospitals that could reach the selected performance threshold under the improvement scenario.

#### Projected Safety Performance

Shows how safety performance could change as the improvement percentage increases.

#### Rating vs. Worse Readmissions

A scatter analysis comparing hospital ratings with worse-than-expected readmission measures to help identify potential outliers.

# 📐 DAX & Analytical Measures

DAX was used to create reusable measures and calculated outputs for the dashboard.

Key measures include:

* Total Hospitals
* Average Hospital Rating
* % High-Performing Hospitals
* % Birthing-Friendly Hospitals
* Mortality Status %
* Safety % by Status
* Readmission % by Status
* Readmission % Worse
* Average Better % for Safety & Readmissions
* Projected High-Performing Hospitals
* Projected Safety % Better
* Hospital Type Display
* State Display

The measures support dynamic filtering, KPI calculations, benchmark comparisons, and What-If scenario analysis.

# 📊 Key Insights

### 1. Overall Hospital Performance

The national average hospital rating is **3.14 out of 5**, indicating generally moderate performance with meaningful variation between hospitals.

### 2. Rating Distribution

3-star hospitals represent the largest rating group, while a smaller but important group of hospitals achieves 1-star ratings and requires closer attention.

### 3. Geographic Variation

Hospital performance varies significantly by state. **Utah and South Dakota** are among the strongest-performing states based on average hospital rating.

### 4. Safety Performance

Safety measures have the strongest "Better" performance share at **17%**, indicating comparatively stronger performance against the benchmark.

### 5. Readmission Opportunity

Readmissions have the highest "Worse" share at **8%**, highlighting readmission reduction as an important improvement opportunity.

### 6. Mortality Stability

Approximately **94% of mortality measures** show no significant difference from the benchmark, indicating relatively stable mortality performance.

### 7. Scenario-Based Decision Making

The What-If analysis allows users to explore how different improvement assumptions could influence the number of high-performing hospitals and safety outcomes.

# 💡 Business Recommendations

Based on the analysis, the following actions can be considered:

### Improve Readmission Performance

Hospitals with higher-than-expected readmission measures should be prioritized for targeted interventions.

### Benchmark High-Performing States

States with stronger average hospital ratings can be studied to identify practices and operational approaches that could be replicated elsewhere.

### Strengthen Patient Safety

Hospitals can focus on reducing complications and improving safety measures where performance is below benchmark.

### Monitor Low-Rated Hospitals

1-star and 2-star hospitals can be prioritized for deeper investigation and targeted improvement programs.

### Use Scenario Planning

Healthcare leadership can use the What-If analysis to evaluate potential improvement targets before allocating resources.

# 🎨 Dashboard Features

The Power BI dashboard includes:

* Interactive KPI cards
* Rating distribution analysis
* State-level analysis
* Quality-domain comparisons
* Hospital-level drill-down
* Interactive slicers
* Dynamic DAX measures
* National benchmark comparisons
* What-If parameters
* Scenario analysis
* Interactive visualizations

# 👥 Project Team

| Member           | Responsibility                         |
| ---------------- | -------------------------------------- |
| Annapoorna Madhu | Data Model & Core DAX                  |
| Anusha Bhagvath  | Data Cleaning & Power Query            |
| Sajal Srivastava | What-If Analysis & Scenario Modeling   |
| Srikanth K.      | Dashboard, UX, Testing & Documentation |

# 👤 My Contribution

### Data Modeling & Core DAX

My primary responsibility in the project was **Data Modeling and Core DAX development**.

I worked on:

* Designing the Power BI data model.
* Structuring the Hospital fact/main table.
* Creating supporting dimension tables.
* Establishing relationships between tables.
* Implementing the Star Schema.
* Developing core DAX measures.
* Creating KPI calculations.
* Developing hospital performance calculations.
* Supporting benchmark-based analysis.
* Creating measures used in dashboard visualizations.
* Supporting dynamic calculations used throughout the report.

This work provided the analytical foundation for the dashboard and enabled the other project components to interact dynamically with the underlying hospital data.

# 📈 Skills Demonstrated

Through this project, the following skills were applied:

### Technical Skills

* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Transformation
* Data Modeling
* Star Schema
* What-If Parameters
* Interactive Dashboard Development

### Analytical Skills

* Exploratory Data Analysis
* KPI Development
* Benchmark Analysis
* Geographic Analysis
* Healthcare Quality Analysis
* Scenario Analysis
* Insight Generation
* Data-Driven Recommendations

### Business Intelligence Skills

* Dashboard Design
* Interactive Reporting
* Drill-Down Analysis
* Decision Support
* Performance Monitoring
* Data Storytelling

# 🚀 Project Outcome

The final dashboard converts a large hospital dataset into an interactive business intelligence solution that enables users to:
Explore Hospital Performance
          ↓
Compare Quality Measures
          ↓
Identify Geographic Variation
          ↓
Find Improvement Opportunities
          ↓
Model Improvement Scenarios
          ↓
Support Data-Driven Decisions

The project demonstrates how **Power BI, DAX, data modeling, and interactive analytics** can be combined to transform complex healthcare data into actionable insights.

## 🔗 Project Highlights

**Domain:** Healthcare Analytics
**Project Type:** Business Intelligence / Data Analytics
**Tool:** Microsoft Power BI
**Dataset:** Hospital General Information
**Hospitals Analyzed:** 5,384
**Quality Domains:** Mortality, Safety & Readmissions
**Core Techniques:** Power Query, DAX, Data Modeling, Star Schema, What-If Analysis

## ⭐ Conclusion

**Hospital Performance & Quality Analytics** demonstrates how healthcare data can be transformed into a practical analytical solution for monitoring hospital quality, identifying performance gaps, comparing geographic patterns, and evaluating potential improvement scenarios.

The project combines **data preparation, dimensional modeling, DAX, interactive visualization, and scenario analysis** to provide a comprehensive view of hospital performance and quality.


### 📌 Author

**Annapoorna Madhu**

Data Analytics | Power BI | SQL | Python | Business Intelligence
