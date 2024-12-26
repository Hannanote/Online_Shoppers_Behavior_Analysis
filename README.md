### Online Shoppers Purchasing Intention Machine Learning Analysis


#### Project Overview:


This project explores the online shopping behavior of consumers, focusing on their actions of searching, selecting, purchasing, using, and disposing of goods and services on the internet.

For e-commerce platforms, an essential question is whether a customer is just browsing or is likely to make a purchase. Since customers vary widely in behavior, it’s crucial for sellers to avoid treating all users the same way. By understanding these differences, sellers can better allocate resources to attract and retain customers who are more likely to complete a purchase. Proactive strategies, such as offering time-limited discounts or free trials, can be employed to incentivize buying behavior.

#### The goal of this project is to conduct a thorough analysis of consumer behavior, with a focus on the following tasks:

+ Classification (Exploratory Data Analysis and Modeling)
+ Customer Segmentation
+ Supervised Learning

<br>

#### Dataset Information:


This project uses the Online Shoppers Purchasing Intention Dataset, which was collected from an online bookstore. The dataset consists of feature vectors representing 12,330 sessions, each corresponding to a unique user session over a 1-year period. The data was designed to minimize biases that could arise from specific campaigns, special days, user profiles, or time periods.

<br>

##### Differences Between Bounce Rate and Exit Rate:


Bounce rate refers to the percentage of single-session visits, while exit rate indicates the percentage of exits from a specific page. The former is calculated by dividing the number of one-page visits by the total number of entrance visits, whereas the latter is calculated by dividing the number of exits from a page by the total visits to that page. Although both metrics are related, a key difference is that the exit rate accounts for the percentage of visitors who exited during their final session, whereas bounce rate only considers those who interacted in a single session. Therefore, bounce rate does not take prior activity into account. This means that all bounces are technically exits, but not all exits are bounces.


##### Implications of High Bounce and Exit Rates: 


A high bounce rate could signal issues with user experience, such as poor website design, slow page load times, or other technical problems. On the other hand, a high exit rate could point to weak areas within sales funnels, where customers leave before completing their purchase. BigCommerce suggests that a bounce rate between 30% and 55% is generally acceptable. Our analysis shows that bounce rates tend to be much lower, often below 10%. According to UpSide Business, a bounce rate under 5% could indicate a potential issue, such as duplicate Google Analytics tracking codes, which requires further investigation. If no technical errors are found, efforts should be focused on optimizing bounce rates and exit rates to protect sales and customer loyalty.

##### Paper

In this paper, we propose a real-time online shopper behavior analysis system consisting of two modules which simultaneously predicts the visitor’s shopping intent and Web site abandonment likelihood. In the first module, we predict the purchasing intention of the visitor using aggregated pageview data kept track during the visit along with some session and user information. The extracted features are fed to random forest (RF), support vector machines (SVMs), and multilayer perceptron (MLP) classifiers as input. We use oversampling and feature selection preprocessing steps to improve the performance and scalability of the classifiers. The results show that MLP that is calculated using resilient backpropagation algorithm with weight backtracking produces significantly higher accuracy and F1 Score than RF and SVM. Another finding is that although clickstream data obtained from the navigation path followed during the online visit convey important information about the purchasing intention of the visitor, combining them with session information-based features that possess unique information about the purchasing interest improves the success rate of the system. In the second module, using only sequential clickstream data, we train a long short-term memory-based recurrent neural network that generates a sigmoid output showing the probability estimate of visitor’s intention to leave the site without finalizing the transaction in a prediction horizon. The modules are used together to determine the visitors which have purchasing intention but are likely to leave the site in the prediction horizon and take actions accordingly to improve the Web site abandonment and purchase conversion rates. Our findings support the feasibility of accurate and scalable purchasing intention prediction for virtual shopping environment using clickstream and session information data.



##### References
https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset
