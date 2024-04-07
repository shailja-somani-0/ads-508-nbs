# ADS-508 Team Project
# Health Equity Analytics: Enhancing Healthcare Crisis Response

## Overview

Health Equity Analytics is a small non-profit organization dedicated to partnering with hospitals, insurance payors, and public health organizations to improve the allocation of staff and supplies during healthcare crises, such as the COVID-19 pandemic. Our project focuses on leveraging data science and cloud computing to address the unequal impact of healthcare crises on various communities, with a special emphasis on Maryland.

## Problem Statement

Traditional methods of allocating medical resources based solely on population often overlook the nuanced impact of socioeconomic factors and health disparities. Our aim is to develop a predictive model that, given social determinants of health (SDOH), healthcare measures, and population data, can forecast COVID-19 case counts in Maryland zip codes, thereby facilitating a more equitable distribution of healthcare resources.

## Goals

1. **Insight Generation:** Analyze the relationships between SDOH factors, healthcare measures, population data, and COVID-19 cases at the zip-code level in Maryland.
2. **Predictive Modeling:** Develop a model to predict COVID-19 cases in Maryland zip codes, incorporating key SDOH and health measures as features.
3. **Optimization:** Refine the model to minimize Root Mean Square Error (RMSE), ensuring accurate predictions.
4. **Resource Allocation:** Use the model to guide equitable allocation of staffing and medical supplies across Maryland zip codes.

## Non-Goals

- Limiting the scope to Maryland to keep the dataset manageable and focused.
- Excluding time series analysis to concentrate on the impact of static factors on COVID-19 cases.

## Data Sources

Our analysis leverages four primary datasets and a crosswalk for ZIP code and ZTCA conversion:

1. [Maryland COVID-19 Cases by Zip Code](https://opendata.maryland.gov/Health-and-Human-Services/MD-COVID-19-Cases-by-ZIP-Code/ntd2-dqpx/about_data)
2. [Social Determinants of Health Database](https://www.ahrq.gov/sdoh/data-analytics/sdoh-data.html#download)
3. [PLACES: Local Data for Better Health](https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-ZCTA-Data-2023/qnzd-25i4/about_data)
4. [Maryland Census Data](https://data.imap.maryland.gov/datasets/eb706b48117b43d482c63d02017fc3ff/explore?location=38.795704%2C-77.268400%2C7.90)
5. [ZTCA to Zip Code Crosswalk](https://udsmapper.org/zip-code-to-zcta-crosswalk/)


## Methodology

The project encompasses data preparation, exploratory data analysis, model training, and implementation for real-world application. We utilized AWS SageMaker for model development and training, focusing on creating a regression model optimized for minimizing RMSE.

## Recommendations

Based on our findings, we recommend prioritizing resource allocation to zip codes identified as high-risk due to socioeconomic disparities. Implementing our model's predictions will enable a more responsive and equitable healthcare crisis management approach.

## Repository Structure

- `data/`: Contains datasets used for analysis.
- `notebooks/`: Jupyter notebooks detailing our data analysis and modeling process.
- `src/`: Source code for data preprocessing, modeling, and analysis.
- `design`: Design Documentation **(assuming the final design doc goes in this folder)**

## Getting Started

To replicate our analysis or explore the datasets:

1. Clone the repository.
2. Navigate to the `notebooks/` directory to find Jupyter notebooks with detailed analysis steps.
3. Data used in the analysis is stored in the `data/` directory.
