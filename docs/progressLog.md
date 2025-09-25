# Progress Log — Groundwater Quality Classification
> Hands-on effort reconstructed from MSc dissertation timeline (Jul–Sep 2024).  
> Hours shown are **personal effort**. Use for transparency, not as a precise time sheet.

---

## Week 1 (01–07 Jul 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 01–07 Jul | Collected CPCB groundwater dataset (2012–2021) & reviewed metadata | PLAN | 6 | 7,872 records from multiple states |
| 01–07 Jul | Exploratory data analysis: distributions of pH, temp, conductivity | EDA | 10 | Detected outliers, missing values |
| 01–07 Jul | Drafted project workflow & repo skeleton | PLAN | 4 | README scaffold |
**Week total: ~20 hrs**

---

## Week 2 (08–14 Jul 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 08–14 Jul | Handled duplicates & standardized state names | CLEAN | 8 | Reduced dataset from 7872 → 7043 |
| 08–14 Jul | Imputed missing values (state-year median for pH/temp/conductivity) | CLEAN | 7 | Used contextual imputation |
| 08–14 Jul | Outlier treatment (pH trimmed 6–9, capped conductivity) | CLEAN | 5 | Domain-guided caps |
**Week total: ~20 hrs**

---

## Week 3 (15–21 Jul 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 15–21 Jul | Designed custom Water Quality Index (WQI) | FEAT | 6 | Weighted sub-indices |
| 15–21 Jul | Feature engineering (sub-indices, label encoding, scaling) | FEAT | 9 | Added risk-scoring emphasis on pH |
| 15–21 Jul | Literature review: WQI methods & ML baselines | PLAN | 5 | Referenced CPCB & WHO guidelines |
**Week total: ~20 hrs**

---

## Week 4 (22–28 Jul 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 22–28 Jul | Built baseline ML pipeline (LogReg + SVM) | ML | 10 | Accuracy ~87–88% |
| 22–28 Jul | Implemented Random Forest baseline | ML | 8 | Accuracy ~96% |
| 22–28 Jul | Documentation of methodology | DOC | 4 | Dissertation draft |
**Week total: ~22 hrs**

---

## Week 5 (29 Jul–04 Aug 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 29 Jul–04 Aug | Implemented XGBoost classifier | ML | 12 | Accuracy ~97.13% |
| 29 Jul–04 Aug | Hyperparameter tuning with GridSearchCV | EVAL | 8 | Improved recall for Poor/Moderate |
**Week total: ~20 hrs**

---

## Week 6 (05–11 Aug 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 05–11 Aug | Cross-validation, PR curve & calibration analysis | EVAL | 12 | Checked class imbalance |
| 05–11 Aug | Feature importance plots & ablation | EVAL | 8 | Confirmed pH dominance |
**Week total: ~20 hrs**

---

## Week 7 (12–18 Aug 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 12–18 Aug | Integrated `geojson` & built choropleth maps | VIS | 12 | Highlighted high-risk states |
| 12–18 Aug | Risk mapping & stakeholder visualization | VIS | 8 | Maps & figures for dissertation |
**Week total: ~20 hrs**

---

## Week 8 (19–25 Aug 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 19–25 Aug | Analysed model drift & thresholds | EVAL | 8 | Adjusted classification cut-offs |
| 19–25 Aug | Drafted ethics & reproducibility section | DOC | 12 | 3,000 words |
**Week total: ~20 hrs**

---

## Week 9 (26 Aug–01 Sep 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 26 Aug–01 Sep | Dissertation writing: results & discussion | DOC | 18 | Wrote ~4,000 words |
| 26 Aug–01 Sep | Repo cleanup: notebooks, figures | PLAN | 4 | Ready for submission |
**Week total: ~22 hrs**

---

## Week 10 (02–13 Sep 2024)
| Date(s) | Activity | Category | Est. Hours | Notes |
|---------|----------|----------|-----------:|-------|
| 02–13 Sep | Final dissertation write-up & submission | DOC | 25 | Total length ~10,000+ words |
| 02–13 Sep | Repo documentation (README, logs, licensing) | DOC | 15 | Prepared for GitHub portfolio |
**Week total: ~40 hrs**

---

## Summary
- **Total personal effort:** ~204 hrs  
- Category split:  
| Category | Hours |
|----------|------:|
| PLAN     | 19 |
| EDA      | 10 |
| CLEAN    | 20 |
| FEAT     | 15 |
| ML       | 30 |
| EVAL     | 28 |
| VIS      | 20 |
| DOC      | 62 |

---

**Categories**:  
- PLAN = Planning/Setup  
- EDA = Exploratory Data Analysis  
- CLEAN = Cleaning/Preprocessing  
- FEAT = Feature Engineering  
- ML = Model training  
- EVAL = Evaluation & tuning  
- VIS = Visualization (plots, maps)  
- DOC = Documentation & dissertation  
