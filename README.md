# ElevateLabs_AI-ML_TASK-03
**Housing Price Prediction Using Linear Regression Models**

---

## 🎯 Objective  
The objective of this task was to implement **Linear Regression models** to predict housing prices based on various features.  
While **Simple Linear Regression** and **Multiple Linear Regression** were **mandatory**, **Polynomial Regression** and **Ridge Regression** were included optionally to explore model performance and regularization effects.

---

## 📁 Dataset  
- **Name**: Housing Price Prediction Dataset  
- **Source**: [Kaggle - Housing Price Prediction](https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction)  
- **File Used**: `Housing.csv`

---

## 🚀 Steps Performed

### 1. Data Loading & Inspection  
- Loaded dataset using `pandas`  
- Checked for missing values and handled them

### 2. Data Preprocessing  
- Dropped missing rows  
- Applied One-Hot Encoding for categorical features:
  - `furnishingstatus`, `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`

---

## ✅ Mandatory Models

### 🔹 Simple Linear Regression  
- Feature used: `area`  
- Evaluated using MAE, MSE, and R² Score  
- Visualized regression line

### 🔹 Multiple Linear Regression  
- Used all encoded and numeric features  
- Trained and evaluated using scikit-learn  
- Visualized predicted vs actual prices

---

## 🆗 Optional Enhancements

### 🔸 Polynomial Regression  
- Applied `PolynomialFeatures` (degree = 1 for baseline, could extend to higher degrees)  
- Scaled features using `StandardScaler`  
- Evaluated performance and plotted predictions

### 🔸 Ridge Regression (Regularized Linear Regression)  
- Used `Ridge` with `alpha = 1.0`  
- Helps reduce overfitting using L2 regularization  
- Evaluated and visualized predictions

---

## 📈 Visual Results

| Model                      | Visualization                             |
|---------------------------|-------------------------------------------|
| Simple Linear Regression  | ![Simple](Simple%20Linear%20Regression.png) |
| Multiple Linear Regression| ![Multiple](Multiple%20Linear%20Regression.png) |
| Polynomial Regression     | ![Polynomial](Polynomial%20Regression.png) |
| Ridge Regression          | ![Ridge](Ridge%20Regression.png)  |

---

## 🛠 Tools & Libraries Used

- Python  
- Jupyter Notebook  
- Pandas, NumPy  
- Matplotlib  
- scikit-learn

---

## 📊 Evaluation Metrics Used

- **MAE**: Mean Absolute Error  
- **MSE**: Mean Squared Error  
- **R² Score**: Coefficient of Determination  

---

## 🔍 Model Performance Comparison
Among the four models tested, **Simple Linear Regression** performed the worst, showing the **highest error and lowest R² score**.
**Multiple Linear Regression**, **Polynomial Regression**, and **Ridge Regression** all gave very **similar results with much lower errors and higher accuracy**.
**Ridge Regression** slightly outperformed the others with the **lowest Mean Absolute Error**, indicating it is **more robust** and a better choice for this dataset.

Overall, **Ridge Regression** is recommended for more reliable predictions on this housing price data.

---
