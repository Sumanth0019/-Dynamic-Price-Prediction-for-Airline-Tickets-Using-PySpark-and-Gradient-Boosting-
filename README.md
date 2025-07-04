# -Dynamic-Price-Prediction-for-Airline-Tickets-Using-PySpark-and-Gradient-Boosting-


# REPO Structure:
├──EDA.ipynb  # Exploratory Data Analysis with visual insights
├── Normal_GradientBoosting.ipynb   # Pandas + Scikit-learn pipeline
├── PySpark_GradientBoosting.ipynb  # PySpark MLlib pipeline
├── README.md

# Objective

The purpose of this project is to create a machine learning model that can utilize Gradient Boosting to 
predict flight ticket prices and evaluate the model performance with PySpark and without

# ABSTRACT 
 
The airline industry tends to depend on dynamic pricing for revenue maximization in response to 
demand. Predicting flight ticket prices traditionally employs machine learning techniques, including 
Random Forest, Gradient Boosting Trees, and Decision Trees. However, these techniques often fail to 
appropriately and efficiently model large-scale volume data while providing a measure of high 
predictive accuracy. In this study, we present our Scalable Dynamic Pricing Model via Extreme 
Gradient Boosting (XGBoost) solving the problems with two configurations: a configuration with 
distributed processing using PySpark and the other configuration for baseline comparison without 
PySpark.  
 
Experimental results reveal that XGBoost without PySpark provides a commendable R² score of 
0.9786—a score much higher than those achieved from conventional methods like Random Forest 
(R²=0.728). Meanwhile, running the PySpark enables distributed computing, which brings the R² score 
to an even higher level of 0.9954, alongside increased speed and scalability. The use of PySpark 
ensures that large volumes of data can be dealt with efficiently while at the same time reducing 
computational time, making this model an ideal candidate for real-life deployment in the airline 
industry. 
 
Moreover, taking into consideration not just predictive performance, we add an integer pricing module 
whose core function is to adjust prices based on demand; it factors in inputs such as seasonality and 
competition-based decisions on current pricing, making it therefore even more competitive from the 
point of view of the airline.  
 
Additionally, the proposed PySpark-based XGBoost model outperforms the existing machine learning 
approaches for both accuracy and scalability. It constitutes a viable, scalable, and high-performance 
alternative for dynamic pricing in the airline sector, having a great avenue to improve revenue 
management systems through predictive analytics and big data technologies.


# Importance of Flight Price Prediction 
Accurate flight price prediction helps various stakeholders in a range of ways: 
⚫ Passengers: It helps travelers understand the best times to purchase their flights and makes price 
trends accessible. Passengers can ultimately make the most well-informed and money-saving 
decisions. 
⚫ Travel Agencies: It provides a way for travel agencies to recommend the best time for their 
customers to purchase their flights, thus increasing customer satisfaction and gaining a competitive 
advantage. 
⚫ Airlines: It allows airlines to be dynamic with their fare pricing relative to market conditions. In 
this way, they can help maximize their profits while remaining competitive with other airlines. 
⚫ Data Scientists and Researchers: It gives the ability to extend research into dynamic pricing 
models, demand forecasting, and market behavior analysis as a whole. 
⚫ E-commerce / Online Travel Platforms: It improves pricing algorithms which online ticketing 
platforms use, which ultimately gives the customer better deals.

![image](https://github.com/user-attachments/assets/ad86e426-3d48-4b4c-a2ce-920d5d676d3c)


The dataset used is available on Kaggle:
[Flight Price Prediction](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)


# Dataset  description 
 
The dataset  contains the full flight price , detailing multiple attributes which contribute to the fare 
structure. The dataset categorized into three variants follows: 
 
⚫ Economy Dataset - An Economy dataset whose flight details and ticket prices are made for 
Economy class passengers. 
⚫ Business Dataset - Business dataset whose flight details and ticket prices are made available for 
Business class passengers. 
⚫ Combined Dataset - Economically and Business class together so as to have a comprehensive look 
at the pricing strategies.


# Attributes of the dataset: 
 
⚫ S.No: A number that serially represents a record. 
⚫ Airline: Name of the flying airline (for example-IndiGo, Air India, Vistara). 
⚫ Flight: Numbers or identifiers assigned to a travel journey. 
⚫ Source_City: The name of the city that serves as the origin point for flights. 
⚫ Departure_Time: Leaving time fixed for a flight; classifications: Morning, Afternoon, Evening, Late Night. 
⚫ Stops: Number of haltings on the journey (Non Stop, 1 Stop, 2+ Stops). 
⚫ Arrival_Time: The scheduled time at which the flight is scheduled to arrive at the destination. 
⚫ Destination: The city where the flight goes to arrive. 
⚫ Class: Type of travel class offered, either Economy or Business. 
⚫ Duration: Total flying time (in hours). 
⚫ Days_Left: Number of days left for departure, at the time when a ticket is bought. 
⚫ Price: The final ticket price, which is the target variable for predictive modeling.


# Data Processing and Transformation

  - Missing Value Treatment
  - Categorical Encoding
  - Numerical Feature Normalization
  - Log Transformation
  - Feature Engineering
  - Data Splitting


# Experimentation Setup

 - CPU : Intel Core i7 Ultra
 - RAM : 16GB
 - GPU : Intel ARC
 - Storage : SSD to enhance quickness
 - OS : Windows 11
 - Prog Language : Python 3.8+
 - IDE : Jupyter notebooks and kaggle notebooks


# Experimental Procedure: 
 
⚫ The dataset was loaded and preprocessed to ascertain data quality. 
⚫ A Gradient Boosting Method (GBM) was trained and tuned for hyperparameters to achieve the 
best prediction accuracy. 
⚫ The comparison of the XGBoost implementation with and without PySpark was made to analyze 
the scalability and performance differences.  
⚫ Lastly, corresponding predictions were generated against actual prices using different error metrics 
for evaluation. 
⚫ This experimental setup will ensure a solid and reproducible avenue toward the dynamic pricing 
prediction using machine learning for fare forecasting. 

# Model Performance metrics

![image](https://github.com/user-attachments/assets/a69dc95e-5396-4f87-a0b6-0f01d1392063)

# Conclusion
 
The model utilizing PySpark and XGBoost is thus the best among the rest when it comes 
to accuracy and computational efficiency that fit better for modern-day airline revenue management 
systems. Future directions would look towards deep learning-based hybrid models and real-time stream 
data integration to step up response and prediction performance
