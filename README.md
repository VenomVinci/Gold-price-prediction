---

# 📈 Gold Price Prediction Using Random Forest Regressor

A machine learning project focused on predicting daily gold prices using historical market data.
The model is built using a **Random Forest Regressor** and achieves an accuracy of **~98%**, demonstrating strong predictive performance.

---

## 🗂️ Dataset

This project uses publicly available historical gold price data from Kaggle:

* **Dataset:** Gold Price Data
* **Source:** Kaggle
* **Link:** (Kaggle – Gold Price Data)
  *(Dataset reference: “altruistdelhite04/gold-price-data”)*

The dataset includes daily values for gold prices and related market indicators such as Silver Price, USD/INR, Oil Price, etc.

---

## 🔧 Project Workflow

### 1. **Data Collection**

The dataset was downloaded from Kaggle and imported into the notebook for exploration and preparation.

### 2. **Data Preprocessing**

* Handling missing values
* Converting dates into a usable datetime format
* Removing irrelevant or redundant columns
* Scaling/normalizing numerical features where necessary

### 3. **Feature Engineering**

* Extracted additional time-based features (e.g., year, month, day)
* Created lag features to capture historical behavior
* Selected the most significant predictors using feature importance

### 4. **Train–Test Split**

* Stratified or chronological split depending on time-series constraints
* Ensured no data leakage across training and testing sets

### 5. **Model Building**

A **Random Forest Regressor** was used due to its robustness, ability to handle non-linear patterns, and high performance on structured/tabular data.

Hyperparameters tuned include:

* Number of estimators
* Maximum depth
* Minimum samples per split/leaf
* Bootstrap settings

### 6. **Model Evaluation**

The model was evaluated using:

* R² Score
* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)

**Final performance:**

> 🟢 **Accuracy (R²): ~98%**

This indicates that the model successfully captures the underlying relationships in the data and is highly effective at predicting gold prices.

---

## 📊 Results

* High accuracy and low error rates
* Key features identified included gold price trends, oil price, USD/INR exchange rate, and silver price
* Predictions closely follow actual values with minimal deviation

> The model demonstrates that ensemble methods like Random Forest are highly reliable for financial time-series regression tasks.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib / Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/gold-price-prediction.git
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook or Python script:

   ```bash
   jupyter notebook
   ```

---

## 📌 Future Improvements

* Integrate advanced models (XGBoost, LSTM for time-series forecasting)
* Hyperparameter optimization using Optuna or Bayesian search
* Deploy model via a web app (Streamlit / FastAPI)
* Add live price tracking and real-time predictions

---
