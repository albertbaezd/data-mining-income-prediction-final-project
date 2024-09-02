# CISC-5790 Final Project Report
## Group #5

Final project for Fordham University's Data Mining Course, Group #5

* Predicting different individual income levels based on census data.

### Presented by:
* Andres Leonardo De Los Santos
* Albert Delgado Baez
* Carlos Ferrer
* Daniela Johnson

May 6th, 2024

Reviewed by Dr. Yiyun Zhao

## 1) Introduction

In an effort to better understand economic disparities and target
socio-economic interventions, our project leverages various data mining
techniques to predict individual income levels from census data. The primary
objective is to accurately classify individuals into two income categories: those
earning above and below the $50K threshold annually.

Our analysis, based on a classification task, utilizes a diverse set of data mining
algorithms, including Decision Trees, Random Forest, K-Nearest Neighbors
(KNN), and Naive Bayes. Each of these methods brings a unique approach to
handling the complexities of the dataset.

This report outlines the methodology used in preparing and analyzing the data,
discusses the predictive models developed, and evaluates their performance.
The findings aim to provide a deeper understanding of the income dynamics
within the population and offer evidence-based recommendations for future
initiatives aimed at economic improvement.

## 2) Objectives

* Data Exploration and Preparation: To conduct a thorough analysis of the census
dataset, including data cleaning, feature selection, and preliminary data exploration to
understand the distribution and relationships of variables that might influence income
levels.

* Model Development: To implement and train various data mining algorithms—namely
Decision Trees, Random Forest, K-Nearest Neighbors (KNN), and Naive Bayes—to
create robust predictive models. The objective is to assess each model’s capability in
accurately classifying individuals based on their income levels.

* Model Comparison and Evaluation: To compare the performance of each algorithm
using metrics such as accuracy, precision, recall, and F1-score. This will help in
identifying the most effective model(s) based on the predictive accuracy and other
performance indicators.

* Feature Importance Analysis: To analyze and interpret the contribution of each
feature in the prediction models, thereby identifying key factors that most significantly
impact income levels. This analysis aims to provide insights into which characteristics
are most predictive of higher income levels.

## 3) Data Exploration and Preparation

To properly understand the existing relationships between all of our categories and values,
we need to get insights and identify patterns that may enhance our data analysis. This way,
our team also was able to identify early on possible anomalies and to improve the data
quality.

The initial phase of our project involved an in-depth exploration of the census dataset to
understand the structure, quality, and characteristics of the dataset so that we could further
prepare our dataset. This section details our findings and the steps taken to prepare the data
for further analysis.

The selected dataset consists of approximately 32,561 records and 14 features, covering a
wide range of demographic and employment-related variables. The target variable is the
income level, classified into two categories: <=50K and >50K.

**Main issues found with our data**:

* Missing values
* Data imbalance
* Data standardization
* Feature transformation
* Duplicate Rows
* Visual Data Analysis

![image](https://github.com/user-attachments/assets/6a2e8a46-a6f4-422a-b579-fe6a7b0d0806)

![image](https://github.com/user-attachments/assets/661a8092-9c84-49b2-9248-3635fc00411b)


## 4) Outcomes of each model trained

This section outlines the implementation and insights gained from implementing various
classification techniques learned in class. We tested Naive Bayes, Decision Trees, Random
Forest, and K-Nearest Neighbors (K-NN), each offering unique predictive strengths, which we
will see summarized below

### Naive Bayes

<img width="624" alt="image" src="https://github.com/user-attachments/assets/2eca1825-fd37-4fb5-a867-70126b1f9c80">

### Random Forest

<img width="624" alt="image" src="https://github.com/user-attachments/assets/464bbb7b-4c04-43be-9759-d93880ad4484">

<img width="624" alt="image" src="https://github.com/user-attachments/assets/ab269cff-8834-4d40-9878-96e20d5fb14f">

### Decision Trees

<img width="624" alt="image" src="https://github.com/user-attachments/assets/ca2a3e62-1bd8-47c2-be1e-dfec4542dcc2">

### K-Nearest Neighbors

<img width="624" alt="image" src="https://github.com/user-attachments/assets/c4e5a96b-793d-4398-9bfd-6765d042755e">


## 5) Model Selection / Closing Thoughts

Our final model selection was Random Forests using the Balanced hyperparameters, since we
want to reduce overfitting while using balanced data, after a thorough consideration process
of KNN as an alternative.

These hyperparameters, tuned by a process of 3 hours of tuning, gave us two different
perspectives on how to approach the predictions. The first one, was a set of parameters that
enabled a higher accuracy, while increasing the overfitting, while the second one loses a
small percentage of accuracy (1.4%) while it assures that the final overfitting is reduced, hence
being selected as our final model.

<img width="412" alt="image" src="https://github.com/user-attachments/assets/1549ac08-6259-4c34-aeff-cd29e8e65764">

In summary, Random Forests with Balanced hyperparameters emerged as the optimal choice
for our classification problem. This selection guarantees optimal performance on both seen
and unseen data, striking a balance between accuracy and overfitting, and ensuring the
robustness of our model across various scenarios.





