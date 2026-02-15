


In this project, I found out why customers leave the online store.


## 5 important facts revealed as a result of the analysis:

1) The majority of churners only placed 0, 1 or 2 orders.

Business logic:A customer is trying the platform but doesn't find enough reason to come back a third time. After the 2nd purchase, the customer's interest fades.

Solution: The customer who accepts the 2nd order will automatically receive the following message: "You are becoming our active customer! A special gift is waiting for you for your next purchase." and we should give bonuses

2)New Customers (Tenure < 5):Many  Customers are very thin in the first 5 months. If we do not pay attention to them during this period, we will lose them.
There is a strong correlation between the tenure column and the cashback amount. The problem is that new customers received cashback between 100 and 170, and there was a lot of churn in this range.

Solution:  if this cashback is less than the cashback of other companies, it should be increased, or cashbacks need to be tied to subsequent purchases to keep the customer.


3)50% of customer is leaving. The complain is not linked to other  factors (for example distance), which means there is a systemic problem.

Solution: If the complaints are not related to other factors, then we need new information.Analyze the complaint column by category (if available) rather than just 0 and 1 (yes/no). For example: "Quality", "Payment", "Application error",or If there are no categories, it is necessary to analyze the comments written by customers using NLP (Natural Language Processing) and find the most repeated words (Word Cloud).
Or If there is a problem with customers who complain, we have to give them a 10% discount on their next purchase to keep them.


4) Many customers have churned within 3 days of their last order.

Solution:Most of the customers leave the platform within the first 3 days after the last purchase. This indicates a lack of post-purchase communication.
If the model detects a churn risk on day 3, automatically provide a limited-time "Surprise Bonus".and  sending personalized push notifications and product guides within 72 hours of purchase.

## Model Results (XGBoost)

A high-accuracy model was built in customer prediction. Our main goal was to find as many potential customers as possible (Recall).XGBoost is better than Decision Tree

Model Accuracy (Accuracy): 97%

Recall: 91%

F1-Score: 0.90


## Technologies:

Python (Pandas, NumPy)

Machine Learning: XGBoost Classifier,Decision Tree

Visualization: Seaborn, Matplotlib



   
