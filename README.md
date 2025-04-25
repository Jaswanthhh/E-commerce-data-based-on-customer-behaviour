# 📊 E-Commerce Customer Behavior Analysis & Predictive Modeling

This project leverages synthetic e-commerce data to perform end-to-end customer behavior analysis, data preprocessing, feature engineering, and predictive modeling, culminating in an interactive web dashboard for visual insights. The solution is built with **Python, scikit-learn, XGBoost, Plotly Dash, and pandas**.

---

## 🧠 Objectives

- Generate a realistic e-commerce dataset simulating user behavior and transaction metrics.
- Introduce controlled data inconsistencies (e.g., missing values, duplicates, outliers).
- Perform thorough data cleaning, feature transformation, and model evaluation.
- Build and compare multiple machine learning models to predict key behaviors (e.g., discount availing).
- Deploy a fully functional interactive dashboard to visualize metrics, feature importances, and PCA-reduced patterns.

---

## 📁 Project Structure

├── app.ipynb # Dash web app integrating ML outputs and visualizations
├── E-COMMERCE DATA ... .ipynb # Notebook for dataset generation and ML experimentation
├── ecommerce_dataset.csv # Generated synthetic dataset with intentional inconsistencies
├── preprocessed_ecommerce_dataset.csv (optional) # Cleaned dataset (if saved separately)
├── README.md # Project overview and documentation


---

## 🧬 Dataset Description

The dataset simulates **1,005 customer records** with 15 features:

- **Demographics**: `Customer_ID`, `Gender`, `Age`, `Region`
- **Behavioral Metrics**: `Browsing_Hours`, `Purchase_Count`, `Cart_Abandonment_Rate`, `Return_Rate`
- **Transactional Data**: `Product_Category`, `Product_Price`, `Payment_Method`, `Delivery_Time`, `Customer_Rating`, `Discount_Availed`
- **Data Challenges Added**:
  - 10% **missing values**
  - **Duplicated rows**
  - **Outliers** in `Age`, `Product_Price`
  - **Gaussian noise** in `Browsing_Hours`

---

## 🧹 Data Preprocessing & Feature Engineering

- Imputation of missing values (mean/mode)
- One-hot encoding for categorical variables
- Outlier identification and optional treatment
- Feature selection and dimensionality reduction (PCA)

---

## 🤖 Machine Learning Models

### Classification Task: Predicting `Discount_Availed`

| Model         | Metrics Tracked                  |
|---------------|----------------------------------|
| Decision Tree | Accuracy, Precision, Recall, F1-Score |

### Regression Task: Predicting aggregate customer target (e.g., spend behavior)

| Model         | Metrics Tracked   |
|---------------|------------------|
| Decision Tree | MSE, R²          |
| Random Forest | MSE, R²          |
| XGBoost       | MSE, R²          |

---

## 📊 Interactive Dashboard

Developed using **Plotly Dash**. Features include:

- 📈 **Model Performance Comparison** (Bar Chart)
- 🧮 **Pre/Post Preprocessing Distributions** (Histograms)
- 🔥 **Feature Importance** (Bar Chart using Random Forest)
- 🧬 **Correlation Heatmap** (px.imshow)
- 🧿 **PCA Visualization** (2D Scatter)

Run locally with:

-python app.py


---

## 💡 Key Learnings

- Effective simulation of realistic business data using Faker
- Full data pipeline from ingestion to insight
- Hands-on model tuning and evaluation
- Seamless deployment of ML results into a user-friendly dashboard

---

## 🚀 Future Enhancements

- Expand classification to include multiple targets (e.g., churn prediction)
- Incorporate time-series behavior and session logs
- Add advanced visual filters and KPIs in the dashboard
- Deploy dashboard via Docker/Cloud for production use

---

## 📚 Technologies Used

- Python (Pandas, NumPy, Scikit-learn, XGBoost)
- Faker (for synthetic data generation)
- Dash & Plotly (dashboard & visualizations)
- Jupyter Notebook (EDA and development)

---

## 📝 Author

This project was developed as part of a comprehensive data science initiative to understand and predict customer behaviors in e-commerce. For contributions or collaborations, feel free to connect!
e-mail : jaswanth2jaswanth@gmail.com
