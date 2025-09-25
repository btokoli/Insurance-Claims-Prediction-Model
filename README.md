# 💡 Insurance Claims Prediction Model

This project builds a **machine learning regression model** to predict **insurance claim amounts** based on demographic and lifestyle factors. By analyzing structured insurance data, the model provides insights into the key drivers of healthcare costs and helps insurers make data-driven decisions.

> **Highlight:** Gradient Boosting achieved strong predictive performance with a **low MSE** and high **R²**, accurately capturing the effect of smoking status, BMI, and region on claim costs.

---

## 📁 Repository Structure

```
Insurance-Claims-Prediction-Model/
├─ data/                        # Insurance dataset (CSV)
├─ notebooks/
│   ├─ preprocessing.ipynb       # Data cleaning & encoding
│   ├─ eda.ipynb                 # Exploratory data analysis
│   ├─ models.ipynb              # Regression models & evaluation
│   └─ tuning.ipynb              # Hyperparameter optimization
├─ results/
│   ├─ model_metrics.csv
│   └─ figures/                  # Plots (distributions, feature importance)
└─ README.md
```

---

## 🔧 Environment & Dependencies

Use Python 3.9–3.11. Install requirements with:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

---

## 📊 Dataset

- **Source:** Synthetic/educational insurance dataset  
- **Size:** 1,340 records  
- **Features:**
  - `age` – Age of insured person  
  - `gender` – Male/Female  
  - `BMI` – Body Mass Index  
  - `children` – Number of children covered  
  - `smoker` – Yes/No  
  - `region` – Northeast, Northwest, Southeast, Southwest  
  - `diabetic` – Yes/No  
- **Target:**
  - `claim` – Insurance claim amount (USD)  

---

## 🧹 Preprocessing

- Handled missing values and outliers  
- Applied **one-hot encoding** for categorical variables  
- Standardized numerical features using **StandardScaler**  
- Split into **train/test sets** for evaluation  

---

## 🧠 Methodology

1. **Exploratory Data Analysis (EDA)**
   - Distribution of claim amounts  
   - Correlations between demographic/lifestyle factors and claims  

2. **Model Training**
   - Linear Regression  
   - Random Forest Regression  
   - Gradient Boosting Regression  

3. **Model Evaluation**
   - Metrics: **MSE, RMSE, R²**  
   - Visual comparisons of predicted vs actual claims  

4. **Hyperparameter Tuning**
   - GridSearchCV applied to Gradient Boosting for optimization  

---

## ✅ Results & Insights

- **Key Drivers of Claims:**
  - **Smoking status** → strongest predictor of higher claims  
  - **Region** → significant geographic variation  
  - **BMI** → positive correlation with claim amount  
  - **Age** → moderate effect on costs  

- **Model Performance:**
  - Gradient Boosting delivered the **best balance of accuracy and interpretability**  
  - Low MSE and high R² indicated strong predictive power  

---

## 📈 Visualizations

- Claim distribution histograms  
- Feature importance plots  
- Predicted vs actual claim scatter plots  

---

## 🗺️ Roadmap / Future Work

- Expand dataset with larger real-world samples  
- Add interaction effects (e.g., smoker × age × BMI)  
- Experiment with **XGBoost / LightGBM** for improved accuracy  
- Deploy as a **web app API** for real-time prediction  

---

## 📚 References

- [Scikit-learn Documentation](https://scikit-learn.org/stable/)  
- Health insurance cost modeling research papers  
- Gradient Boosting for regression tasks  

---

## ⚖️ License

No explicit license provided. If open-sourcing, consider MIT or Apache-2.0.

---

## 🙏 Acknowledgments

Developed by **Bismack Tokoli** as part of an applied data science project in predictive modeling.
