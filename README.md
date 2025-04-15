# 🧠 Age Prediction from High-Dimensional Health Data

This project explores and compares various machine learning models to predict a person's age based on a large set of features related to health, behavior, and environment. The models include **Linear Regression with PCA**, **Neural Network**, **XGBoost**, and **LightGBM**.

---

## 📁 Dataset

The dataset contains over 1,500 features across approximately 2,600 observations. Features include clinical metrics (e.g., cholesterol level, BMI), behavioral data (e.g., sleep patterns, alcohol consumption), and environmental factors (e.g., pollution exposure). The target variable is `Age (years)`.

---

## 📊 Objective

To evaluate and compare the performance of multiple regression models in predicting age, and to assess the effectiveness of dimensionality reduction (PCA) in improving model accuracy and stability.

---

## 🧪 Models Compared

| Model                  | Preprocessing       | Avg MSE | Avg R² |
|------------------------|---------------------|---------|--------|
| Linear Regression      | PCA (50 components) | 30.20   | 0.92   |
| XGBoost                | Raw features        | 31.13   | 0.92   |
| LightGBM               | Raw features        | 32.44   | 0.91   |
| Neural Network         | Raw features        | 40.16   | 0.89   |

All scores are reported based on **5-fold cross-validation**.

---

## ⚙️ Technologies Used

- Python 3
- scikit-learn
- XGBoost
- LightGBM
- TensorFlow/Keras
- NumPy / Pandas / Matplotlib / Seaborn

---

## 🧠 Key Insights

- **Linear Regression with PCA** outperformed more complex models, demonstrating the power of dimensionality reduction on high-dimensional data.
- **XGBoost** and **LightGBM** delivered robust and consistent results, making them excellent choices for structured datasets.
- Neural networks performed well, though additional tuning or regularization might improve results.

---

## 📌 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/age-prediction-ml.git
   cd age-prediction-ml
2. (Optional) Create a virtual environment:
   python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install dependencies:
   pip install -r requirements.txt

## 📚 Author

Nour Jennane
Data Science & Health Analytics Enthusiast
📧 jennanenour@gmail.com
