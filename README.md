# 🏠 House Price Prediction — AI/ML Task 2
**Maincrafts Technology Internship**

Feature Engineering, Model Optimization & Performance Comparison using the California Housing Dataset.

---

## 📌 Objective
Build an enhanced ML pipeline that goes beyond basic model training by applying preprocessing, training multiple algorithms, and selecting the best model using measurable metrics.

---

## 📁 Files
| File | Description |
|------|-------------|
| `AI_ML_Task2_Model_Comparison.ipynb` | Full Jupyter Notebook (all steps) |
| `AI_ML_Task2_Report.pdf` | 2-page methodology & results report |
| `task2_performance.png` | 4-panel performance chart |
| `model_comparison.csv` | RMSE & R² results table |
| `best_model.pkl` | Saved Decision Tree model |
| `scaler.pkl` | Saved StandardScaler |

---

## 🛠️ Tech Stack
`Python` `pandas` `NumPy` `scikit-learn` `matplotlib` `joblib` `Jupyter Notebook`

---

## ⚙️ Steps Implemented
1. Load the California Housing Dataset (20,640 samples)
2. Exploratory data analysis — no missing values found
3. Separate features (X) and target (y = HousePrice)
4. Feature scaling with `StandardScaler` → mean=0, std=1
5. Train/test split — 80% train / 20% test (`random_state=42`)
6. Train 3 models: Linear Regression, Ridge Regression, Decision Tree
7. Evaluate with RMSE and R² Score
8. Visual validation — Actual vs Predicted & residual plots
9. Save best model with `joblib`

---

## 📊 Model Performance

| Model | RMSE | R² Score |
|-------|------|----------|
| Linear Regression | 0.5940 | 0.7929 |
| Ridge Regression | 0.5940 | 0.7929 |
| **Decision Tree** ✅ | **0.5121** | **0.8461** |

**Selected model:** Decision Tree Regressor (`max_depth=5`)  
**Reason:** Lowest RMSE and highest R² — captures non-linear relationships between income, location, and house prices that linear models miss.

---

## 🚀 How to Run
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
pip install -r requirements.txt
jupyter notebook AI_ML_Task2_Model_Comparison.ipynb
```

---

## 📄 License
MIT — free to use for learning and portfolio purposes.
