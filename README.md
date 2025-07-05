# Residual Strength Prediction in FRP Composites

This project aims to predict the **residual strength** of **Fiber-Reinforced Polymer (FRP)** composites subjected to **cyclic (fatigue) loading** using a combination of traditional modeling approaches and machine learning techniques.

## Problem Overview

FRP composites degrade progressively under fatigue, leading to a decline in their load-bearing capacity—referred to as residual strength. Accurately predicting this decline is critical for ensuring structural safety and integrity.

## Prediction Methods Explored

1. **Empirical Models** – Fit experimental data using power-law equations.
2. **Damage Mechanics Models** – Use damage variables to model degradation.
3. **Fracture Mechanics** – Analyze crack propagation and delamination.
4. **Micromechanical Models** – Simulate fiber/matrix behavior and interactions.
5. **Machine Learning** – Data-driven prediction using stress levels, cycles, and material properties.

## Dataset Overview

- **Source**: [GitHub Research Dataset](https://github.com/Dewa1989/Residual-Fatigue-Strength/tree/main)
- **File**: `Residual_Fatigue.csv`
- **Features**:
  - Material, Nature, Stacking (encoded)
  - UTS (Ultimate Tensile Strength)
  - Stress Amplitude & Ratio
  - Frequency, Number of Plies
  - Fatigue Cycles, Normalized Fatigue Life
- **Target**: Residual Strength

## Methodology

1. **Material Selection**: Define composite and layup (e.g., [0/90], ASTM D3479).
2. **Fatigue Testing**: Apply cyclic loads at various stress ratios and record intermediate/final strengths.
3. **Damage Monitoring** (Optional): Acoustic Emission, Thermography, etc.
4. **Data Collection**: Cycle count, initial/residual strength, failure modes.
5. **Modeling**:
   - Empirical / Damage Mechanics Models
   - Machine Learning Regressors
6. **Evaluation**:
   - Metrics: RMSE, R², Cross-validation
7. **Prediction**:
   - Residual strength vs. fatigue cycles
   - Comparison across different configurations

## Machine Learning Models Used

### Baseline Regressors
- Linear Regression
- Ridge Regression
- Lasso Regression
- Elastic Net

### Tree-Based Models
- Random Forest Regressor (with GridSearchCV)
- Gradient Boosting Regressor (with GridSearchCV)

### Neural Network
- MLP Regressor (scikit-learn)

## Graphs & Analysis

1. **Residual Strength vs. Cycles** – Visualizes degradation trend.
2. **Actual vs. Predicted Plot** – Evaluates regression model accuracy.
3. **Confusion Matrix** – Categorical classification into High, Medium, Low strength.

## Project Files

- `ML Project Report.docx` – Full technical report
- `Research article.pdf` – Reference material
- `Residual_Fatigue.csv` – Dataset

## References

- Dataset: [Residual Fatigue Strength GitHub Repository](https://github.com/Dewa1989/Residual-Fatigue-Strength/tree/main)

---

## Author

**Tanishka Khandelwal**

