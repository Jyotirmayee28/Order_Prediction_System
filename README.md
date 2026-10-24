# 📦 Order Prediction System
🚀 Machine Learning System for Predicting Daily Orders


---

## 📜 Project Overview  
The **Order Prediction System** is a Machine Learning-based solution designed to predict the number of orders for a given day based on historical and operational factors. The system analyzes parameters such as **day of the week, promotion activity, and previous-day orders** to identify patterns that influence current-day order demand.

The project uses **Exploratory Data Analysis (EDA)** to understand relationships between different features and order volume. Data preprocessing is performed by checking for missing values and removing extreme order values using the **Z-score method**.

A **Linear Regression** model is then trained using historical order data to predict current-day orders. The model is evaluated using **Mean Squared Error (MSE)**, and users can also provide new-day information to generate predicted order quantities.

---


## 🎯 Key Features  
✅ Daily order prediction using Machine Learning 📦  
✅ Historical order data analysis 📊  
✅ Outlier detection using Z-score 🔍  
✅ Missing-value checking and data preprocessing 🧹  
✅ Promotion-based order analysis 📈  
✅ Linear Regression-based prediction 🤖  
✅ Model evaluation using Mean Squared Error 📋  
✅ Prediction of orders for a new day 🔮

---

## 🛠️ Tech Stack  
- **Programming Language**: Python 🐍  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn  
- **Machine Learning**: Scikit-learn  
- **Algorithm**: Linear Regression  
- **Data Processing**: Z-score Outlier Detection, Data Cleaning  
- **Model Evaluation**: Mean Squared Error (MSE)  
- **Dataset**: Large Orders Dataset (`large_orders_data.xlsx`)

---

## 🖥️ How It Works
1️⃣ **Load Dataset:** Import the order dataset from an Excel file using Pandas.

2️⃣ **Data Inspection:** Check the dataset for missing values and examine its structure and information.

3️⃣ **Outlier Removal:** Calculate Z-scores for the order values and remove extreme observations using a threshold of 3.

4️⃣ **Feature Preparation:** Rename and organize the dataset columns, including `Day_of_Week`, `Promotion_Active`, `Previous_Day_Orders`, and `Current_Day_Orders`.

5️⃣ **Exploratory Analysis:** Use pair plots to visualize relationships between the different features and current-day order volume.

6️⃣ **Feature Selection:** Use `Day_of_Week`, `Promotion_Active`, and `Previous_Day_Orders` as input features, with `Current_Day_Orders` as the target variable.

7️⃣ **Train Model:** Split the dataset into training and testing sets using an **80/20 train-test split** and train a Linear Regression model.

8️⃣ **Generate Predictions:** Use the trained model to predict current-day order quantities for the test dataset.

9️⃣ **Evaluate Model:** Calculate the **Mean Squared Error (MSE)** to measure the difference between actual and predicted order values.

🔟 **Predict New Orders:** Enter the day of the week, promotion status, and previous-day orders to generate a predicted order quantity for a new day.


---

## 📊 Model

**Algorithm Used:** Linear Regression

**Input Features:**
- `Day_of_Week`
- `Promotion_Active`
- `Previous_Day_Orders`

**Target Variable:** `Current_Day_Orders`

**Train-Test Split:** 80% Training | 20% Testing

**Evaluation Metric:** Mean Squared Error (MSE)

**Mean Squared Error:** **170.61196315719766** 📈

The model achieved a **Mean Squared Error of 170.61**, indicating the average squared difference between the actual and predicted order values on the test dataset.
