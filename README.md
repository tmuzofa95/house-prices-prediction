# House Prices Prediction - Machine Learning

**Author:** Matthew Muzofa

---

## 📌 Project Overview

This project demonstrates machine learning skills by building a Linear Regression model to predict house prices. The model was trained on historical house data and achieved an R² score of **0.8844**, meaning it explains 88.44% of the variation in house prices. This project showcases the complete machine learning pipeline from data exploration through model evaluation and visualization.

---

## 🗃️ Dataset

- **Source:** [Kaggle - House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
- **Training Data:** 1,460 houses with 81 features
- **Test Data:** 1,459 houses for predictions
- **Features Include:** Square footage, number of bedrooms, garage size, quality ratings, year built, and more
- **Target:** Sale price of the house

---

## 🛠️ Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| Python | Programming language |
| Python (Pandas) | Data cleaning and preprocessing |
| Scikit-learn | Machine learning model building |
| Matplotlib & Seaborn | Data visualization |
| Jupyter Notebook | Python development environment |
| Kaggle | Dataset source |

---

## 🔄 Machine Learning Pipeline

```
Raw Data (Kaggle)
      ↓
Data Exploration & Analysis
      ↓
Data Cleaning & Preprocessing
      ↓
Feature Engineering (Convert categorical to numeric)
      ↓
Train/Validation Split (80/20)
      ↓
Model Training (Linear Regression)
      ↓
Model Evaluation & Visualization
      ↓
Predictions on Test Data
```

---

## 🧹 Data Cleaning Steps

- Dropped columns with >50% missing values
- Filled remaining missing values:
  - Numeric columns: Filled with median value
  - Categorical columns: Filled with mode (most common value)
- Converted all categorical columns to numeric using one-hot encoding
- Aligned training and test datasets to have matching features

---

## 📊 Model Performance

| Metric | Value | Interpretation |
|--------|-------|-----------------|
| **R² Score** | 0.8844 | Model explains 88.44% of price variation |
| **RMSE** | $29,773.44 | Average prediction error is ~$30k |

**Performance Assessment:** This is strong performance for a beginner machine learning model. The model successfully identifies patterns in house features that correlate with price.

---

## 📈 Visualisations Included

| Chart | Description |
|-------|-------------|
| actual_vs_predicted.png | Scatter plot comparing actual vs predicted prices. Points close to the red diagonal line indicate accurate predictions |
| residuals_plot.png | Shows prediction errors (residuals). Points scattered around zero indicate a well-balanced model |

---

## 📁 File Structure

```
house-prices-prediction/
│
├── house_prices_prediction.ipynb      # Complete machine learning notebook
├── house_prices_cleaned.csv           # Cleaned dataset after preprocessing
├── house_prices_predictions.csv       # Model predictions on test data
├── actual_vs_predicted.png            # Model accuracy visualization
└── residuals_plot.png                 # Prediction errors visualization
```

---

## 🚀 How to Reproduce

1. Download the dataset from Kaggle (link above) and save train.csv and test.csv
2. Place them in the same folder as the notebook
3. Open house_prices_prediction.ipynb in Jupyter Notebook
4. Run all cells in order
5. The model will train and generate predictions and visualizations

---

## 💡 Key Learnings

- Data preprocessing is critical — cleaning and preparing data took more effort than building the model itself
- Feature engineering matters — converting categorical variables to numeric format was essential for the algorithm
- Model evaluation is important — RMSE and R² score help understand model performance in real business terms
- Visualization reveals insights — the actual vs predicted plot clearly shows where the model performs well and where it struggles

---

## 🔑 Machine Learning Concepts Used

| Concept | What it means |
|---------|--------------|
| Linear Regression | Algorithm that finds the best-fit line through data points to predict continuous values |
| Train/Test Split | Dividing data into a training set (to learn patterns) and a test set (to evaluate performance) |
| Features | Input variables (house characteristics) used to make predictions |
| Target | The output variable we're trying to predict (sale price) |
| RMSE | Root Mean Squared Error — measures average prediction error in the same units as target |
| R² Score | Coefficient of determination — explains what percentage of variation the model captures (0-1) |

---
