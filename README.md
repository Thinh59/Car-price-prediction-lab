# 🚗 Car Price Prediction Lab
This repository contains the notebook and source code for the **Car Price Prediction Lab**.  
The main objective is to build a **Linear Regression model from scratch (without using sklearn)** to predict used car prices based on their technical features.

We are Group 9 in Class 23TNT1 at Ho Chi Minh City University of Science, specializing in Advanced Programming for Artificial Intelligence.

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
1. **Data Loading & Exploration**  
   - Display dataset size, column names, and first 5 rows.
2. **Preprocessing**  
   - Remove text from numerical columns (`Engine`, `Max Power`, …).  
   - Convert categorical values into numerical format (Label Encoding / One-hot Encoding).  
   - Select relevant columns for training.  
3. **Model Building**  
   - Implement Linear Regression **from scratch** (no sklearn).  
   - Define and test multiple regression formulas as required.  
4. **Evaluation**  
   - Compute R², MSE, and MAE on both training and test sets.

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
