# 🔥Machine Learning 2.0

<img src="https://github.com/AbdullahKhanKakar/Machine-Learning-2.0/blob/main/Data%20Preprocessing.png" width="100%" height="auto">

## Data Preprocessing Techniques:
Data preprocessing is a critical phase in the data analysis and machine learning pipeline, setting the foundation for accurate modeling and insightful analysis. This repository explores advanced techniques in data preprocessing, covering a variety of tasks to enhance the quality and usability of raw data.

## Topics Covered:

### 1. Data Cleaning:
   - Handle missing values effectively.
   - Remove outliers to ensure data integrity.
   - Correct errors and inconsistencies in the dataset.
   - Eliminate duplicated rows for cleaner data.

### 2. Data Integration:
   - Combine data from multiple sources for a comprehensive dataset.
   - Techniques include Data Merging and Data Concatenating.

### 3. Data Transformation:
   - Modify data formats to make them suitable for analysis and modeling.
   - **Handling Numerical Data:**
      - **Scaling:**
         - Standardization (z-score scaling): Convert data to a range of [-3,3]. Suitable for handling both positive and negative values.
         - Min-Max Scaler: Transform data to a range of [0,1], suitable for positive values.
         - MaxAbs Scaler: Convert data to a range of [-1,1], handling both positive and negative values.
         - Robust Scaler: Scale data to a range of [-1,1] and efficiently handle outliers.
      - **Normalization:**
         - Box-Cox Transformer: Transform values greater than 0, not suitable for values equal to or smaller than 0.
         - Yeo-Johnson: Improved version of Box-Cox, capable of handling both positive and negative values.
         - Log Transformer: Use numpy for logarithmic transformations, converting large values to smaller ones.

      - **Regularization:**
         - L1 Regularization (Lasso): Individually convert rows to values, ensuring their sum equals 0.
         - L2 Regularization (Ridge): Similar to Lasso but with a different method of achieving the same result.

   - **Handling Categorical Data:**
      - Label Encoding: Convert target variable categories into numeric values, especially recommended for the target variable.
      - One-Hot Encoding: Convert categorical values into a binary matrix format, suitable for unordered categories.
      - Ordinal Encoding: Convert categorical values with ordinal relationships into numerical format.

### 4. Data Discretization or Binning:
   - Convert continuous data into discrete bins or categories for improved analysis and modeling.

---------------------------

<img src="https://github.com/AbdullahKhanKakar/Machine-Learning-2.0/blob/main/ML%20Algorithms.png" width="100%" height="auto">

## ML Algorithms

# 1. Linear Regression:

Linear regression is a statistical method used to model the relationship between a dependent variable and one or more independent variables. The core idea is to fit a linear equation to the observed data in order to describe the statistical association between variables. `The main goal in Linear Regression is to minimize the sum of squared distances between observed values of Y and the values predicted by the linear equation.`

### There are 2 types of Linear Regression
- **Simple Linear Regression:** Involves a single independent variable.
- **Multiple Linear Regression:** Involves more than one independent variables.

### Formula to find linear equation:
           basic equation:
               Y = mx + c or Y = B1.X + B0
               Y = B0 + B1.X1 + B2.X2 + B3.X3 + .... + BnXn
           where,
               - Y is independent variable
               - B0 is y-intercept, calculating by setting x=0, as (0,y)
               - B1,B2,B3, ... ,Bn are slopes, calculated by using slope formula: slope=m=rise/run=(y2-y1)/(x2-x1)

### Selecting best linear equation:
- **How first linear equation comes?** It based on estimations of slope and y-intercept. This is done by using OLS(order least squares)
- **How best line comes?** After first line calculation, the distance of points from the line is calculated by taking their squares and adding them. A single value come which is usually referred as error. Similarly, algorithm tries different linear equations and select the best one that have minimum error.

### Performance Evaluation Metrics:
There are many ways to measure performance of Linear Regression models. But main or important metrics are:
- **MSE(Mean Squared Error)**
- **RMSE(Root Mean Squared Error)**
- **R-Squared Error(also called r-2 score)**
- **MAE(Mean Absolute Error)**

# 2. Logistic Regression:

Logistic regression is a statistical method used for binary classification problems, where the outcome variable is categorical. Despite its name, logistic regression is a classification algorithm rather than a regression algorithm.

### There are 3 types of Classifications in Logistic Regression:
- **Binary Classification(use sigmoid function method):** Target variable have exactly 2 classes e.g., True, False or Male, Female etc.
- **Multiclass Classification(use softmax function method):** Target variable have more than 2 classes, each instance belongs to one class e.g, different colous Red, Green, Orange, Blue in target variable etc.
- **Multilabel Classification:** Target variable have more than 2 classes, each instance can belongs to multiple classes e.g, there are 3 classes Movies, Cartoons, Anemy. The Movies instance can belongs to multiple classes e.g, Action, Horror etc.

### Performance Evaluation Metrics:
There are many ways to measure performance of Logistic Regression models. But main or important metrics are:
- **Accuracy Score**
- **Recall Score**
- **Precision Score**
- **Confusion Matrix**
- **F1 Score**

## Math Behind Sigmoid or Ligit Function:
The sigmoid function, denoted as **σ(z)**, is a mathematical function that convert any real number **z** into a range between **0 and 1**. It's often used in machine learning for tasks like **binary classification**, where you want to predict **probabilities**.

      Mathematically, sigmoid function is represented as:
            σ(z) = 1/(1+e^-z)
      Here,
            **σ(z)**: This is the output of the sigmoid function. It represents the probability of an event happening.
            **e**: This is Euler's number, a mathematical constant approximately equal to 2.71828.
            **z**: This is the input to the sigmoid function

Here, actually **z == mx + b**. During training sigmoid will learn the values of m(slope) and b(y-intercept). This equation can be represented as **z = B0 + B1.X**

## Softmax Function:
For multiclass classification problems, the softmax function is commonly used. The softmax function takes a vector of raw scores (also known as logits) and transforms them into a probability distribution over multiple classes. This ensures that the predicted probabilities sum to 1.

# 3. Support Vector Machine(SVM):
It can be used for both classification and regression problem.

#### For more read: here is my blog on SVM 👉 <a href="https://medium.com/@abdullahkhan4465917/support-vector-machines-svm-96a66699721a">Click</a>

# 4. K-Nearest Neighbors(KNN):
K-Nearest Neighbors (KNN) is a simple supervised machine learning algorithm used for both classification and regression tasks. The fundamental idea behind KNN is to make predictions based on the majority class (for classification) or average (for regression) of the K-nearest data points in the feature space.

**KNN calculate distance of given point from nearest points through following techniques:**
- **i. Euclidean Distance:** It calculates direct distance between two points e.g, as we move through Airplane from one country(point) to another.
              d=sqrt((x2​−x1​)2+(y2​−y1​)2)​
- **ii. Manhattan Distance:** It calculates indirect distance between two points e.g, as we move through Car from one country(point) to another.
              d=∣x2​−x1​∣+∣y2​−y1​∣
- **iii. Minkowski Distance:** It's usually combination of both distances. Means through this techniques, we can calculate any distance(whether Euclidean or Manhattan).
              d= (∣x2​−x1​∣p + ∣y2​−y1​∣p)1/p
              Here, **p** is a positive real number, which defines the order of the Minkowski distance. When p=2, it becomes the Euclidean distance, and when p=1, it becomes the                       Manhattan distance
- **iv. Hamming Distance:** Hamming distance is a measure of the difference between two strings of equal length. It counts the number of positions at which the corresponding symbols (characters or bits) are different. Hamming distance is often used in information theory and error detection. It's use in NLP domain.

# 5. Decision Tree:
Decision is a supervised machine learning algorithm used for both classification and regression tasks. It splits the dataset into subsets on the most significant column at each level of tree. The goal is to **create a tree** that able to predicts the target variable by learning simple decision rules from data features(means from training dataset).- 

### Elements used in Decision Tree:
- **Root Node:** The top node in the tree is called Root Node. It represents the entire dataset and splits into child nodes based on the most significant columns.
- **Decision Nodes(internal nodes):** These nodes represents the decisions or tests based on a specific column. Each decision node is further split into two or more child nodes.
- **Leaf Nodes(terminal nodes):** These nodes represents the final outcomes or predictions. Each leaf node corresponds to a class label in classification task and to numerical value in regression tasks.
- **Branches:** The edges connecting nodes are called branches.
- **Pruning:** Pruning helps to reduce the unnecessary nodes. It reduce overfitting and improves the model for better predictions on unseen data.
- **Entropy and Information Gain:** Entropy is used for measuring impurity(it's mixture of data). Information Gain measures the effectiveness of feature in reducing entropy. Decision Trees aims to maximize information gain.









 
