# Improving Quality of Life: Optimal Financial Aid Allocation

## Overview
This project applies data science, predictive modeling, and mathematical optimization to design an evidence-based international aid allocation strategy for Africa. The goal is to predict Human Development Index (HDI) using features that can be directly improved through financial aid, and then optimally allocate a fixed budget across resources to maximize quality of life.

The workflow includes:

- Data integration: Merging multi-source global development datasets (health, sanitation, water access, HDI, country mapping).
- Data preprocessing: Country-level cleaning, missing value imputation, normalization, and consistency harmonization.
- Feature engineering: Distribution correction using transformations and engineered feature evaluation.
- Dataset filtering: Continent-level analysis and Africa-specific modeling.
- Predictive modeling: HDI regression modeling using k-fold cross-validation.
- Model evaluation: Performance analysis using train/test R², prediction stability, and coefficient interpretation.
- Optimization modeling: Budget-constrained convex optimization for aid allocation.
- Sensitivity analysis: Binding and non-binding constraint evaluation.

---

## Key Features

### Data Preprocessing
- Multi-source dataset integration (WHO, Our World in Data, Oxford Martin School)
- Country name normalization and consistency handling
- Modular missing-data imputation functions
- Country-level and continent-level filtering
- Structured feature selection
- Removal of non-actionable policy variables

### Exploratory Data Analysis (EDA)
- Continent-level development comparison
- Developing country distribution analysis
- Life expectancy and development indicators
- Africa-focused scope selection
- Distribution analysis and skew detection
- Correlation analysis

### Feature Engineering
- Distribution correction using square-root transformations
- Feature normalization
- Automated feature combination testing using F-scores
- Statistical significance testing for engineered features
- Removal of redundant and non-informative attributes

### Predictive Modeling
- Target variable: Human Development Index (HDI)
- Model: Linear Regression
- Validation: 5-fold cross-validation
- Performance evaluation:
  - Train/Test R² comparison
  - Prediction stability across folds
  - Overfitting control
- Feature importance analysis via regression coefficients
- Interpretability-driven modeling

### Prediction Objectives
- Predict HDI without using traditional HDI components
- Identify actionable development drivers
- Quantify impact of aid-influenceable variables
- Enable data-driven policy targeting
- Support evidence-based intervention planning

---

## Optimization Model

### Objective
Maximize predicted HDI impact through optimal allocation of international aid funding across health and infrastructure resources.

### Optimization Framework
- Method: Convex optimization (CVXPY)
- Decision variables: Resource allocation quantities
- Objective function: Weighted HDI impact maximization
- Weights: Regression coefficients (feature importance)
- Model type: Budget-constrained multi-resource optimization

### Constraints
- Total budget constraint (WHO Africa allocation)
- Maximum resource demand constraints
- Maximum funding share per resource (diversification constraint)
- Non-negativity constraints
- Scaled numerical stability constraints

### Resources Modeled
- Hepatitis B vaccines
- Measles vaccines
- Polio vaccines
- Diphtheria vaccines
- HIV/AIDS treatment
- Basic drinking water access
- Basic sanitation services
- Basic handwashing facilities

---

## Sensitivity Analysis
- Binding vs non-binding constraint detection
- Budget allocation sensitivity
- Demand saturation analysis
- Resource prioritization stability
- Policy robustness evaluation
- Allocation diversification behavior

---

## Methods & Tools
- Python
- NumPy
- Pandas
- Scikit-learn
- CVXPY
- Matplotlib
- Seaborn
- K-Fold Cross Validation
- Linear Regression
- Statistical Feature Selection
- Convex Optimization

---

## Results
- Accurate HDI prediction using alternative, aid-influenceable features
- Strong generalization performance across folds
- Interpretable feature importance structure
- Stable predictive performance
- Optimized funding allocation under real-world constraints
- Policy-relevant resource prioritization
- Data-driven aid strategy design

---

## Applications
- International development planning
- NGO funding strategies
- Government aid distribution
- Global health policy modeling
- Resource allocation systems
- Public sector optimization
- Development economics analytics
- Humanitarian logistics planning

---

## Author
Victoria Piroian  

University of Toronto  

Faculty of Applied Science & Engineering, 2022
