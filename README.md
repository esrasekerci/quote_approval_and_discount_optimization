# Insurance Quote Approval and Discount Optimization

## Overview

Predictive modeling and optimization framework for insurance quote acceptance. Combines statistical analysis with machine learning to identify high-value prospects for discount targeting, maximizing portfolio growth while protecting margins.

## Methodology

**Phase 1: Exploratory Analysis (R)**
- Statistical testing on 15+ features (age, premium, vehicle type, customer segment)
- Portfolio segment identified as strongest approval predictor
- Premium effect varies significantly by customer type

**Phase 2: Machine Learning (Python)**
- Three models evaluated: Logistic Regression, Random Forest, Gradient Boosting
- Gradient Boosting selected: 82% ROC-AUC, 85% Average Precision
- 5-fold cross-validation with SMOTE for class imbalance

**Phase 3: Discount Optimization (MILP)**
- Strategic discount allocation (0-10% reduction by quote)
- Segment-specific targeting maximizes approval rate
- Expected impact: 8-15% portfolio growth, <3% margin reduction

## Files

| File | Purpose |
|------|---------|
| `Case_Study_Data.xlsx` | Raw insurance data |
| `model_ready.xlsx` | Cleaned dataset for modeling |
| `analysis.Rmd` | Statistical analysis and EDA |
| `ml.ipynb` | ML models and optimization |
| `03042026.pptx` | Initial findings |
| `14042026.pptx` | Final recommendations |

## Results

- **Best Model:** Gradient Boosting (ROC-AUC: 0.82)
- **Key Insight:** Portfolio segment and premium are primary approval drivers
- **Recommendation:** Implement real-time prediction with quarterly retraining

## Technical Stack

**Languages:** R, Python  
**Libraries:** tidyverse, scikit-learn, xgboost, scipy, imbalanced-learn

## Limitations

Historical data only; approval behavior may shift. Limited external features (no agent quality, customer LTV, competitive data). Geographic patterns aggregated to province level.

---

**Author:** Esra Sekerci (2026)
