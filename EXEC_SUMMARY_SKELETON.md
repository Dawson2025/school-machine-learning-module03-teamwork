# Executive Summary Skeleton — Module 03: Housing Estimates

> **Template**: Reddic Housing LLC — House Price Estimate Report
> **Page limit**: 3 body pages (title page and notebook links page don't count)
> **Format**: Will be converted to .docx using module 03 template (summary.docx)

---

## [TITLE PAGE] — Does NOT count toward 3 pages

**Reddic Housing LLC**
**House Price Estimate Report**

- Dawson
- Peter
- Tanner

---

## 1. Executive Summary

*2-3 paragraphs. High-level overview of the project, approach, and top-line results.*

### Core Task: House Price Prediction Model (ITEM-M03-001)

<!-- Brief description of the prediction task — what was built and why -->

### Stakeholder Summaries

<!-- Cecil: "Predictions achieved [metric] reliability" -->
<!-- William: "Top price drivers identified: [features]" -->
<!-- Devon: "External factors [were/were not] investigated" -->

### Discussion Q1: What Kind of ML Problem Is This? (Devon, CEO)

<!-- Explain why this is a regression problem (predicting continuous price values). Keep it brief — 1-2 sentences woven into the overview. -->

---

## 2. Methodology

*Describe the approach: data exploration, preprocessing, model selection, tuning.*
*Rubric: Quality of Implementation and Approach (40 pts)*

### Data Exploration

<!-- Key findings from exploring housing.csv — distributions, correlations, outliers, 21 features, 20k rows -->

### Preprocessing Pipeline

<!-- Cleaning steps, encoding, feature engineering, derived features -->

### Discussion Q4: Handling Features with Different Ranges (Johnny, Intern)

<!-- How did you handle square footage and other features with vastly different ranges for gradient boosted trees? Note: tree-based models are generally scale-invariant, but explain your approach. -->

### Model Selection & Tuning

<!-- Models tried (baseline, XGBoost, Random Forest, etc.), hyperparameter tuning approach -->

### External Data Investigation (ITEM-M03-005 — Devon, CEO — Above & Beyond)

<!-- Did the team find and merge external data sources via zip code? If yes, describe sources and merge process. If not, note it was time-constrained. -->

---

## 3. Results

*Present quantitative results — metrics, comparisons, holdout performance.*
*Rubric: Quality of Evaluation (10 pts)*

### Model Comparison

<!-- Table comparing models: Model | RMSE | MAE | R² | Notes -->

| Model | RMSE | MAE | R² | Notes |
|-------|------|-----|----|-------|
| Baseline (mean) | | | | |
| XGBoost | | | | |
| | | | | |

### Best Model Performance

<!-- Cross-validation results for the selected model -->

### Prediction Reliability Evidence (ITEM-M03-002 — Cecil, VP Customer Relations)

<!-- Q-CECIL-01: "Can you provide quantifiable evidence that predictions are reliable?" -->
<!-- Multiple metrics, cross-validation, prediction vs actual analysis, plain-language explanation -->

### Discussion Q2: Best Confidence Metric (Cecil, VP Customer Relations)

<!-- Which metric best shows confidence: SSE, MSE, RMSE, or R²? Explain your choice with reasoning. Weave into the reliability discussion above. -->

### Holdout Predictions (ITEM-M03-003 — Cecil, VP Customer Relations)

<!-- Summary of holdout predictions generated. File: team8-module3-predictions.csv -->
<!-- DO NOT include the holdout CSV content here — just confirm predictions were generated and summarize. -->

---

## 4. Key Findings

*Business-relevant insights derived from the analysis.*
*Rubric: Quality of Insights and Inferences (20 pts)*

### Feature Importance Analysis (ITEM-M03-004 — William, VP Finance)

<!-- Q-WILLIAM-01: "Which property types weigh most heavily in predicted prices?" -->
<!-- Ranked feature importance with business interpretation. Top 5-7 drivers explained in non-technical language. -->
<!-- Address C-WILLIAM-01: Prove AI adds value over Excel -->

### External Factors Findings (ITEM-M03-005 — Devon, CEO)

<!-- Q-DEVON-01: "Are there additional factors affecting prices we aren't accounting for?" -->
<!-- Report whatever was found, even if time-limited. Address C-DEVON-01: unaccounted factors. -->

### Discussion Q3: Insurance & Ethics Question (William, VP Finance)

<!-- William asks about lowering estimates for "unsavory neighborhoods" to protect insurance customers. -->
<!-- Evaluate the 4 options: -->
<!-- 1. Lower predicted price for specific neighborhoods before training -->
<!-- 2. Add average income or demographic info as features -->
<!-- 3. Post-prediction price reduction for specific zip codes -->
<!-- 4. This would violate federal laws and/or ethics -->
<!-- Address Fair Housing Act, redlining, ethical implications. This is a 5-point rubric item. -->

### Surprising or Counterintuitive Findings

<!-- Any unexpected patterns in the data or model behavior -->

---

## 5. Visualizations

*Presentational-quality visuals for executive audience. NOT exploratory charts about model training.*
*Rubric: Quality of Visuals (15 pts)*

### [FIGURE 1]: Feature Importance Bar Chart

*Caption: [describe what the chart shows]*

<!-- For William — horizontal bar chart, sorted by importance, labeled for executives -->
<!-- Maps to ITEM-M03-004 -->

### [FIGURE 2]: Prediction vs Actual Scatter Plot

*Caption: [describe what the chart shows]*

<!-- For Cecil — shows prediction accuracy, include R² and trend line -->
<!-- Maps to ITEM-M03-002 -->

### [FIGURE 3]: Model Performance Comparison

*Caption: [describe what the chart shows]*

<!-- Comparison of all models tried — RMSE, R² -->
<!-- Maps to ITEM-M03-001 -->

### [OPTIONAL FIGURE 4]: Additional Visualization

*Caption: [describe what the chart shows]*

<!-- Above & Beyond options: residual distribution, price by key features, geographic map -->

---

## 6. Strengths

*What the approach did well. Build confidence in the model.*

### Model Strengths

<!-- Strong performance metrics, effective feature engineering, robust evaluation -->

### Process Strengths

<!-- Team collaboration, methodology, what XGBoost brought vs simpler models -->

---

## 7. Limitations

*Honest assessment of caveats. Acknowledging limitations is key for the Evaluation rubric.*

### Data Limitations

<!-- Missing features, noise, geographic/temporal constraints -->

### Model Limitations

<!-- Where predictions are less reliable, overfitting risks and mitigations -->

### Scope Limitations

<!-- Time constraints, external data availability (C-DEVON-02) -->

---

## 8. Conclusion

*Wrap up with actionable recommendations. 2-3 paragraphs.*

### Direct Answers to Stakeholders

<!-- Cecil: "Our model achieves [metric], demonstrating reliable predictions for customer-facing use." -->
<!-- William: "The top price drivers are [features], which your team can leverage for [action]." -->
<!-- Devon: "External factors like [X] show promise for future investigation." -->

### Recommendations & Next Steps

<!-- What should Reddic Housing do next? -->

---

## [NOTEBOOK LINKS PAGE] — Does NOT count toward 3 pages

### Python Notebooks

Below are GitHub Gist links to the notebooks we used during this case study:

- 

---
