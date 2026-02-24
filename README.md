🔥 Calorie Expenditure Prediction using Ridge Regression

Predict how many calories you burn based on your health and activity metrics — powered by Ridge Regression.


📌 Overview

This project builds a machine learning pipeline to estimate calorie expenditure from physiological and exercise-related data. Ridge Regression is chosen for its ability to handle multicollinearity and prevent overfitting, making it well-suited for health datasets with correlated features.

📂 Dataset

The dataset contains health and activity records with features such as age, gender, height, weight, heart rate, body temperature, and exercise duration.

✨ Features

Data Preprocessing — Handles missing values, outliers, and data types
Normalization & Scaling — Standardizes features for optimal model performance
Feature Engineering — Creates meaningful derived features from raw data
Ridge Regression Model — Regularized linear model with tuned alpha parameter
Model Evaluation — RMSE, MAE, R² score, and residual analysis
Visualization — Actual vs. predicted plots and feature importance charts


🛠 Installation

bashgit clone https://github.com/your-username/calorie-expenditure-predictor.git
cd calorie-expenditure-predictor
pip install -r requirements.txt
Requirements include: pandas, numpy, scikit-learn, matplotlib, seaborn

🚀 Usage

Place your dataset in the data/raw/ directory.
Run the preprocessing script:

bash   python src/preprocess.py

Train and evaluate the model:

bash   python src/train.py

Or explore interactively via the notebook:

bash   jupyter notebook notebooks/calorie_prediction.ipynb

📊 Results

MetricScoreR² Score~0.98RMSELowMAELow
Ridge Regression demonstrated strong predictive performance, effectively capturing the relationship between physical activity features and calorie burn.

🧠 Model Insight

Ridge Regression adds an L2 penalty to the loss function, which shrinks coefficients and reduces variance — particularly useful when features like heart rate, duration, and weight are correlated.


📄 License
This project is licensed under the MIT License.
