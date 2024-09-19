# Data Driven Project Management

**Title:** Data Driven Project Management  
**Client:** Canada Revenue Agency
**Data Privacy:** Open-Source

## Abstract

Effective project management requires accurate cost estimation and tracking to ensure projects stay within budget and meet deadlines. However, discrepancies between estimated and actual project costs can lead to budget overruns, delays, and client dissatisfaction. This project focuses on developing machine learning models to predict monthly cost variances for Work Breakdown Structure (WBS) elements and creating visualizations to better understand the factors driving these variances.

## Problem Statement

The Canada Revenue Agency (CRA) faces challenges in predicting monthly cost variances for Work Breakdown Structure (WBS) elements in construction projects. Current methods of cost estimation often lead to significant discrepancies between projected and actual costs, resulting in:

- **Budget Overruns:** Financial strain and potential funding shortfalls.
- **Project Delays:** Increased time and resources required to manage budget issues.
- **Client Dissatisfaction:** Negative impact on client relationships and organizational reputation.
- **Resource Misallocation:** Inefficient use of resources leading to wasted expenditures.
- **Financial Instability:** Challenges in managing future projects and maintaining operational stability.

To address these challenges, there is a need for a more accurate method of forecasting cost variances using advanced analytical techniques.

## Proposed Solution

To improve the accuracy of cost variance predictions, the following solution is proposed:

1. **Data Integration and Preparation:**
   - Consolidate and preprocess the provided dataset to focus on relevant monthly cost data. Ensure data accuracy by cleaning and handling missing or non-contributing records.

2. **Development of Machine Learning Models:**
   - Apply various machine learning algorithms, including Linear Regression, Support Vector Machine (SVM), Decision Tree, and Random Forest Regression, to predict monthly cost variances.
   - Perform data preprocessing, including encoding categorical variables and managing class imbalances, to enhance model performance.

3. **Model Evaluation and Selection:**
   - Evaluate model performance using accuracy metrics within a 15% tolerance threshold. Select the best-performing model based on its ability to accurately predict cost variances.

4. **Data Visualization and Analysis:**
   - Create interactive visualizations in Power BI to explore and present insights from the machine learning models. Key visualizations include:
     - Comparison of actual vs. predicted costs.
     - Monthly cost predictions versus actual expenditures.
     - Analysis of top resources and WBS elements with significant cost variances.
     - Examination of cost variance in scenarios of work target exceedance or failure.

5. **Recommendations for Improvement:**
   - **Incorporate Additional Metrics:** Enhance model accuracy by including additional data such as team performance and project duration. These metrics can provide context and improve predictions.
   - **Enhance Data Granularity:** Integrate more detailed cost data or resource specifics to refine predictions and better understand cost drivers.

## Background

In project management, cost estimates often diverge significantly from actual expenditures due to factors such as inaccurate initial estimates, unforeseen scope changes, market fluctuations, and execution inefficiencies. These discrepancies can lead to:

- **Budget Overruns:** Additional financial strain and potential funding issues.
- **Project Delays:** Increased time and resources required to address budget issues.
- **Client Dissatisfaction:** Damaged relationships and a negative impact on organizational reputation.
- **Resource Misallocation:** Inefficient use of resources and wasted expenditures.
- **Financial Instability:** Challenges in managing future projects and maintaining operational stability.

Predictive models using machine learning can provide valuable insights into cost variances, helping organizations better manage and control project budgets.

## Data Source

The dataset used in this project is an open-source resource provided by the client, published by Brett Thiele, Michael Ryan, and Alireza Abbasia on the National Center for Biotechnology Information. The dataset is titled *Developing a dataset of real projects for portfolio, program, and project control management research.*

### Description of Projects

- **P01:** Construction of new carparks and access at a regional airport.
- **P02:** Construction of a lined landfill cell and leachate collection system in Queensland.
- **P03:** Widening and strengthening of a road for heavy vehicles.
- **P04:** Pavement rehabilitation along a 27 km section of road.
- **P05:** Road rehabilitation following the 2011 Queensland floods.
- **P06:** Reconstruction of urban streets post-floods.
- **P017:** Marina subdivision (details not provided).
- **P018:** Rural road repairs (details not provided).

### Data Characteristics

**Portfolio WBS Worksheet Columns:**

- **Portfolio WBS:** Name of WBS element.
- **Description:** Description of the WBS element.
- **Quantity:** Planned quantity of work.
- **UOM:** Unit of measurement.
- **BAC:** Budget at Completion for the WBS element.
- **BAC Rate:** Rate at which the budget should increase.
- **Final Qty:** Actual quantity of work completed.
- **Final Cost:** Total cost of WBS elements.
- **Final Rate:** Rate at which the budget increased based on actual quantity.
- **PQ:** Planned Quantity of work each month.
- **PV:** Planned Value for a WBS element each month.
- **AQ:** Actual Quantity of work completed each month.
- **AC:** Actual Cost for a WBS element each month.
- **EV:** Earned Value based on Actual Quantity.

**Actual Cost Worksheet Columns:**

- **Date:** Date of expenditure.
- **Description:** Invoice number and description of resource.
- **Resource:** Name of resource.
- **Unit:** Unit of measurement.
- **Quantity:** Quantity of resource.
- **Rate:** Cost per unit of resource.
- **Total:** Total cost of resource expenditure.
- **Portfolio WBS:** WBS element associated with the resource.

## Executive Summary

- Integrated and reformatted data from 8 construction projects for monthly cost prediction.
- Refined the dataset by removing records with missing key metrics and non-contributing entries.
- Applied machine learning models, including Linear Regression, Support Vector Machine (SVM), Decision Tree, and Random Forest Regression.
- SVM emerged as the best-performing model with an accuracy of 24.64% within a 15% tolerance.
- Developed data warehouse bus architecture in Power BI for improved report performance and & reporting.
- Proposed recommendations & solutions to enhance developed models. 

## Features Used for Machine Learning Models

- **Independent Features:** Quantity, BAC, BAC Rate, Planned Quantity, Planned Value, Portfolio WBS, UOM, Month.
- **Dependent Feature:** Actual Cost.

**Feature Correlations:** BAC and Planned Value exhibit a strong positive correlation with the target variable (Actual Cost).

## Machine Learning Models used

- **Linear Regression**
- **Support Vector Machine (SVM)**
- **Decision Tree**
- **Random Forest Regression**

The SVM model provided the highest accuracy within a 15% tolerance, achieving 24.64% accuracy.

## Analysis & Explanations

- Visualizations in Power BI were used to support solutions and analysis.
## References

- [Dataset on National Center for Biotechnology Information](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7770534/)
- [Figshare Dataset](https://figshare.com/articles/dataset/Project_Portfolio_Dataset/12998822?file=24779921)
- Thiele B, Ryan M, Abbasi A. *Developing a dataset of real projects for portfolio, program, and project control management research*. Data Brief. 2020 Dec 17;34:106659. doi: 10.1016/j.dib.2020.106659. PMID: 33385027; PMCID: PMC7770534. [Accessed July 21, 2024]
