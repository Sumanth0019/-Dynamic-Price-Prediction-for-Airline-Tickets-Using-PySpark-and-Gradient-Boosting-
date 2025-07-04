# -Dynamic-Price-Prediction-for-Airline-Tickets-Using-PySpark-and-Gradient-Boosting-
ABSTRACT 
 
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
