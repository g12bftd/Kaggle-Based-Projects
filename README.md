# Real-World Applications of Machine Learning
A few of the projects I completed on my machine learning journey.
The datasets used are all publically available on platforms such as Kaggle and Super Data Science.


## 1) Breast Cancer Classification (SVC)

Objective: Given features regarding breast tumors, we wish to classify these tumors as either benign or malignant

30 features are used, examples include:
- radius (mean of distances from center to points on the perimeter)
- texture (standard deviation of gray-scale values)
- perimeter
- area
- smoothness (local variation in radius lengths)
- compactness (perimeter^2 / area - 1.0)
- concavity (severity of concave portions of the contour)
- concave points (number of concave portions of the contour)
- symmetry
- fractal dimension ("coastline approximation" - 1)

Datasets are linearly separable using all 30 input features Number of Instances: 569 Class Distribution: 212 Malignant, 357 Benign Target class:
Malignant
Benign https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)

Using Support Vector Classification, we build a model to predict whether a tumor is benign or malignant.

## 2) Customer Subscription Behavior Analysis

We are working for a fintech company that wants to provide customers with a paid mobile app subscription that will allow them to track their finances.
To attract customers, the company releases a free version of the app.
The task is to identify which users will most likely NOT purchase the paid version of the app, so that additional offers can be provided to them. Accuracy is key, because increased targeted advertising is costly.

Our dataset features:
- User ID
- Day and time at which the user first opened the app
- Day of the week (numerical) at which the user first opened the app
- Hour of the day at which the user first opened the app
- User age
- Screen list: every screen name visited by user in the app
- Number of screens visited in the app by the user
- Whether the user played the available minigame
- Whether the user gave a "like" rating to the app
- Whether the user used the app's premium feature
- Whether the user enrolled in the paid product
- The date of enrolment (if any)

Using Logistic Regression, we build a model to predict whether a customer has enrolled in the app's paid version.

## 3) Fashion Class Classification

Given a series of images, we want to build a machine learning model that is able to identify the fashion content of each image. Examples of classes include shorts, bags, dresses etc.

This is a simpler, smaller version of the Amazon Echo Look Style Assistant.
Applications could have real life benefits. By idenitifying most liked images on social media platforms, we could provide targeted advertisements that stay on top of fashion trends.

Our dataset will contain 70, 000 images:
60,000 for training
10, 000 for testing
Images are 28 x 28 grayscale
There will be 10 target output classes.

A note on greyscale:
System of 256 tones ranging from 0-255
0 represents black and 255 represents white
Therefore, each image will be represented by a row of 28x28 = 784 values to encode its grayscale values.

Detailed dataset info from Kaggle:
Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes. Zalando intends Fashion-MNIST to serve as a direct drop-in replacement for the original MNIST dataset for benchmarking machine learning algorithms.
Each training and test example is assigned to one of the following labels:
0 T-shirt/top
1 Trouser
2 Pullover
3 Dress
4 Coat
5 Sandal
6 Shirt
7 Sneaker
8 Bag
9 Ankle boot

Using a convolutional neural network, we predict which of the 10 items of fashion feature in any given image.

## 4) Logistic Regression - Breast Cancer (UCI ML Repo Dataset)

Objective: Given features regarding breast tumors, we wish to classify these tumors as either benign or malignant

30 features are used, examples include:
- radius (mean of distances from center to points on the perimeter)
- texture (standard deviation of gray-scale values)
- perimeter
- area
- smoothness (local variation in radius lengths)
- compactness (perimeter^2 / area - 1.0)
- concavity (severity of concave portions of the contour)
- concave points (number of concave portions of the contour)
- symmetry
- fractal dimension ("coastline approximation" - 1)

Datasets are linearly separable using all 30 input features Number of Instances: 569 Class Distribution: 212 Malignant, 357 Benign Target class:
Malignant
Benign https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)

Using Logistic Regression, we build a model to predict whether a tumor is benign or malignant.

## 5) Minimizing Churn Rate

Objective: to predict which users are most likely to churn, thereby allowing the company to re-engage/advertise to these users.
We're working for a fintech company that has a subscription product that allows a user to manage their finances.
Data:
We will have access to users' finances and how they handle finances through the product.
We also have demographic info acquired from sign-up process
Caveat: financial data can be unreliable and delayed, so companies are more likely to use demographic data instead.
Dataset - Our dataset will include fields such as:
- User ID
- Whether they churned (0 or 1) response variable
- Age
- Housing (na, R = renting, O = owner)
- Credit score
- Deposits = number of deposits
- Withdrawals = number of withdrawals
- Purchases = how many purchases outside of company partner stores
- Purchases_special = number of purchases with company partner stores
- CC_taken = number of credit cards
and more...

Using Logistic Regression, we build a model to predict whether or not a given user has churned (i.e. no longer interested in the company product).

## 6) Project - Sales Analysis

Given 12 months of sales data, we use the Pandas library to answer the following questions:
1) What was the best month of sales? How much revenue was made?
2) What city has the highest number of sales?
3) What is the best time of the day to advertise to customers?
4) What products are most often sold together in pairs?
5) Which product is sold the most?

## 6) Credit Card Fraud Detection

We are working for an e-commerce company and will use past transactional data to detect potential fraud.

- Our dataset is slightly unusual. 
- We have 284807 transactions and 31 different columns
- We have 29 unknown columns and numeric values.

This is appropriate in this business environment because customers and their information should ideally remain anonymous. One column denotes how many times the customer has purchased goods on our platform.
- One column denotes how much money the user has spent on our platform in total.
- The response variate denotes whether the transaction is fraudulent.

Using random forest and decision tree classification as well as a dense sequential neural network, we aim to predict whether any given transaction is legitimate or fraudulent.¨

## 7) E-Signing Loans & Financial History

We work for a fintech company that specializes in loands. It offers low APR loans to applicants based on their financial habits. The company has partnered with a peer-to-peer lending marketplace that provides real time loan applicants.

We aim to develop a model to predict whether loan applicant will complete the electronic signature phase of the loan application. The company will leverage the model to identify "low quality" applicants and experiment with different onboarding screens.

Our dataset includes features such as:
- Age
- Pay schedule (weekly, monthly, bi-weekly, semi-monthly etc.)
- Home owner (y/n)
- Has debt
- Annual income
- Years of employment
- Time user has had a personal bank account 
- Risk score 
- e-signed (y/n) = our response variable

etc...


Our dataset has 908 entries and 21 columns

We use logistic regression, linear SVM, radial SVM and random forest classification to build 4 machine learning models to address the given challenge. Using 10-fold cross validation and grid searching of hyperparameters with respect to the accuracy metric, we identify the best model with the best parameters for this problem.  

## 8) Combined Cycle Power Plant Project


Data Set Information:

The dataset contains 9568 data points collected from a Combined Cycle Power Plant over 6 years (2006-2011), when the power plant was set to work with full load. Features consist of hourly average ambient variables Temperature (T), Ambient Pressure (AP), Relative Humidity (RH) and Exhaust Vacuum (V) to predict the net hourly electrical energy output (EP) of the plant.

A combined cycle power plant (CCPP) is composed of gas turbines (GT), steam turbines (ST) and heat recovery steam generators. In a CCPP, the electricity is generated by gas and steam turbines, which are combined in one cycle, and is transferred from one turbine to another. While the Vacuum is colected from and has effect on the Steam Turbine, he other three of the ambient variables effect the GT performance.
For comparability with our baseline studies, and to allow 5x2 fold statistical tests be carried out, we provide the data shuffled five times. For each shuffling 2-fold CV is carried out and the resulting 10 measurements are used for statistical testing.

Attribute Information:
- Features consist of hourly average ambient variables
- Temperature (T) in the range 1.81°C and 37.11°C,
- Ambient Pressure (AP) in the range 992.89-1033.30 milibar,
- Relative Humidity (RH) in the range 25.56% to 100.16%
- Exhaust Vacuum (V) in teh range 25.36-81.56 cm Hg
- Net hourly electrical energy output (PE) 420.26-495.76 MW

The averages are taken from various sensors located around the plant that record the ambient variables every second. The variables are given without normalization.

More info available at https://archive.ics.uci.edu/ml/datasets/Combined+Cycle+Power+Plant

We aim to use a densely-connected neural network to predict net hourly electrical energy output based on our 4 predictors listed above.
