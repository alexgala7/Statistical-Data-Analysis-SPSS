# Statistical Data Analysis: Solving Time Performance & Learning Curves

This repository contains the final statistical analysis project for the **Probability Theory and Statistics** course (June 2023). The study utilizes **IBM SPSS Statistics** to analyze and model the learning progress of two players in word-puzzle games.

## 🚀 Project Overview
The analysis compares two datasets: `timeA` (experienced player) and `timeB` (student/group data). By applying statistical inference and regression models, we evaluate performance differences and the "learning effect" over time.

## 🛠 Methodology & Tools
* **Software:** IBM SPSS Statistics
* **Statistical Techniques:** Descriptive Statistics, Independent Samples T-Test, Confidence Intervals (95%), Simple & Piecewise Linear Regression.

## 📊 Key Statistical Findings

### 1. Comparative Analysis
* **Inference:** Hypothesis testing confirmed that **Player B (Student)** achieved significantly lower mean solving times compared to Player A.
* **Variability (95% CI for $\sigma$):**
    * Player A: $[26.71, 39.69]$
    * Player B (Student): $[24.12, 40.71]$
* **Visual Data:**
![Boxplot Comparison](./images/boxplot_comparison.png)
*Figure 1: Boxplot comparison of solving times (timeA vs timeB).*

### 2. Correlation & Regression Modeling
* **Correlation ($r$):** A very strong negative correlation was found for the student sample ($r = -0.913$), significantly stronger than Player A's ($r = -0.781$).
* **Linear Models:**
    * **Player A:** $time = 145.318 - 0.622 \times day$ ($R^2 = 0.61$)
    * **Player B (Student):** $time = 145.893 - 0.800 \times day$ ($R^2 = 0.833$)
* **Learning Rate:** The student demonstrated a faster overall learning rate (slope $-0.800$) compared to Player A (slope $-0.622$).

![Linear Regression](./images/regression_line.png)
*Figure 2: Linear regression model visualizing the learning curve for the Student dataset.*

### 3. Piecewise Regression Analysis
The study investigated shifts in learning trends by splitting the data into two phases:
* **Player A:** Improvement accelerated after day 75 (slope increased from $-0.622$ to $-0.755$).
* **Player B (Student):** Showed an extremely rapid initial adaptation (slope $-1.060$ for the first 61 days), followed by a stabilization phase (slope $-0.517$).

## 📂 Repository Structure
* `/docs`: Project guidelines and the final report (`Statistical_Analysis_Report.pdf`).
* `/images`: SPSS output charts (Boxplots, Scatter Plots, Regression Tables).

## 📂 Project Documents
* [📄 Assignment Description (PDF)](./docs/Project2023.pdf)
* [✅ Final Project Report (PDF)](./docs/Statistical_Analysis_Report.pdf)

## 🎓 Academic Info
* **Institution:** Aristotle University of Thessaloniki (AUTh)
* **Department:** Electrical and Computer Engineering (ECE)
* **Course:** Probability Theory and Statistics (2023)
* **Team:** A. Alexiadis (10617) & A. Galazoulas (10629)
* **Instructor:** Prof. D. Kugiumtzis
