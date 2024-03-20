# Credit Card Fraud Detection project

# Introduction:

The Credit Card Fraud Detection project focuses on enhancing financial security through advanced machine learning and data analysis techniques.

Its primary goal is to develop a predictive model that can proactively distinguish between legitimate and fraudulent credit card transactions.

Leveraging machine learning, specifically supervised learning and anomaly detection, this project addresses the dynamic nature of fraud patterns, surpassing the limitations of traditional rule-based systems.

Key components involve data preprocessing, feature engineering, model selection, and evaluation metrics.

The exploration of machine learning algorithms, including logistic regression, decision trees, XGBoost , and HistGradientBoostingClassifier, aims to identify the most effective approach for fraud detection.

Ultimately, the project aims to provide a robust, efficient, and adaptive solution to safeguard financial transactions from the evolving landscape of fraudulent activities.

# Project Objectives

In this project, the goal is to leverage machine learning models to predict fraudulent credit card transactions. The process typically involves preprocessing and exploring the dataset, which may include features such as transaction amount, location, time, and previous transaction history.

After splitting the dataset into training and testing sets, various machine learning algorithms such as logistic regression, decision trees, random forests, or support vector machines can be employed to build predictive models.

The models are trained on a labeled dataset where instances of fraudulent and non-fraudulent transactions are identified. Evaluation metrics like precision, recall, and the F1 score are commonly used to assess the model's performance. Continuous improvement may involve tuning hyperparameters, employing ensemble methods, or exploring more advanced techniques like anomaly detection.

The final model aims to accurately identify and prevent fraudulent credit card transactions by learning patterns from historical data.

# Project Understanding

Suppose you get a call from your bank, and the customer care executive informs you that your card is about to expire in a week. Immediately, you check your card details and realise that it will expire in the next eight days. Now, to renew your membership, the executive asks you to verify a few details such as your credit card number, the expiry date and the CVV number. Will you share these details with the executive?

In such situations, you need to be careful because the details that you might share with them could grant them unhindered access to your credit card account.

Although digital transactions in India registered a 51% growth in 2018–2019, their safety remains a concern. Fraudulent activities have increased severalfold, with approximately 52,304 cases of credit/debit card fraud reported in FY 2019 alone. Owing to this steep increase in banking frauds, it is the need of the hour to detect these fraudulent transactions in time to help consumers and banks that are losing their credit worth each day. Machine learning can play a vital role in detecting fraudulent transactions.

So far, you have learnt about the different types of machine learning models. Now, you will learn which model to choose for your purpose and the reason for it. Understanding models based on different scenarios is an important skill that a data scientist / machine learning engineer should possess. In addition, tuning your model is equally important to get the best fit for your given data.

By the end of this module, you will learn how you can build a machine learning model that is capable of detecting fraudulent transactions. You will also learn how to handle class imbalances present in any data set, along with model selection and

# Problem Statement:

The problem statement chosen for this project is to predict fraudulent credit card transactions with the help of machine learning models.

In this project, you will analyse customer-level data which has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group.
The dataset has a total of 2,84,807 transactions, out of which 492 are fraudulent. Since the dataset is highly imbalanced, so it needs to be handled before model building.

# Business Problem Overview:

For many banks, retaining high profitable customers is the number one business goal. Banking fraud, however, poses a significant threat to this goal for different banks. In terms of substantial financial losses, trust and credibility, this is a concerning issue to both banks and customers alike.

It has been estimated by Nilson report(https://nilsonreport.com/upload/content_promo/The_Nilson_Report_Issue_1164.pdf) that by 2020 the banking frauds would account to $30 billion worldwide. With the rise in digital payment channels, the number of fraudulent transactions is also increasing with new and different ways.

In the banking industry, credit card fraud detection using machine learning is not just a trend but a necessity for them to put proactive monitoring and fraud prevention mechanisms in place. Machine learning is helping these institutions to reduce time-consuming manual reviews, costly chargebacks and fees, and denials of legitimate transactions.

# Data Dictionary:

The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with Principal Component Analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in others.

# Project Pipeline:
The project pipeline can be briefly summarized in the following four steps:

• Data Understanding: Here, you need to load the data and understand the features present in it. This would help you choose the features that you will need for your final model.

• Exploratory data analytics (EDA): Normally, in this step, you need to perform univariate and bivariate analyses of the data, followed by feature transformations, if necessary. For the current data set, because Gaussian variables are used, you do not need to perform Z-scaling. However, you can check if there is any skewness in the data and try to mitigate it, as it might cause problems during the model-building phase.

• Train/Test Split: Now you are familiar with the train/test split, which you can perform in order to check the performance of your models with unseen data. Here, for validation, you can use the k-fold cross-validation method. You need to choose an appropriate k value so that the minority class is correctly represented in the test folds.

• Model-Building/Hyperparameter Tuning: This is the final step at which you can try different models and fine-tune their hyperparameters until you get the desired level of performance on the given dataset. You should try and see if you get a better model by the various sampling techniques.

• Model Evaluation: Evaluate the models using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. Choose an appropriate evaluation metric which reflects this business goal.
