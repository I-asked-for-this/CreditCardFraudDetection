## Machine Learning Model Comparison with Correlation Check
### Project Description:
This project explores the application of five different machine learning algorithms - Logistic Regression, Support Vector Classifier (SVC), Random Forest Classifier,K-Nearest Neighbors Classifier (KNN), and Gaussian Naive Bayes (GNB) - in the context of credit card fraud detection.
##### This project serves as a comprehensive guide to understanding the role of feature selection in machine learning model performance, particularly in the context of credit card fraud detection.

### Unique Aspects:
##### The problem of credit card fraud detection is characterized by several unique aspects:
1-Enormous Data: The models need to process millions of transactions daily, necessitating high computational efficiency.

2-Imbalanced Data: The vast majority of transactions are non-fraudulent, resulting in a highly imbalanced dataset.

### Handling Imbalanced Dataset: Undersampling
In the context of our project, we encountered the common issue of imbalanced datasets. This is a scenario where the classes in the target variable are not represented equally. In our case, the majority of credit card transactions were non-fraudulent, leading to a highly imbalanced dataset.

After conducting research, we decided to use undersampling to address this issue. Undersampling is a technique where you randomly overlook some of the observations from the majority class in order to balance the class distribution.

Initially, we were concerned that undersampling might hurt the model’s performance. This is a valid concern as undersampling can lead to loss of information, given that it involves removing instances from the dataset. However, our results showed that undersampling actually improved the performance of our models.


### Something special:
Initially, we applied these models directly to our dataset, without considering the correlation between the features and the target variable. Then, we incorporated a correlation check before building the models. This step involved calculating the correlation of each feature with the target variable, which added an extra layer of depth to our model comparison. This correlation check was ensured by having a look at the heatmap or sample correlation matrix. We then understood the prevalence of certain variables when put into prespective in the what we referred to as the 'grand scheme'.
Note: Goes without saying we cleaned the data, ie, dropped the duplicate values, filled the missing data and of course we standardized it using the standard scaler, which was not arbitrary because we checked every variable to see the distribution of the values(Most variables in this dataSet were pre-standardized and had their names written off). Which turned out to be in a Gaussian pattern, and therefore we came to the conclusion that this is almost definitely the work of a standard scaler(We left a sample for the distribution checking).

### Results and Insights:

Through our project, we discovered that the performance of the machine learning models was quite similar when using all variables versus a select few. This observation led us to an important insight: working with a handful of relevant variables can be just as effective, if not more so, than working with a larger set.

This finding is significant for several reasons:

#### Efficiency: 
Using fewer variables reduces the computational complexity of the models, leading to faster training times and less resource usage.
#### Simplicity: 
Models with fewer variables are easier to understand and interpret.
#### Avoid Overfitting: 
By limiting the number of variables, we reduce the risk of overfitting, where the model learns the training data too well and performs poorly on unseen data.

In retrospect, this may seem evident, but the process of reaching this conclusion through our own research was a valuable learning experience. It underscores the importance of feature selection in machine learning and the need to question the assumption that more data always leads to better results. This insight is a key takeaway from our project and serves as a reminder of the importance of understanding the data and the problem at hand.


## Author: Mohamed Taha Sta.
### Team members: Mohamed Taha Sta | Fares Makki | Jasser Hamdi.

