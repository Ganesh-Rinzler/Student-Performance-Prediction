# Student Performance Prediction - ML Regression

This repository explores **predicting secondary-school students’ final grades** using a multivariate dataset of 649 records and 30 features.  
The project demonstrates how different regression algorithms perform on the same task and how hyperparameter tuning can significantly improve accuracy.

## Key Steps
- **Baseline Models**: Linear Regression, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, and Support Vector Regression (SVR) with various kernels.
- **Feature Engineering**: Data cleaning, scaling, and exploratory analysis.
- **Model Evaluation**: Train/test split with R² score as the main metric.

## Results
| Model                 | Best R² Score |
|-----------------------|--------------:|
| SVR (Linear kernel)   | **0.882** |
| SVR (RBF tuned)       | 0.862 |
| SVR (Polynomial)      | 0.712 |
| Linear Regression     | 0.868 |
| Random Forest         | 0.854 |
| Gradient Boosting     | 0.847 |
| AdaBoost             | 0.831 |
| Decision Tree         | 0.704 |

Feature selection with `SelectPercentile` and dimensionality reduction using PCA further improved the tuned SVR (RBF) to **≈0.877 R²**.
