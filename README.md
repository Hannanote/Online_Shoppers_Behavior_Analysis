## Online Shoppers Purchasing Intention Machine Learning Analysis


<br>

#### Project Overview:

This project explores the online shopping behavior of consumers, focusing on their actions of searching, selecting, purchasing, using, and disposing of goods and services on the internet.

For e-commerce platforms, an essential question is whether a customer is just browsing or is likely to make a purchase. Since customers vary widely in behavior, it’s crucial for sellers to avoid treating all users the same way. By understanding these differences, sellers can better allocate resources to attract and retain customers who are more likely to complete a purchase. Proactive strategies, such as offering time-limited discounts or free trials, can be employed to incentivize buying behavior.

The goal of this project is to analyze online shopper behavior and predict their purchase intentions. The analysis is achieved through various machine learning algorithms, offering insights that can guide resource allocation, customer engagement, and sales strategies.



이 프로젝트는 소비자의 온라인 쇼핑 행동을 분석하며, 상품과 서비스를 검색하고 선택하고 구매하고 사용하며 폐기하는 과정을 중심으로 진행됩니다.
전자상거래 플랫폼에서 중요한 질문 중 하나는 고객이 단순히 탐색하는 것인지 아니면 실제로 구매할 가능성이 있는지를 파악하는 것입니다. 고객들은 매우 다양하므로 판매자들이 모든 고객을 동일하게 대하지 않는 것이 중요합니다. 이러한 차이를 이해함으로써 판매자는 구매 가능성이 높은 고객을 유치하고 유지하는 데 더 많은 자원을 효율적으로 배분할 수 있습니다. 또한, 시간 한정 할인 쿠폰이나 무료 체험과 같은 적극적인 전략을 사용하여 구매를 유도할 수 있습니다.
이 프로젝트의 목표는 온라인 쇼핑객의 행동을 분석하고 그들의 구매 의도를 예측하는 것입니다. 이 분석은 다양한 머신 러닝 알고리즘을 통해 이루어지며, 이는 리소스 할당, 고객 참여 및 판매 전략을 안내하는 데 도움이 되는 통찰을 제공합니다.


<br>

#### The goal of this project is to conduct a thorough analysis of consumer behavior, with a focus on the following tasks:

+ Classification
+ Exploratory Data Analysis
+ Modeling
+ Model Evaluation
<br>

#### Dataset Information:


This project uses the Online Shoppers Purchasing Intention Dataset, which was collected from an online bookstore. The dataset consists of feature vectors representing 12,330 sessions, each corresponding to a unique user session over a 1-year period. The data was designed to minimize biases that could arise from specific campaigns, special days, user profiles, or time periods.

#### Target Variable: 
Whether a visitor made a purchase or not. Out of 12,330 sessions, 10,422 did not result in a purchase, while 1,908 did.

<img src='https://github.com/user-attachments/assets/8cf2c958-2753-4e9a-bae0-f3f9a99e2343' width='600px' height='400px'>


<br>

#### Monthly Revenue and Contribution:
This graph shows the monthly revenue breakdown and the percentage of total revenue for each month:

<img src='https://github.com/user-attachments/assets/e76d80c6-520d-47ef-b6c3-5099152dad60' width='700px' height='400px'>


Peak Revenue Months: November, with a significant spike in purchases, possibly due to holiday shopping behaviors.
Low Revenue Months: January and August show relatively lower revenues, which could be attributed to seasonal fluctuations in shopping behavior.


<br>

#### Differences Between Bounce Rate and Exit Rate:


Bounce rate refers to the percentage of single-session visits, while exit rate indicates the percentage of exits from a specific page. The former is calculated by dividing the number of one-page visits by the total number of entrance visits, whereas the latter is calculated by dividing the number of exits from a page by the total visits to that page. Although both metrics are related, a key difference is that the exit rate accounts for the percentage of visitors who exited during their final session, whereas bounce rate only considers those who interacted in a single session. Therefore, bounce rate does not take prior activity into account. This means that all bounces are technically exits, but not all exits are bounces.

<img src='https://github.com/user-attachments/assets/e755470b-afef-4737-86ba-cd1ebba7bb6b' width='700px' height='400px'>

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


<br>


Model Evaluation (Random Forest Classifier):

The Random Forest classifier demonstrated strong predictive performance, particularly in terms of specificity, which is essential in distinguishing between potential buyers and non-buyers.

- Accuracy: 0.885
- Specificity: 0.962
- Recall: 0.504
- Precision: 0.724
- F1-Score: 0.594
- ROC-AUC: 0.73

<img src='https://github.com/user-attachments/assets/70e09775-7220-46e6-bce8-5e14f6d975cd' width='700px' height='400px'>

<br>




<br>

#### Feature Importance:
The feature importance plot shows the relative importance of each feature used by the model. In this case, the most important features for predicting purchasing behavior were the page values, such as the pages visited and the time spent on the site.

<img src='https://github.com/user-attachments/assets/e934d83a-1f32-4dbc-b6b0-c1aae23976ca' width='700px' height='400px'>


<br>

#### Conclusion:
This project demonstrates the power of machine learning in understanding consumer behavior and predicting purchasing intentions in an online shopping environment. By leveraging techniques such as feature engineering, model evaluation, and hyperparameter tuning, we can build accurate models that help e-commerce platforms make data-driven decisions to increase sales and improve customer retention.

Model Performance: Random Forest was the most accurate model, achieving high specificity and reasonable recall.

Revenue Trends: November showed the highest number of purchases, correlating with seasonal shopping behavior. We also found that certain pages and behaviors, like browsing more product pages and spending more time on the site, were predictive of purchases.


#### Next Steps:
+ Scalability: Explore the scalability of the model with larger datasets.
+ Real-Time Prediction: Implement real-time prediction systems for e-commerce platforms.
+ Advanced Models: Investigate deep learning models for even better performance.

##### References
https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset
