# 🚀 Boosting Algorithms Comparison  

This repository contains experiments comparing three popular **Boosting techniques** — **AdaBoost**, **Gradient Boosting**, and **XGBoost** — on both **classification** and **regression** problems using well-known inbuilt datasets.  

---

## 📂 Datasets Used  

1. **Digits Dataset (Classification)**  
   - Inbuilt `sklearn` dataset  
   - 1,797 samples of 8×8 grayscale images of digits (0–9)  
   - 64 pixel features per sample  

2. **California Housing Dataset (Regression)**  
   - Inbuilt `sklearn` dataset  
   - 20,640 samples  
   - 8 numerical features (e.g., MedInc, HouseAge, AveRooms, Latitude, Longitude, etc.)  
   - Target: Median house value  

---

## ⚙️ Methods  

- Data preprocessing:  
  - Feature scaling (`StandardScaler`)  
  - Train-test split (stratified for classification)  
- Models trained:  
  - `AdaBoostClassifier` / `AdaBoostRegressor`  
  - `GradientBoostingClassifier` / `GradientBoostingRegressor`  
  - `XGBClassifier` / `XGBRegressor`  
- Evaluation using classification and regression metrics  

---

## 📊 Results  

### 🔹 Digits Dataset (Classification)  

| Model              | Accuracy | Key Observations |
|---------------------|----------|------------------|
| **AdaBoost**        | 48.6%    | Poor performance, struggles with high-dimensional image data |
| **Gradient Boosting** | 95.5% | Strong performance, balanced precision & recall |
| **XGBoost**         | 96.1%    | Best overall accuracy, slightly better than Gradient Boosting |

✅ **Conclusion**: For handwritten digit recognition, **Gradient Boosting** and **XGBoost** clearly outperform AdaBoost, achieving ~96% accuracy.  

📌 *Visuals:*  
- Confusion matrices  
- Accuracy comparison bar chart  

---

### 🔹 California Housing Dataset (Regression)  

| Model              | MAE   | RMSE  | R²    | Key Observations |
|---------------------|-------|-------|-------|------------------|
| **AdaBoost**        | 0.65  | 0.78  | 0.53  | Weak performance, underfits |
| **Gradient Boosting** | 0.37 | 0.54 | 0.77 | Much stronger, good fit |
| **XGBoost**         | 0.31  | 0.47  | 0.83  | Best performer, lowest error |

✅ **Conclusion**: For housing price prediction, **XGBoost** is the most accurate with lowest MAE/RMSE and highest R² score.  

📌 *Visuals:*  
- Actual vs Predicted scatterplots  
- Bar plot comparing MAE/RMSE across models  


---

## 🛠️ Tech Stack  

- Python 3.x  
- Libraries:  
  - `scikit-learn`  
  - `xgboost`  
  - `matplotlib`, `seaborn`  
  - `numpy`, `pandas`  

---

## 📌 Conclusions  

- **AdaBoost** is less effective on complex datasets but works as a baseline.  
- **Gradient Boosting** provides strong performance with minimal tuning.  
- **XGBoost** consistently outperforms the others in both classification and regression, showing its efficiency and robustness.  

---

## 🔮 Future Work  

- Hyperparameter tuning with GridSearchCV / RandomizedSearchCV  
- Try **LightGBM** and **CatBoost** for comparison  
- Extend to more real-world datasets  

---

## 👤 Author  

**Jenil Gandhi**  
📌 Exploring Machine Learning & Data Science  
📌 Building projects on boosting techniques & ensemble models  

---
