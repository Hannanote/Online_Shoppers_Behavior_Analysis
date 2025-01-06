### Online Shoppers Purchasing Intention Machine Learning Analysis


#### Project Overview:


This project explores the online shopping behavior of consumers, focusing on their actions of searching, selecting, purchasing, using, and disposing of goods and services on the internet.

For e-commerce platforms, an essential question is whether a customer is just browsing or is likely to make a purchase. Since customers vary widely in behavior, it’s crucial for sellers to avoid treating all users the same way. By understanding these differences, sellers can better allocate resources to attract and retain customers who are more likely to complete a purchase. Proactive strategies, such as offering time-limited discounts or free trials, can be employed to incentivize buying behavior.

=====================================================================================
Overview: In the world of e-commerce, understanding customer behavior is essential for optimizing sales strategies and improving the user experience. This project explores the online shopping behavior of consumers, focusing on their actions such as searching, selecting, purchasing, using, and disposing of goods and services on the internet.

For e-commerce platforms, one of the most crucial questions is whether a customer is just browsing or is actually likely to make a purchase. Customers exhibit highly diverse behaviors, making it important for sellers to understand these differences. By effectively analyzing these behaviors, sellers can better allocate their resources to attract and retain customers who are more likely to convert into buyers. Proactive strategies like offering time-limited discounts or free trials can also incentivize purchasing decisions.

This project uses machine learning models to predict online shoppers' purchasing intentions, utilizing various classification algorithms to extract meaningful insights.

#### The goal of this project is to conduct a thorough analysis of consumer behavior, with a focus on the following tasks:

+ Classification
+ Exploratory Data Analysis
+ Modeling
+ Model Evaluation
<br>

#### Dataset Information:


This project uses the Online Shoppers Purchasing Intention Dataset, which was collected from an online bookstore. The dataset consists of feature vectors representing 12,330 sessions, each corresponding to a unique user session over a 1-year period. The data was designed to minimize biases that could arise from specific campaigns, special days, user profiles, or time periods.

<br>

#### Differences Between Bounce Rate and Exit Rate:


Bounce rate refers to the percentage of single-session visits, while exit rate indicates the percentage of exits from a specific page. The former is calculated by dividing the number of one-page visits by the total number of entrance visits, whereas the latter is calculated by dividing the number of exits from a page by the total visits to that page. Although both metrics are related, a key difference is that the exit rate accounts for the percentage of visitors who exited during their final session, whereas bounce rate only considers those who interacted in a single session. Therefore, bounce rate does not take prior activity into account. This means that all bounces are technically exits, but not all exits are bounces.

![image](https://github.com/user-attachments/assets/e755470b-afef-4737-86ba-cd1ebba7bb6b)

#### Implications of High Bounce and Exit Rates: 


A high bounce rate could signal issues with user experience, such as poor website design, slow page load times, or other technical problems. On the other hand, a high exit rate could point to weak areas within sales funnels, where customers leave before completing their purchase. BigCommerce suggests that a bounce rate between 30% and 55% is generally acceptable. Our analysis shows that bounce rates tend to be much lower, often below 10%. According to UpSide Business, a bounce rate under 5% could indicate a potential issue, such as duplicate Google Analytics tracking codes, which requires further investigation. If no technical errors are found, efforts should be focused on optimizing bounce rates and exit rates to protect sales and customer loyalty.

+ ounce Rate: Percentage of visitors who view only one page and leave.
+ Exit Rate: Percentage of visitors who leave from a specific page after interacting with the site.
+ Difference: While all bounces are exits, not all exits are bounces. Bounce rate doesn't account for prior actions, whereas exit rate considers the visitor's entire journey.
+ Implications: A high bounce rate might indicate poor user experience, while a high exit rate suggests weak areas in the sales funnel.


#### Modeling
+ Logistic Regression
+ Random Forest
+ Decision Tree
+ AdaBoost
+ Hyperparameter Tuning for Logistic Regression (RandomizedSearch CV)


![image](https://github.com/user-attachments/assets/443870b0-915f-40e2-bcae-c27f1ef8c8c2)


<img src='https://github.com/user-attachments/assets/70e09775-7220-46e6-bce8-5e14f6d975cd' width='700px' height='400px'>


Model Evaluation (Random Forest Classifier):
- Accuracy: 0.885
- Specificity: 0.962
- Recall: 0.504
- Precision: 0.724
- F1-Score: 0.594
- ROC-AUC: 0.73

<img src='https://github.com/user-attachments/assets/e934d83a-1f32-4dbc-b6b0-c1aae23976ca' width='700px' height='400px'>


#### Feature Importance:
The feature importance plot shows the relative importance of each feature used by the model. In this case, the most important features for predicting purchasing behavior were the page values, such as the pages visited and the time spent on the site.

#### Conclusion:
This project demonstrates the power of machine learning in understanding consumer behavior and predicting purchasing intentions in an online shopping environment. By leveraging techniques such as feature engineering, model evaluation, and hyperparameter tuning, we can build accurate models that help e-commerce platforms make data-driven decisions to increase sales and improve customer retention.

The Random Forest classifier emerged as the most accurate model, achieving high accuracy and specificity. The feature importance analysis highlighted the importance of session-related information in predicting purchase behavior.

#### Next Steps:
Scalability: Explore the scalability of the model with larger datasets.
Real-Time Prediction: Implement real-time prediction systems for e-commerce platforms.
Advanced Models: Investigate deep learning models for even better performance.

##### References
https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset
