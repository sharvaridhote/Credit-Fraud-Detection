# Credit-Fraud-Detection 


## Installations

Libraries used - To succesfully run this Jupyter notebook the following libraries need to be installed. 

    - Python 3
    - Pandas
    - Sklearn
    - Seaborn
    - Matplotlib
    - Numpy
    

## Motivation 

I found the imbalanced dataset problem interesting and challenging.  That’s the motivation behind selecting this topic for my first DS project. In real life, imbalanced dataset problem affects different businesses spanning from cybersecurity, financial institutions and industrial or medical diagnosis. Credit card fraud detection is an important issue in the banking sector. 

The goal of this project is to understand everything about solving this challenging problem with different examples and learning different approaches and provide a guidance to ML newbie learners with all the information for starting the project related to imbalanced datasets. I have carried out a comprehensive review of different blogs and articles. I started with a popular credit fraud dataset to carry out data explorations, learn different metrics and techniques to handle the imbalanced dataset. 

## File Description

**Data credit and download :**
- Andrea Dal Pozzolo, Olivier Caelen, Reid A. Johnson and Gianluca Bontempi. Calibrating Probability with Undersampling for Unbalanced Classification. In Symposium on Computational Intelligence and Data Mining (CIDM), IEEE, 2015Credit Card Fraud Detection : Anonymised credit card transactions labelled as fraudulent or genuine.
- Download dataset  @ : https://www.kaggle.com/mlg-ulb/creditcardfraud

- The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions. 
- Input - 31 features with 28 PCA transformed features except 'Time' and 'Amount'.

**Files in the repository:** 
- Credit Card Modeling.ipynb - This file includes detail steps and the code I used to achieve the results of this project. 
- Fraud_detection_Report.pdf - File containing review, results and conclusions. 

**Dataset :** Credit card dataset presents transactions that occurred in two days, where there are 492 frauds out of 284,807 transactions. 

## Results & Conclusions

- class_weight= option for the classifier works like resampling. 
- Feature scaling was applied to scale time and the amount. However, V1-V27 features were within a scale. 
- Grid search was used to obtain best parameters
- Selecting learning algorithms and/or resampling techniques depends on the metrics and the business problem to be solved.  
- Credit cards are main source of transactions for any bank customers. Thus, if our fraud detection model blocks non-fraudulent transaction
- the customer complaints and customer dissatisfaction will increase. Thus, the metric used for fraud detection should be accuracy of
  Classifying non-fraud cases then the recall score. The cost of miss-classifying actual positive is very high. 
- Gradient boosting algorithm performed better only with the SMOTE sampling technique. It needs further parameter tuning or not suitable for this dataset.
- All advanced ensemble models’ performance is comparable when applied re-sampling technique with an AUC score above 0.99.


Please see the Fraud_Detection_Report in the root directory for the review, results and conclusions.





