# ALY 6015 — Intermediate Analytics

**Northeastern University · Roux Institute**  
**Course:** ALY 6015 Intermediate Analytics  
**Language:** R · ggplot2 · glmnet · caret

---

## Overview

A rigorous treatment of intermediate statistical methods and machine learning in R, applied to real-world datasets including the ISLR College dataset and 130 years of Maine climate data from NOAA.

---

## Modules

### Module 1 — Linear Regression & Diagnostics
- Multiple linear regression with `lm()`
- Residual analysis: Q-Q plots, residuals vs fitted, scale-location
- Influential point detection (Cook's distance, leverage)
- Model fit metrics: R², adjusted R², F-statistic, AIC

---

### Module 2 — Chi-Square Tests & ANOVA
Real-world applications across healthcare, transportation, agriculture, and education:

- **Blood type distribution:** Chi-square goodness-of-fit (hospital vs population)
- **Airline on-time performance:** Chi-square test vs government benchmarks — p < 0.0002
- **Movie admissions by ethnicity:** Chi-square independence test — p < 2.2×10⁻¹³
- **Military rank by branch:** Chi-square — χ² = 405.73
- **Sodium in foods:** One-way ANOVA across condiments, cereals, desserts — p = 0.021
- **Plant growth:** Two-way ANOVA (light × food supplement interaction) — p = 0.077
- **Crop yield:** Two-way ANOVA — Fertilizer p = 0.032 · Density p = 0.014

---

### Module 3 — GLM & Logistic Regression ⭐
**Dataset:** ISLR College dataset · 777 U.S. colleges · 18 variables

- EDA: bar charts, histograms, boxplots, scatter plots
- 70/30 train/test split
- Logistic regression with `glm()` — predictors: F.Undergrad, Outstate, Enroll
- **Accuracy: 91.45%** · Sensitivity: 94.83% · Specificity: 81.67%
- Confusion matrix analysis · false positive vs false negative trade-offs
- **ROC curve: AUC = 0.96**

---

### Module 4 — Regularisation: Ridge, LASSO & Stepwise ⭐
**Dataset:** ISLR College dataset · predicting graduation rates (Grad.Rate)

- Ridge regression: λ tuned via 10-fold cross-validation · λ_min = 3.214
- LASSO regression: feature selection — 12 of 17 predictors retained · λ_min = 0.41
- Stepwise regression: AIC-based forward/backward selection · 12 predictors retained
- **RMSE comparison:**

| Model | Train RMSE | Test RMSE |
|---|---|---|
| Ridge | 12.51 | 13.46 |
| LASSO | 12.51 | 13.42 |
| Stepwise | 12.45 | 13.37 |

- Key finding: Top10perc and Private status are strongest graduation rate predictors

---

### Module 5 — Nonparametric Methods & Simulation ⭐
- **Sign test:** Game attendance (median = 3,000) · Lottery ticket sales
- **Wilcoxon rank sum test:** Prison sentences by gender · Baseball wins NL vs AL
- **Wilcoxon signed-rank test:** 4 hypothesis tests at varying α and tail configurations
- **Kruskal-Wallis test:** Mathematics literacy scores across Western Hemisphere, Europe, Eastern Asia
- **Spearman rank correlation:** Subway vs commuter rail passenger trips
- **Monte Carlo simulation:** Average boxes to collect 4 prizes (result: 7.97 ≈ theoretical 8.33)
- **Lottery simulation:** Average tickets to spell "big" given unequal probabilities

---

### Group Final Project — 130-Year Maine Climate Analysis ⭐
**Dataset:** Maine Climate Office · University of Maine · NOAA · 1895–2024  
**Team:** Alexandra Offei · Conor Noonan · Alex Morrow

**Variables:** Temperature Anomaly · Average Temp · Min Temp · Max Temp · Precipitation Anomaly · Precipitation  
**Regions:** Statewide · North (CD1) · Central (CD2) · Coastal (CD3) · Seasonal breakdowns

**Research Questions:**
1. Is there a significant difference in mean temperatures and precipitation by year?
2. Is there a relationship between temperature and precipitation anomalies?
3. Do region and season have any relationship with climate variables?
4. Does warming in the data match expected rates from climate science?

**Methods:** Linear regression · ANOVA · Chi-square goodness-of-fit and independence tests

---

## Skills Demonstrated

`R` `ggplot2` `glmnet` `glm()` `lm()` `Logistic regression` `Ridge` `LASSO` `Cross-validation` `ROC/AUC` `ANOVA` `Chi-square` `Nonparametric tests` `Monte Carlo simulation` `Climate data analysis`
