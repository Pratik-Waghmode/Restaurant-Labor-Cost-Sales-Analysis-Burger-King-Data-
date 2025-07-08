# 🧾 Restaurant Labor Cost & Sales Analysis (Burger King Data)

This project demonstrates how to load, clean, analyze, and build a linear regression model to predict **labor cost** based on **sales and labor hours** in a fast-food restaurant scenario — inspired by real-world Burger King operations.

---

## 📁 Dataset
The dataset contains daily restaurant data for 2024 and includes the following key columns:
- `Date`: Transaction date
- `Net_Sales`: Total net sales for the day
- `Actual_Hours`: Total labor hours worked
- `Overtime`: Overtime hours
- `Cost_of_Labour`: Actual labor cost
- `Actual_Labor`: Labor as a percentage of sales
- `Purchased_Inventory`, `Waste`, `Theo_Use`, `Act_Use`, `Act_OnHand`: Inventory-related metrics


---

## 📊 Key Steps

### 1. **Data Cleaning & Preparation**
- Loaded data with `pandas`
- Renamed columns for consistency
- Converted `Date` to `datetime`
- Handled missing values by filling with `0`

### 2. **Exploratory Data Analysis (EDA)**
- Visualized:
  - **Net Sales over time**
  - **Labor % over time** (`Actual_Labor`)
- Tools used: `matplotlib` and `seaborn`

### 3. **Machine Learning Model (Linear Regression)**
- **Goal:** Predict `Cost_of_Labour` using:
  - Features: `Net_Sales`, `Actual_Hours`
- Split into train/test sets (80/20)
- Evaluated using:
  - `Mean Absolute Error (MAE)`
  - `R² Score`
- Visualized Actual vs Predicted labor costs


