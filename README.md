# 🚖 Taxi Price Prediction using Machine Learning

## 📘 Project Overview
This project aims to **accurately estimate taxi trip fares** using a **Linear Regression model** trained on structured trip data.  
The model leverages multiple trip-related attributes such as **distance**, **duration**, **traffic conditions**, **weather**, and **rate components** to predict the **total trip price**.  
The goal is to assist taxi companies and customers with **fare transparency**, **dynamic pricing**, and **trip cost estimation**.

---

## 📊 Dataset Description

The dataset consists of trip-level details that influence fare amount.  
Below is a summary of the features used in model training:

| Column | Description |
|---------|--------------|
| Trip_Distance_km | Total trip distance in kilometers |
| Time_of_Day | Categorical feature representing when the trip occurred (Morning, Afternoon, Evening, Night) |
| Day_of_Week | Indicates whether the trip happened on a weekday or weekend |
| Passenger_Count | Number of passengers during the trip |
| Traffic_Conditions | Traffic intensity level such as Low, Medium, or High |
| Weather | Weather condition during the trip (e.g., Clear, Rain, Snow) |
| Base_Fare | Initial fare charged at the start of the trip |
| Per_Km_Rate | Fare rate applied per kilometer traveled |
| Per_Minute_Rate | Fare rate applied per minute of trip duration |
| Trip_Duration_Minutes | Total trip duration in minutes |
| Trip_Price | Target variable representing the total fare |

---

## ⚙️ Workflow

### 1️⃣ Data Visualization
Performed exploratory analysis and visualizations to understand feature relationships:
- **Correlation Matrix** → Identified multicollinearity between variables  
- **Distribution & Pair Plots** → Explored patterns in distance, duration, and price  

### 2️⃣ Data Preprocessing
- Loaded and cleaned the dataset (handled **missing** and **invalid** entries)  
- Applied **encoding** to categorical features (e.g., traffic, weather, time of day)  
- Used **scaling/normalization** for continuous variables to improve model stability  

### 3️⃣ Model Evaluation
- Split dataset into **training and testing sets**  
- Trained a **Linear Regression** model using Scikit-learn  
- Evaluated using regression metrics:
  - **Mean Absolute Error (MAE)**
  - **Mean Squared Error (MSE)**
  - **R² Score**
- Visualized **actual vs predicted fares** to assess prediction accuracy

---

## 🧾 Result Summary

| Metric | Value |
|---------|--------|
| Mean Squared Error (MSE) | 194.72 |
| R-squared (R²) | 0.765 |

✅ The model achieved a **R² = 0.76**, indicating strong correlation between predicted and actual fares.  
Optimized feature scaling and encoding pipelines further improved consistency and performance.

---

## 🧩 Technologies Used

| Category | Tools / Libraries |
|-----------|-------------------|
| Programming Language | Python 3.8+ |
| Data Handling | pandas, numpy |
| Data Visualization | matplotlib, seaborn |
| Machine Learning | scikit-learn |
| Environment | Jupyter Notebook |

---

## 🚀 Installation & Usage

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/AShr12xz/Taxi-Price-Prediction.git
cd Taxi-Price-Prediction
