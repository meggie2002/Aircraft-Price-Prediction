# ✈️ Aircraft Price Prediction - Multiple Linear Regression Model

![R](https://img.shields.io/badge/Language-R-276DC3)
![License](https://img.shields.io/badge/License-MIT-green)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-blue)
![Adjusted R²](https://img.shields.io/badge/Adjusted_R²-0.9248-success)

A multiple linear regression model to predict aircraft prices using technical specifications. Built for Data 603 Group Project.

---

## Table of Contents
- [Project Overview](#-project-overview)
- [Dataset](#-dataset)
- [Installation](#-installation)
- [Usage](#-usage)
- [Methodology](#-methodology)
- [Results](#-results)
- [Repository Structure](#-repository-structure)
- [Challenges](#-challenges)
- [Contributing](#-contributing)
- [Team](#-team)
- [References](#-references)
- [License](#-license)

---

## 📌 Project Overview

**Goal:**  
Predict aircraft prices using features like engine specifications, speed metrics, and wing span. Identify key drivers of pricing for aviation stakeholders.

**Key Achievements:**
- Achieved **92.48% explained variance** (Adj. R²) with interaction terms.
- Identified critical predictors: engine type, cruise speed, and wing span.
- Handled multicollinearity, heteroscedasticity, and outliers rigorously.

---

## 📊 Dataset

**Source:** [Kaggle Aircraft Dataset](https://www.kaggle.com/datasets/mehmet0sahinn/aircraft-price-analysis-and-prediction-dataset)  
**Size:** 518 aircraft records | **Features:** 14 quantitative + 2 qualitative

**Variables:**
| Type          | Key Features                                                                 |
|---------------|------------------------------------------------------------------------------|
| **Target**    | `Price` (USD)                                                               |
| **Predictors**| `engine_type` (Jet/Piston/Propjet), `engine_power` (hp), `cruise_speed` (knots), `wing_span` (inches), `range` (nautical miles) |


