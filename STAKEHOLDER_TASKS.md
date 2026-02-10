# Module 03 — Stakeholder Tasks & Team Assignments

## Team Members

| Member | Role | Tasks Claimed |
|--------|------|---------------|
| **Dawson** | Team Member | Tasks 5, 7 |
| **Peter** | Project Manager | Task 2 (holdout CSV) |
| **Tanner** | Team Member | — |

---

## Core Task — SHARED (Everyone Contributes)

Building the regression model is shared work. Everyone contributes to making it happen.

- [ ] Load and explore housing.csv (20k rows, 21 columns, target: `price`)
- [ ] Data cleaning (missing values, outliers, duplicates)
- [ ] Feature engineering (encoding, scaling, binning, derived features)
- [ ] Train baseline model(s)
- [ ] Train XGBoost + other models
- [ ] Hyperparameter tuning
- [ ] Cross-validation + evaluation metrics (RMSE, MAE, R², MAPE)
- [ ] Draft executive summary (use EXEC_SUMMARY_SKELETON.md)
- [ ] Create visualizations (presentational quality for executives)
- [ ] Quality assurance + rubric check
- [ ] Final submission

---

## Stakeholder Tasks — TO DIVIDE (7 total)

These are specific stakeholder requests beyond building the core model. Each should be claimed by a team member.

### Task 1: Prediction Reliability Evidence (Cecil, VP Customer Relations)

**Assigned to**: _____________

> "The biggest thing I want to see is quantifiable evidence that the predictions we come up with are reliable."

**Deliverable**:
- [ ] Multiple evaluation metrics showing model accuracy
- [ ] Cross-validation or holdout validation proving generalization
- [ ] Prediction vs actual scatter plot
- [ ] Plain-language explanation of reliability

**Goes in**: Exec Summary Section 3 (Results)

---

### Task 2: Holdout Set Predictions CSV (Cecil, VP Customer Relations)

**Assigned to**: Peter (Project Manager)

> "We actually just received a batch of new home data. Could you run your model on it to make some predictions for us?"

**Deliverable**:
- [ ] Run final model on `housing_holdout_test.csv`
- [ ] CSV: single column, header `price`, one prediction per row
- [ ] Filename: **`team8-module3-predictions.csv`** (DASHES, not underscores!)
- [ ] Verify format before submitting

**CRITICAL WARNING**: Module 02 holdout scored 0/100 because the file was named wrong (underscores instead of dashes). Double-check the filename!

**Goes in**: Exec Summary Section 3 (Results) — mention that predictions were generated

---

### Task 3: Feature Importance Analysis (William, VP Finance)

**Assigned to**: _____________

> "I'd like to know which property types are weighing most heavily in the house prices predicted by your model."

**Deliverable**:
- [ ] Feature importance ranking from the model
- [ ] Horizontal bar chart (presentational quality)
- [ ] Business-language explanation of top 5-7 price drivers
- [ ] Show that AI reveals insights Excel can't

**Goes in**: Exec Summary Section 4 (Key Findings) + Section 5 (Visualizations, Figure 1)

---

### Task 4: External Factors Investigation (Devon, CEO) — Above & Beyond

**Assigned to**: _____________

> "Is there are additional factors about these areas that might be affecting prices, which we aren't taking into account?"

**Deliverable**:
- [ ] Research external data sources for King County (school ratings, crime stats, income, transit)
- [ ] Find and merge at least one external dataset via zip code
- [ ] Test whether external features improve predictions
- [ ] Report findings (even if time-limited)

**Goes in**: Exec Summary Section 2 (Research) + Section 4 (Key Findings)

---

### Task 5: Feature Scaling Explanation (Johnny, Data Science Intern)

**Assigned to**: Dawson

> "I've noticed that a lot of the features use pretty different ranges. For example, how should we handle square footage?"

**Deliverable**:
- [ ] Explain approach to handling features with different ranges
- [ ] Note that tree-based models (XGBoost) are generally scale-invariant
- [ ] Describe any scaling/normalization actually applied and why

**Goes in**: Exec Summary Section 2 (Research Conducted) — Discussion Q4

---

### Task 6: Insurance & Ethics Question (William, VP Finance)

**Assigned to**: _____________

> "Is there a way we can easily identify properties in low income areas and have the model lower those estimates to protect our insurance customers' interests?"

**Deliverable**:
- [ ] Evaluate all 4 options presented:
  1. Lower predicted price for specific neighborhoods before training
  2. Add average income or demographic info as features
  3. Post-prediction price reduction for specific zip codes
  4. This would violate federal laws and/or ethics
- [ ] Address Fair Housing Act and redlining implications
- [ ] Well-reasoned response with supporting examples

**Goes in**: Exec Summary Section 4 (Key Findings) — Discussion Q3

---

### Task 7: ML Problem Type Explanation (Devon, CEO)

**Assigned to**: Dawson

> "What kind of machine learning problem do you think we're looking at here?"

**Deliverable**:
- [ ] Explain why this is a regression problem
- [ ] Connect to the data (continuous price target) and business model (price estimates)
- [ ] Brief and clear for a non-technical audience

**Goes in**: Exec Summary Section 1 (Executive Summary) — Discussion Q1

---

## Task Assignment Summary

| # | Task | Stakeholder | Assigned | Exec Summary Section |
|---|------|-------------|----------|---------------------|
| 1 | Prediction reliability evidence | Cecil | Tanner | 3. Results |
| 2 | Holdout CSV predictions | Cecil | Peter | 3. Results |
| 3 | Feature importance analysis | William | _______ | 4. Key Findings |
| 4 | External factors investigation | Devon | _______ | 2. Research + 4. Findings |
| 5 | Feature scaling explanation | Johnny | Dawson | 2. Research |
| 6 | Insurance & ethics question | William | Tanner | 4. Key Findings |
| 7 | ML problem type explanation | Devon | Dawson | 1. Executive Summary |

**Unassigned tasks**: 1, 3, 4, 6 (need Peter and Tanner to claim)

