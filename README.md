# FINALTICS_INTERNSHIP
Tasks performed during the Internship
# Internship Tasks Overview

This repository contains Jupyter Notebooks documenting analytical tasks completed during an internship. The tasks focus on data analysis, statistical modeling, and deriving insights from different datasets.

## Project Structure

* `Sales TASK (1).ipynb`: Analyzes the impact of advertising spending on sales.
* `FACEBOOK TASK (1).ipynb`: Investigates the performance of different Facebook post types.

---

## 1. Sales Task: Advertising Impact Analysis

### Objective
The primary objective of this task was to analyze the relationship between advertising spending across various media (TV, Radio, Newspaper) and product sales. This involved understanding individual and combined effects of advertising channels on sales, and building predictive models.

### Methodology
1.  **Data Loading and Exploration**: Initial inspection of the dataset to understand its structure and content.
2.  **Exploratory Data Analysis (EDA)**:
    * Visualizing the distribution of spending across TV, Radio, and Newspaper advertising, as well as the distribution of Sales.
    * Analyzing the correlation between advertising channels and sales using a heatmap to identify strong relationships.
3.  **Linear Regression Modeling**:
    * **Simple Linear Regression**: Developed individual regression models for TV, Radio, and Newspaper advertising against Sales to understand the independent impact of each.
    * **Multiple Linear Regression**: Constructed a comprehensive model incorporating all three advertising channels to predict Sales, accounting for their combined influence.
4.  **Model Evaluation**: Assessed the performance of the regression models using metrics such as R-squared, Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).

### Technologies and Libraries
* Python
* `pandas` for data manipulation and analysis
* `numpy` for numerical operations
* `matplotlib.pyplot` for data visualization
* `seaborn` for enhanced statistical data visualization
* `sklearn.model_selection` for splitting data into training and testing sets
* `sklearn.linear_model` for linear regression models
* `sklearn.metrics` for evaluating model performance

### Key Findings
* Distributions of TV, Radio, Newspaper spending, and Sales were analyzed.
* Correlations between advertising spend and sales were identified, showing stronger relationships with certain media (e.g., Radio and TV).
* Regression models provide insights into how changes in advertising budget affect sales.

---

## 2. Facebook Task: Post Performance Analysis

### Objective
The aim of this task was to analyze the performance of different Facebook post types (`status_type`) based on engagement metrics such as reactions, comments, and shares.

### Methodology
1.  **Data Loading and Initial Inspection**: Loaded the Facebook data and performed initial checks for structure and missing values.
2.  **Data Preprocessing**:
    * Identified and handled missing values, specifically noting columns with entirely null values (`Column1`, `Column2`, `Column3`, `Column4`) and dropping them as they were deemed irrelevant for the analysis.
    * Examined data types and ensured consistency for analysis.
3.  **Engagement Metrics Analysis**:
    * Calculated descriptive statistics for key engagement metrics (`num_reactions`, `num_comments`, `num_shares`, `num_likes`, `num_loves`, `num_wows`, `num_hahas`, `num_sads`, `num_angrys`).
    * Grouped the data by `status_type` to compute average reactions, comments, and shares for each type of post (e.g., video, photo, status, link).

### Technologies and Libraries
* Python
* `numpy` for numerical operations
* `pandas` for data manipulation and analysis

### Key Findings
* Different status types exhibit distinct engagement patterns:
    * **Status updates** tend to have the highest average number of reactions and a good average for comments, but low shares.
    * **Video posts** are highly effective in generating comments and shares, with a moderate number of reactions.
    * **Photo posts** generally receive a good number of reactions, but fewer comments and very low shares compared to videos or status updates.
    * **Link posts** generally show lower engagement across all metrics.
* These insights can help optimize content strategy on Facebook by tailoring post types to achieve specific engagement goals.
