# 🚖 Taxi Trip Price Prediction

## 📌 Project Overview
Predicting taxi trip prices using various machine learning models, including **Linear Regression, Ridge, Lasso, Random Forest, and Gradient Boosting**. The dataset contains trip-related details such as distance, duration, traffic conditions, and weather.

## 📂 Dataset
The dataset consists of:
- **Categorical Features:** Time of Day, Day of Week, Traffic Conditions, Weather
- **Numerical Features:** Trip Distance, Passenger Count, Base Fare, Per Km Rate, Per Minute Rate, Trip Duration, Trip Price (Target)

## 🚀 Project Workflow

### 1️⃣ Importing Libraries
Essential libraries for data handling, visualization, and machine learning are imported.

### 2️⃣ Loading the Dataset
Dataset is read using **pandas**.

### 3️⃣ Data Exploration
Basic exploration is performed using:
- `.head()`, `.tail()`, `.shape()`, `.info()`, `.describe()`, and `.isnull().sum()`

### 4️⃣ Handling Missing Values
- **Categorical Data:** Filled with mode.
- **Numerical Data:** Filled with median.

### 5️⃣ Data Visualization
- Countplot for **trips by time of day**
- Violin plot for **trip price by weather**
- Line plot for **trip price vs. duration (Traffic conditions)**
- Heatmap for **feature correlation**

### 6️⃣ Encoding Categorical Variables
Label Encoding is applied to categorical features for ML compatibility.

### 7️⃣ Splitting Data
Data is split into **80% training** and **20% testing**.

### 8️⃣ Feature Scaling
Standardization is applied using `StandardScaler`.

### 9️⃣ Training Models
The following models were trained:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**

### 🔟 Comparing Model Performance
Models were compared using the **R-squared** score. A bar chart visualizes the results.

## 🏆 Results
| Model                | R-squared Score |
|----------------------|----------------|
| Linear Regression   | 0.8135          |
| Ridge Regression    | 0.8134          |
| Lasso Regression    | 0.8136          |
| Random Forest       | **0.9275**      |
| Gradient Boosting   | 0.9221          |

### 🎯 **Best Model:**
✅ **Random Forest Regressor** performed best with an **R² score of ~0.92**.

## 📜 Conclusion
- **Random Forest** is the most accurate model for predicting taxi trip prices.
- **Lasso Regression** helped in feature selection.
- **Gradient Boosting** also performed well, making ensemble models a strong choice.
- **Linear & Ridge Regression** had moderate performance.

## 📌 How to Run the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/AbhishekMudaliyar/taxi-trip-price-prediction.git
   ```
2. Navigate to the project folder:
   ```bash
   cd taxi-trip-price-prediction
   ```
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the script:
   ```bash
   python taxi_price_prediction.py
   ```

## 📬 Contact
For any questions or suggestions, feel free to open an issue or reach out.
Gmail - abhishekmudaliyar2003@gmail.com

📌 **Happy Coding! 🚖**

