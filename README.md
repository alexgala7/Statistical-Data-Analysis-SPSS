# Statistical Data Analysis: Solving Time Performance & Learning Curves

This repository contains the final project for the **Probability Theory and Statistics** course (June 2023). The project focuses on statistical inference and predictive modeling using **IBM SPSS**, analyzing the performance and learning patterns of players in a word-puzzle game.

## 🚀 Project Overview
The study analyzes two datasets: `timeA` (Player A, experienced) and `timeB` (Student, new player). The goal is to compare performance metrics and model the "learning effect" over time through linear regression.

## 🛠 Methodology & Tools
* **Software:** IBM SPSS Statistics
* **Statistical Techniques:** Descriptive Analysis, Hypothesis Testing (t-tests), Confidence Intervals (95%), Linear Regression, and Correlation Analysis.

## 📊 Statistical Highlights & Results (Based on Group 107 Data)

### 1. Comparative Analysis
* **Performance:** Hypothesis testing (Independent Samples T-Test) confirmed that **Player B (Student)** achieved a significantly lower mean solving time than Player A.
* **Variability:** 95% Confidence Intervals for standard deviation:
  * Player A: $\sigma \in [26.71, 40.58]$
  * Player B (Student): $\sigma \in [23.82, 34.69]$
* **Key Visual:**
![Boxplot Comparison](./images/boxplot_comparison.png)
*Figure 1: Comparison of solving times (timeA vs timeB) showing lower median for Student.*

### 2. Regression & Learning Curves
* **Correlation:** Found significant negative correlation for both, showing the learning effect:
  * Player A: $r = -0.781$
  * Student (Player B): $r = -0.835$ (Stronger correlation than Player A)
* **Your Estimated Models (Page 9):** * Player A: $time = 145.318 - 0.622 \times day$
  * Player B (Student): $time = 120.457 - 0.730 \times day$
* **Interpretation:** Your learning rate (slope -0.730) is actually **faster** than Player A's (-0.622), meaning you improved more quickly!

![Linear Regression](./images/regression_line.png)
*Figure 2: Linear regression model visualizing your specific learning curve ($R^2 = 0.697$).*

## 📋 Key Findings
* **Learning Rate:** Both players demonstrated nearly identical learning rates (slopes of -0.622 vs -0.618).
* **Stability:** Player B's learning rate remained stable throughout the study, while Player A showed accelerated improvement in the later stages.
* **Limitations:** The report includes a critical evaluation of model assumptions (normality and variance equality).

## 📂 Repository Structure
* `/docs`: Project guidelines and the final analytical report.
* `/images`: Key charts extracted from SPSS (Boxplots, Scatter Plots, Coefficients).

## 📂 Project Documents
* [📄 Assignment Description (PDF)](./docs/Probability_Statistics_Assignment.pdf)
* [✅ Final Project Report (PDF)](./docs/Statistical_Analysis_Report.pdf)

## 🎓 Academic Info
* **Institution:** Aristotle University of Thessaloniki (AUTh)
* **Team:** A. Alexiadis (10617) & A. Galazoulas (10629)
* **Instructor:** Prof. D. Kugiumtzis
