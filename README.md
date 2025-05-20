# Aircraft Price Prediction - Multiple Linear Regression Model 

A robust multiple linear regression model in **R** to predict aircraft prices using technical specifications. 

---

## Project Overview

**Goal:**  
Predict aircraft prices using features such as engine type, engine power, speed, and wing span. Identify key pricing drivers for aviation stakeholders.

**Key Achievements:**
- Achieved **92.5% explained variance** (Adj. R²) with interaction terms.
- Identified critical predictors: engine type, cruise speed, and wing span.
- Rigorous handling of multicollinearity, heteroscedasticity, and outliers.

---

## Dataset

**Source:** [Kaggle Aircraft Dataset](https://www.kaggle.com/datasets/mehmet0sahinn/aircraft-price-analysis-and-prediction-dataset)  
**Records:** 517 aircraft (after cleaning)  
**Features:** 14 quantitative + 2 qualitative

**Variables:**

| Type          | Key Features                                                                 |
|---------------|------------------------------------------------------------------------------|
| **Target**    | `price` (USD)                                                                |
| **Predictors**| `engine_type` (Jet/Piston/Propjet), `engine_power` (hp), `cruise_speed` (knots), `wing_span` (inches), `range` (nautical miles), etc. |

---

## Usage

### 1. Open R or RStudio

### 2. Install required packages

```r
install.packages(c("tidyverse", "car", "MASS", "broom", "GGally"))
```

### 3. Run the analysis

- Oopen and execute the RMarkdown notebook:  
  `Aircraft_Price_Prediction.Rmd`

---

## Methodology

- **Data Cleaning:** Removed missing values, standardized units, and encoded categorical variables.
- **EDA:** Visualized relationships, checked for outliers.
- **Feature Engineering:** Created interaction terms.
- **Modeling:** Built multiple linear regression models with stepwise selection.
- **Diagnostics:** Checked multicollinearity (VIF), heteroscedasticity, and outliers.

---

## Results

- **Best Model:**  
  ```
  price ~ factor(engine_type) + engine_power + max_speed + cruise_speed + stall_speed +
          all_eng_roc + out_eng_roc + takeoff_distance + wing_span + range
  ```

- **Adjusted R²:** **0.9248**  
- **Key Predictors:** Engine type, cruise speed, wing span

- **Main Effects of Engine Type:**
    - **Piston:** Aircraft with a piston engine are, on average, **$4.4 million cheaper** than jets (holding other variables constant).
    - **Propjet:** Aircraft with a propjet engine are **$2.8 million cheaper** than jets.

- **Model Diagnostics:**  
  - Multicollinearity managed (VIF mostly < 5)
  - Residuals checked for normality and equal variance

---

## Repository Structure

```
.                  
├── notebook/                  
│   └── Aircraft_Price_Prediction.Rmd # RMarkdown notebook
├── README.md
└── .gitignore
```

---

## Challenges

- Handling missing and inconsistent data
- Addressing multicollinearity among predictors
- Managing outliers and influential points

---


## Team

- Anitha Joseph
- Jincy Thomas
- Joshua Quartey
- Megha Radhakrishnan Sanitha
- Prichelle Lal
- Riya Chevli


