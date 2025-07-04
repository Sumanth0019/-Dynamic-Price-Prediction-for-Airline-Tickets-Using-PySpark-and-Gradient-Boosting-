
<h1 align="center">✈️ Dynamic Price Prediction for Airline Tickets</h1>
<p align="center">
  <em>Scalable Airline Ticket Price Forecasting Using PySpark and Gradient Boosting</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Machine%20Learning-XGBoost-green?style=flat-square" />
  <img src="https://img.shields.io/badge/Big%20Data-PySpark-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/Language-Python%203.8+-yellow?style=flat-square" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square" />
</p>

---

##  Table of Contents

- [ Objective]
- [ Abstract]
- [ Importance of Flight Price Prediction]
- [Dataset Description]
- [ Data Attributes]
- [ Data Processing & Transformation]
- [ Experimentation Setup]
- [ Experimental Procedure]
- [ Model Performance Metrics]
- [Conclusion]
- [ Repository Structure]
- [🔗 Dataset Link](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)

---

##  Objective

Build a machine learning pipeline that leverages **Gradient Boosting (XGBoost)** for predicting dynamic airline ticket prices. Compare scalability and accuracy between **PySpark-based** and **Scikit-learn-based** implementations.

---

##  Abstract

The airline industry relies on **dynamic pricing** to maximize revenue. Traditional models like Random Forests often struggle with large datasets and scalability.

The airline industry tends to depend on dynamic pricing for revenue maximization in response to 
demand. Predicting flight ticket prices traditionally employs machine learning techniques, including 
Random Forest, Gradient Boosting Trees, and Decision Trees. However, these techniques often fail to 
appropriately and efficiently model large-scale volume data while providing a measure of high 
predictive accuracy. In this study, we present our Scalable Dynamic Pricing Model via Extreme 
Gradient Boosting (XGBoost) solving the problems with two configurations: a configuration with 
distributed processing using PySpark and the other configuration for baseline comparison without 
PySpark. 


This project introduces a **Scalable Dynamic Pricing Model** using **XGBoost**, with two configurations:
- **Standalone (Scikit-learn + Pandas)**
- **Distributed (PySpark MLlib)**

Key results:
-  XGBoost (Pandas): **R² = 0.9786**
-  XGBoost (PySpark): **R² = 0.9954**, improved scalability and reduced computation time

In addition, an **Integer Pricing Module** is developed for real-world deployment by adjusting prices based on seasonality and competition.

---

## Importance of Flight Price Prediction

-  **Passengers**: Helps find the best time to book
-  **Travel Agencies**: Boost customer trust with better recommendations
-  **Airlines**: Optimize revenue while staying competitive
-  **Data Scientists**: Extend research on demand forecasting
-  **E-commerce / OTAs**: Enhance user retention with smarter pricing

---

## Repository Structure
├──EDA.ipynb  # Exploratory Data Analysis with visual insights
├── Normal_GradientBoosting.ipynb   # Pandas + Scikit-learn pipeline
├── PySpark_GradientBoosting.ipynb  # PySpark MLlib pipeline
├── README.md


---

##  Dataset Link

[📂 Kaggle: Flight Price Prediction](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)

---

##  Dataset Description

The dataset contains details of both **Economy** and **Business** flight tickets with multiple predictive features.

### Variants:
- Economy
- Business
- Combined (Economy + Business)

---

## Attributes of the Dataset

| Attribute       | Description |
|----------------|-------------|
| S.No           | Unique identifier |
| Airline        | Name of airline (e.g., IndiGo, Air India) |
| Flight         | Flight number/code |
| Source_City    | Origin city |
| Departure_Time | Time of day (Morning, Afternoon, etc.) |
| Stops          | No. of stops (Non Stop, 1 Stop, etc.) |
| Arrival_Time   | Arrival time category |
| Destination    | Destination city |
| Class          | Travel class: Economy or Business |
| Duration       | Flight duration |
| Days_Left      | Days left before departure |
| Price          | Target variable (ticket price) |

---

##  Data Processing and Transformation

- Missing Value Treatment
- Categorical Encoding
- Log Transformation
- Feature Engineering
- Train/Test Split

---

## ⚙Experimentation Setup

| Component      | Spec                      |
|----------------|---------------------------|
| CPU            | Intel Core i7 Ultra       |
| RAM            | 16 GB                     |
| GPU            | Intel ARC                 |
| Storage        | SSD                       |
| OS             | Windows 11                |
| Language       | Python 3.8+               |
| IDE            | Jupyter & Kaggle Notebooks|

---

## Experimental Procedure

- 🔹 Load and clean dataset
- 🔹 Apply preprocessing steps
- 🔹 Train and tune Gradient Boosting models
- 🔹 Compare performance: Scikit-learn vs PySpark
- 🔹 Evaluate with R² and other error metrics

---

## Model Performance Metrics

| Model                | R² Score |
|----------------------|----------|
| Random Forest        | 0.728    |
| XGBoost (Scikit-learn) | 0.9786   |
| XGBoost (PySpark)    | **0.9954** |



---

## Conclusion

The PySpark-based XGBoost model:
- Achieves **highest accuracy**
- Scales better for large datasets
- Offers real-time adaptability for airline pricing strategies

> Future work: Real-time stream integration + Deep Learning Hybrid Models

---

## Repo Structure

 Airline-Ticket-Price-Prediction
   - EDA.ipynb                       # Exploratory Data Analysis with visual insights
   - Normal_GradientBoosting.ipynb  # Scikit-learn Gradient Boosting pipeline
   - PySpark_GradientBoosting.ipynb # PySpark MLlib pipeline for distributed training


##  Contact

For queries or collaboration:
- GitHub: [@Sumanth0019](https://github.com/Sumanth0019)
- Email: [sumanthreddy202039401@gmail.com]

---



Would you like help turning this into a live portfolio or website with GitHub Pages or Streamlit?

Let me know and I can generate that too!
