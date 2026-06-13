# Asthma Control Score Prediction Using Machine Learning

## Overview

Asthma is a chronic respiratory condition influenced by environmental, behavioral, and demographic factors. This project aims to predict the **Asthma Control Test (ACT) Score** using machine learning techniques and structured healthcare data.

The project follows a complete machine learning pipeline, including data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning, and performance evaluation. Multiple regression algorithms were compared to identify the most effective model for predicting asthma control levels.

---

## Objectives

* Predict Asthma Control Test (ACT) scores from patient and environmental data.
* Compare the performance of multiple machine learning regression models.
* Identify the most influential factors affecting asthma control.
* Build an interpretable and reproducible machine learning workflow.

---

## Dataset

The dataset contains approximately **1,010 records** and includes:

### Demographic Features

* Age
* Gender
* Location

### Lifestyle Features

* Smoking Habit
* Outdoor Activities
* Outdoor Job Frequency

### Environmental Features

* Humidity
* Temperature
* Atmospheric Pressure
* Wind Speed
* UV Index

### Target Variable

* ACT Score (Asthma Control Test Score)

---

## Data Preprocessing

The following preprocessing steps were performed:

* Removal of identifier columns
* Duplicate record removal
* Outlier detection and filtering using the IQR method
* Categorical feature encoding
* Feature scaling and standardization
* Train-test data splitting

---

## Exploratory Data Analysis

The project includes:

* Statistical summaries
* Distribution analysis
* Boxplots
* Correlation heatmaps
* Feature importance analysis

These analyses help understand the relationships between environmental conditions and asthma control.

---

## Machine Learning Models Used

The following regression models were implemented and evaluated:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. K-Nearest Neighbors Regressor
5. Artificial Neural Network (MLP Regressor)

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter/Colab Notebook

---

## Evaluation Metrics

Models were evaluated using:

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* Cross Validation Score

---

## Results

| Model             | R² Score  | MAE       | RMSE      |
| ----------------- | --------- | --------- | --------- |
| Linear Regression | 0.756     | 1.913     | 2.365     |
| Decision Tree     | 0.921     | 0.505     | 1.346     |
| Random Forest     | **0.935** | **0.629** | **1.219** |
| KNN               | 0.821     | 1.351     | 2.027     |
| ANN               | 0.852     | 1.250     | 1.840     |

### Best Performing Model

**Random Forest Regressor**

Performance:

* R² Score: **0.935**
* MAE: **0.629**
* RMSE: **1.219**

---

## Key Findings

* Environmental factors significantly influence asthma control.
* Humidity and wind speed were among the most important predictive features.
* Ensemble learning methods outperformed traditional linear approaches.
* Random Forest provided the best balance between accuracy and interpretability.

---

## Future Improvements

* Integration of air quality and pollution data.
* Testing on larger healthcare datasets.
* Deployment as a web application.
* Implementation of XGBoost and LightGBM.
* Model explainability using SHAP values.

---

## Project Structure

```text
Asthma-Control-Score-Prediction/
│
├── data/
│   └── ASTHMA.csv
│
├── notebooks/
│   └── Asthma_Prediction.ipynb
│
├── images/
│   ├── heatmap.png
│   ├── feature_importance.png
│   └── model_comparison.png
│
├── report/
│   └── Project_Report.pdf
│
├── requirements.txt
│
└── README.md
```

---

## Author

**Vinay Kumar**

B.Tech Computer Science and Engineering
National Institute of Technology Uttarakhand

---

## License

This project is intended for educational and research purposes.
