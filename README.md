Problem Statement:

E-commerce companies process millions of orders across multiple categories, sellers, locations, and payment methods. 
However, businesses often face challenges such as:
1. High return rates increasing logistics costs
2. Delivery delays reducing customer satisfaction
3. Difficulty identifying risky sellers and products
4. Inefficient discount strategies impacting profitability
5. Lack of operational visibility into return patterns

These issues lead to:

1. Increased operational expenses
2. Revenue leakage
3. Delayed business decisions
4. Poor customer experience


Objective:
Develop an AI-powered Return & Delivery Intelligence System that:
1. Predicts whether an order is likely to be returned
2. Identifies operational drivers behind returns and delays
   
Problem Solution - Machine Learning Method
 Predict:
Whether an order will be returned using the pre-defined feature (is_returned) in the dataset

This is highly business-relevant because:

1. Product returns directly affect logistics costs
2. Helps reduce reverse logistics inefficiencies
3. Matches your logistics and returns analysis experience perfectly

However from analysing the model accuracy report/classification report I found that the models are giving 100% accuracy in its prediction which seems high unlikely towards any data. To understand further i checked if there is any one feature who is dominating every other feature in its prediction also if there is any one feature whose correlation is near to 1.0. Upon testing this theory i found that is_returned feature is more domineering towards other features with correlation 1.0 that means that its a major red-flag when it comes to machine learning modelling
It usually indicates:

1. Data Leakage

Meaning:

The model is indirectly “seeing the answer” before prediction.

2. Correlation close to +1 means:
As the feature increases,
the target variable also increases almost perfectly.

This is extremely unusual in real-world business data.
