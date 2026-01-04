# GDT500: MULTIVARIABLE ANALYSIS (Regression Analysis)

## Overview
This repository contains my group’s coursework submission for GDT500 – Multivariable Analysis (Doctor of Public Health, Universiti Sains Malaysia).

The project demonstrates the use of linear regression and logistic regression on simulated datasets, following the full workflow required in the assignment brief: data generation, exploratory data analysis, model fitting, diagnostics, interaction assessment, and interpretation of results.

All analyses were conducted in R and documented using Quarto.

## Assignment Context
- Instructor: Professor Kamarul Imran Musa
- Assessment type: Group assignment (simulated data)

## Group Information
Group 3:
  1. Siti Nurhafizah binti Saharudin (23202464)
  1. Muamar Iskandar bin Mohamaed Yusoff (23202846)
  1. Nur Fazlina binti Dzulkifli (23202967)
  1. Yogeswary Mithra A/P Nandi Mithra (23202677)

## What this project covers
Two separate regression analyses were performed using simulated data (n = 200 per dataset):
  1. Linear Regression – Quality of Life 
      - Outcome: Quality of Life (qol, continuous)
      - Predictors:
        - Years of working experience (years_working, continuous)
        - Physical activity score (phys_activity, continuous)
        - Obesity status (obesity, binary)
      - Key focus:
        - How obesity status modifies the association between physical activity and quality of life

2. Logistic Regression – Depression
      - Outcome: Depression status (depression, binary)
      - Predictors:
        - Years of working experience (years_working, continuous)
        - Physical activity score (phys_activity, continuous)
        - Obesity status (obesity, binary)
      - Key focus:
        - Whether obesity status modifies the association between physical activity and depression

Both analyses include models with and without interaction terms, followed by comparison and interpretation.

## Repository Structure
The files in this repository are organised by analysis type, with separate Quarto documents for linear and logistic regression.

```text

├── QOL/
│   ├── QOL.qmd                                                           # Linear regression analysis document (Quarto source)
│   ├── QOL.html                                                          # Rendered HTML report for linear regression
│   └── styles.css                                                        # custom styling for consistent report formatting
│   
│
├── DEPRESSION/
│   ├── Logistic Regression Analysis of Depression.qmd                     # Logistic regression analysis document (Quarto source)
│   ├── Logistic Regression Analysis of Depression.html                    # Rendered HTML report for logistic regression
│   └──  styles.css                                                         # custom styling for consistent report formatting
│   
├── README.md                            # This file
└── LICENSE                              # MIT License

```

## Methods (Summary)

**PART A - Data Generation**
  - Simulated datasets with realistic ranges and distributions
  - Fixed random seeds used for reproducibility
  - Interaction effects deliberately included
  - A small number of influential observations added to support diagnostics

**PART B - Exploratory Data Analysis**
  - Summary statistics (mean, SD, median, IQR)
  - Frequency and proportion tables
  - Histograms, boxplots, scatter plots, and bar charts
  - Correlation matrices for continuous variables

**PART C - Regression Analysis**
  - Linear regression for Quality of Life
  - Logistic regression for Depression
  - Model comparison (with vs without interaction terms)

**PART D - Model Checking**
  - **Linear regression:**
    Linearity, normality of residuals, homoscedasticity, influential points (Cook's distance, DFBETAS, Leverage points)
  - **Logistic regression:**
    Linearity in the logit, goodness-of-fit, multicollinearity, influential points (Cook's distance, DFBETAS, Leverage points)

**PART E - Results Presentation and interpretations**
  - Results are presented using regression tables and model performance statistics, with interaction plots included to support interpretation of the findings.

## How to reproduce the analysis
1. Open the .qmd files in RStudio (with Quarto installed)
2. Render the documents using:
    ```text
    r
    
    - quarto render QOL.qmd
    - quarto render "Logistic Regression Analysis of Depression.qmd"
    ```
3. The rendered HTML files will reproduce all tables, figures, and outputs.

## Limitation
- All data used in this project are simulated, so findings are for methodological demonstration only.
- Effect sizes and statistical significance were influenced by how the data were generated.
- Results should not be interpreted as real-world evidence but as examples of correct regression workflow and interpretation.

## Contact
For questions or clarifications regarding this analysis:
- Primary Contact: SITI NURHAFIZAH SAHARUDIN
- Email: fizasaharudin@gmail.com

## Course information
**Programme:** Doctor of Public Health (DrPH)
**Course:** GDT500 – Multivariable Analysis
**Institution:** Universiti Sains Malaysia
**Academic year:** 2026
