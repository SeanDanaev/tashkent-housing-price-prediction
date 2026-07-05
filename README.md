# 🏠 Tashkent Housing Price Prediction

Predicting residential property prices in Tashkent, Uzbekistan using machine learning.  
Dataset: 7,565 entries × 7 features (local Tashkent housing market data)

---

## 📌 Project Overview

Real estate pricing in Tashkent is influenced by a mix of location, size, and infrastructure factors.  
This project builds and compares regression models to predict housing prices, following a full ML pipeline from raw data to saved model.

---

## 🔧 Tools & Libraries

- **Python** — Pandas, NumPy
- **Visualization** — Matplotlib, Seaborn
- **Modeling** — Scikit-learn (Linear Regression, Random Forest Regressor)
- **Evaluation** — RMSE, Cross-Validation

---

## 📊 Workflow

1. Data loading and exploration
2. Data cleaning and preprocessing
3. Exploratory Data Analysis (EDA) with visualizations
4. Feature preparation
5. Model training — Linear Regression and Random Forest
6. Model evaluation and comparison
7. Model export (saved as file)

---

## 📈 Results

| Model | RMSE |
|---|---|
| Linear Regression | 10,617 |
| Random Forest Regressor | 9,603 |
| Random Forest (Cross-Validation) | 9,827 |

Random Forest outperformed Linear Regression and was selected as the final model.

---

## 💡 Key Takeaways

- Random Forest reduced RMSE by ~9% compared to Linear Regression
- Cross-validation confirmed the model generalizes well beyond the training set
- - The `level` (floor) column showed the lowest correlation with price among all features,
  yet it may carry hidden significance: in Tashkent's housing market, floor level likely
  interacts with elevator availability — a top-floor unit without an elevator could see a
  meaningful price drop, while the same unit with an elevator may command a premium.
  This interaction was not captured in the raw feature and points to a valuable direction
  for future feature engineering.
- Two new features were engineered from existing columns. Despite showing negative
  correlation with price, they were retained as potentially informative signals —
  negative correlation still carries predictive value in a regression context.

---

## 🚀 How to Run

1. Clone this repository
2. Open `tashkent_housing_price_prediction.ipynb` in Jupyter or Google Colab
3. Run all cells in order
