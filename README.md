🚗 Toyota Corolla — Used Car Price Prediction (Regression)

  This project aims to implement a complete Machine Learning regression pipeline on a real dataset containing Toyota Corolla used cars.
The goal is to predict the selling price of a vehicle based on the three most impactful numeric features:
  -  Age (years)
  -  KM (mileage - km)
  -  Weight (vehicle weight - kg)

Even though the dataset is simple and clean (no missing values, no categorical encoding required), it allows building a highly effective and well-structured regression project suitable for a professional ML portfolio.

📚 Step 1. Dataset Description

The dataset contains real Toyota Corolla listings.

Characteristics:

  -  No missing values
  -  No duplicates
  -  All features numeric
  -  No categorical encoding needed
  -  Strong linear relationships with the target (Price)

This dataset is ideal for:

  -  Learning regression techniques
  -  Comparing linear vs. ensemble models
  -  Showing a clean but realistic ML workflow

📊📉 Step 2. Exploratory Data Analysis (EDA)

Correlations:

The strongest correlations with Price:

  -  Age → strongly negative
  -  KM → negative
  -  Weight → weak-to-moderate positive

Data distributions

  -  All features follow near-normal or slightly skewed distributions — suitable for both linear and non-linear models.

✨ Step 3. Data Preprocessing

Minimal preprocessing was required:

  -  Train–test split
  -  Standardization using StandardScaler (for linear and polynomial models)
  -  No encoding (all features numeric)
  -  No imputation needed

The dataset is exceptionally clean and modelling-ready.

🦾 Step 4. Regression Models Implemented

The project includes a full comparison between traditional and ensemble algorithms:

  🔵 4.1. Linear Regression (Baseline)

    RMSE ≈ 1495
    R2 ≈ 0.83

A strong baseline given the linear structure of the data.

  🔵 4.2. Ridge Regression

Similar to baseline → regularization doesn’t add value due to balanced features.

  🔵 4.3. Lasso Regression

Same behavior as Ridge — no coefficients removed; dataset is too simple.

  🔵 4.4. Polynomial Regression (Degrees 1–4)

    Degree 2: RMSE ≈ 1164, R2 ≈ 0.90
    Degree 3: slight overfitting
    Degree 4: severe overfitting (R2 ≈ -10)

Best polynomial model: Degree 2

  🔵 4.5. Random Forest Regressor

    RMSE ≈ 1118
    R2 ≈ 0.91

Strong performance — better than all linear models.

  🔵 4.6. Gradient Boosting Regressor

    RMSE ≈ 1022
    R2 ≈ 0.922

📌 Best performing model overall.

  🔵 4.7. Extreme Gradient Boosting (XGBoost)

    RMSE ≈ 1041
    R2 ≈ 0.918

Very strong model, slightly behind Gradient Boosting.


🏆 Step 5. Final Performance Comparison

  | Model                 | RMSE     | R2        |
| --------------------- | -------- | --------- |
| Linear Regression     | 1495     | 0.83      |
| Ridge                 | 1495     | 0.83      |
| Lasso                 | 1495     | 0.83      |
| Polynomial (deg 2)    | 1164     | 0.90      |
| Random Forest         | 1118     | 0.91      |
| **Gradient Boosting** | **1022** | **0.922** |
| XGBoost               | 1041     | 0.918     |

Gradient Boosting achieved the best performance.


📈 Conclusions

This project demonstrates:

  -  Correct regression workflow
  -  Comparison between linear, regularized, polynomial, and ensemble models
  -  How simple features can still produce high predictive accuracy
  -  Clear improvement when moving from linear → polynomial → boosting algorithms

Gradient Boosting obtained the best results, offering a great balance between bias and variance.

🛠 How to Run the Project

git clone [https://github.com/Ctrl-Shift-Rem/Regression_Toyota-Corolla](https://github.com/Ctrl-Shift-Rem/Regression_Task_Toyota-Corolla).git
cd Regression_Toyota-Corolla

# Open the notebook
jupyter notebook Regression_task_Toyota.ipynb

Or open directly in Google Colab.

🌐 Contact

Feel free to connect or reach out:

GitHub: https://github.com/Ctrl-Shift-Rem

LinkedIn: https://linkedin.com/in/remus-rafael-cristea
