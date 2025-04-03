# Flight-Price-Prediction-using-Machine-Learning


## 📌 Overview
This project aims to predict airline ticket prices using Machine Learning. By analyzing various factors such as airline type, number of stops, departure/arrival times, and flight duration, the model provides an estimated price for a given flight.

---

## 📂 Dataset
- **Source**: Kaggle Flight Price Dataset
- **Features Used**:
  - ✈️ `Airline` - Type of airline
  - 🌍 `Source` & `Destination` - Departure and arrival locations
  - ⏳ `Total_Stops` - Number of layovers
  - 🕒 `Duration` - Total travel time (converted into minutes)
  - 📅 `Date_of_Journey` - Extracted day, month, and weekday  
- **Preprocessing Steps**:
  - Removed missing values
  - Encoded categorical variables (`Airline`, `Source`, `Destination`)
  - Converted `Total_Stops` from text (e.g., *"non-stop"*) into numerical values  
  - Used **Chi-Square test** to determine feature importance  

---

## 🏗️ Model Training
- Used `train_test_split` with **80% training & 20% testing**  
- Implemented **Random Forest Regressor** for price prediction  


## 📊 Evaluation Metrics

The model's performance was evaluated using the following metrics:

| Metric | Description | Value |
|--------|------------|--------|
| **R² Score** | Measures how well the model fits the data (closer to 1 is better) | **74%** |
| **Mean Absolute Error (MAE)** | Measures the average absolute error between actual and predicted prices | **21%** |
| **Root Mean Squared Error (RMSE)** | Penalizes larger errors more heavily (lower is better) | **26.25%** |



