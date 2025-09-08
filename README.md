# 🚗 Car Price Prediction Lab
This repository contains the notebook and source code for the **Car Price Prediction Lab**.  
The main objective is to build a **Linear Regression model from scratch (without using sklearn)** to predict used car prices based on their technical features.

We are Group 9 in Class 23TNT1 at Ho Chi Minh City University of Science.

We are excited to share our work with you and look forward to your feedback.
Best regards from Group 9!

---

## 📊 Dataset
- Source: `train.csv`
- Features (X):
  - Make, Model, Year, Kilometer, Fuel Type, Transmission, Location, Color, Owner, Seller Type, Engine, Max Power, Max Torque, DriveTrain, Length, Width, Height, Seating Capacity, Fuel Tank Capacity.
- Target (Y): Selling Price.

---

## 🛠 Workflow  

1. **Data Processing**  
   - Load and inspect dataset (size, columns, first rows).  
   - Handle unit inconsistencies in numerical columns.  
   - Process missing values.  
   - Remove low-variance categorical columns.  
   - Encode categorical features into numerical format (Label Encoding / One-hot Encoding).  

2. **Feature Selection**  
   - Build correlation matrix to analyze relationships between features and target.  
   - Visualize correlation heatmap.  
   - Remove features with low correlation.  
   - Update dataset and assign values into **X** (features) and **Y** (target).  

3. **Data Splitting**  
   - Apply **K-Fold Cross-Validation** for robust model evaluation.  
   - Randomly shuffle and partition dataset into K folds.  
   - Ensure equal fold sizes for training and validation.  

4. **Model Training**  
   - Explore correlations between features and target variable.  
   - Define and implement multiple regression formulas.  
   - Standardize features before training.  
   - Construct feature matrix and target vector.  
   - Implement **Normal Equation** with Ridge Regression (from scratch).  
   - Train and evaluate models with cross-validation.  
   - Summarize training results.  

5. **Model Testing**  
   - Load and preprocess test set in the same way as training set.  
   - Standardize test features.  
   - Predict car prices using trained linear regression model.  
   - Handle dimensionality mismatches if any.  
   - Evaluate model performance on test set (R², MSE, MAE).  


---

## 📈 Results
- **R² (Train):** 0.9370  
- **R² (Test):** 0.9179  
- **MAE (Train):** 296,323.48  
- **MAE (Test):** 365,041.95  

Compared to previous models (R² ~0.89, MAE > 420k), this is a clear improvement.  
The model learns features effectively and generalizes well to unseen data.

---

## 🚀 How to Run
```bash
# Install dependencies
pip install -r requirements.txt

# Launch notebook
jupyter notebook notebooks/CarPricePrediction.ipynb
