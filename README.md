**Fake News Detection**

This repository contains code for detecting fake news using machine learning techniques. The dataset used consists of URLs, headlines, body text, and corresponding labels indicating whether the news is fake or real.


**Dataset Overview**

The dataset comprises the following features:

URLs
Headline
Body
Label (1 for fake news, 0 for real news)


**Data Preprocessing**

Data preprocessing involved the following steps:

1. Cleaning the data to remove any noise or irrelevant information.
2. Imputation for missing values.
3. Changing the basic schema of the table to ensure uniformity.
4. Splitting the data into training and testing sets with a 70-30 ratio.
5. Vectorization of textual data to convert it into a numerical format.
6. Fitting and transforming the data to prepare it for model training.

![image](https://github.com/ayushnshrivastav/Fake_news_detection/assets/71760784/d744a79d-47ea-4adc-9800-111088bfbafc)


**WordCloud**

A WordCloud was generated to gain insights into the data by visualizing the most frequently occurring words (including stop words) in the news articles.
![image](https://github.com/ayushnshrivastav/Fake_news_detection/assets/71760784/3ff009cc-872a-4d25-9548-2eccd433fab1)


**Classification Algorithms Used**

Several classification algorithms were employed for fake news detection, including:

1. Multinomial Naive Bayes:

  Naive Bayes is a probabilistic classifier based on Bayes' theorem.
  Multinomial Naive Bayes is suitable for classification with discrete features, such as word counts.
  Algorithm Overview: Multinomial Naive Bayes is a probabilistic classifier based on Bayes' theorem with strong (naive) independence assumptions between features.
  Application: It's commonly used in text classification tasks, such as spam filtering and sentiment analysis, where the features represent word counts or term frequencies.
  Strengths: Efficient and simple to implement, even with large datasets. Works well with high-dimensional data and is relatively robust to irrelevant features.
  Achieved an accuracy of 94.35%.

  
2. Random Forest:

  Random Forest is an ensemble learning method based on decision trees.
  It creates a multitude of decision trees and combines their predictions to improve accuracy and reduce overfitting.
  Algorithm Overview: Random Forest is an ensemble learning method that constructs multiple decision trees during training and outputs the mode of the classes for classification problems.
  Application: Widely used in various domains due to its robustness and high accuracy. Suitable for both classification and regression tasks.
  Strengths: Reduces overfitting by averaging multiple decision trees. Handles high-dimensional data well and is less prone to overfitting compared to individual decision trees.
  Achieved an accuracy of 95.93%.

  
3. K-Nearest Neighbors (KNN):

  KNN is a simple algorithm that classifies data points based on the majority class of their k nearest neighbors.
  Algorithm Overview: K-Nearest Neighbors is a simple and intuitive classification algorithm that classifies data points based on the majority class of their k nearest neighbors.
  Application: Suitable for classification tasks with numerical or categorical features. Works well with small to medium-sized datasets.
  Strengths: Easy to understand and implement. Non-parametric nature allows it to adapt well to nonlinear decision boundaries.
  Achieved an accuracy of 91.19%.


4. Decision Tree:

  Decision Tree is a non-parametric supervised learning method used for classification and regression tasks.
  It splits the data into subsets based on the most significant attribute.
  Algorithm Overview: Decision Tree is a non-parametric supervised learning method that recursively splits the data into subsets based on the most significant attribute at each node.
  Application: Suitable for classification and regression tasks. Provides interpretable and easy-to-understand decision rules.
  Strengths: Simple to understand and interpret. Handles both numerical and categorical data. Can capture nonlinear relationships in the data.
  Achieved an accuracy of 95.01%.

  
5. Ensembling:

  Ensembled multiple classifiers including Multinomial Naive Bayes, Random Forest, KNN, and Decision Tree.
  Algorithm Overview: Ensembling combines the predictions of multiple classifiers to improve overall performance and robustness.
  Application: Widely used in machine learning competitions and real-world applications where high accuracy is crucial.
  Strengths: Reduces overfitting and variance by combining diverse models. Often results in higher accuracy compared to individual models.
  Achieved an accuracy of 97.01%.
  
  These algorithms were evaluated based on their accuracy in distinguishing between real and fake news articles.


**Model Analysis:**

Accuracy:
![image](https://github.com/ayushnshrivastav/Fake_news_detection/assets/71760784/f321b03c-230a-40a3-ba1d-ffe5da9e5c15)

True positive:
![image](https://github.com/ayushnshrivastav/Fake_news_detection/assets/71760784/828c8dac-b47e-4433-8aa4-eff5ed22d25d)

True Negative:
![image](https://github.com/ayushnshrivastav/Fake_news_detection/assets/71760784/61adc087-211d-4f78-af9c-3bc670f78466)

Flase Positive:
![image](https://github.com/ayushnshrivastav/Fake_news_detection/assets/71760784/eab1ba66-179e-42ed-a367-527c81b6f188)

False negative:
![image](https://github.com/ayushnshrivastav/Fake_news_detection/assets/71760784/0d13e9c3-f14b-42e4-831d-e6a455a03fdd)



**Conclusion**

This project demonstrates the effectiveness of machine learning algorithms in detecting fake news based on textual content. By preprocessing the data, generating insights through visualizations, and training various classifiers, the models were able to accurately classify news articles as real or fake.





