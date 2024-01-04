# 🔥Machine Learning 2.0

<img src="https://github.com/AbdullahKhanKakar/Machine-Learning-2.0/blob/main/Data%20Preprocessing.png" width="100%" height="auto">

## Data Preprocessing Techniques:
Data preprocessing is a critical phase in the data analysis and machine learning pipeline, setting the foundation for accurate modeling and insightful analysis. This repository explores advanced techniques in data preprocessing, covering a variety of tasks to enhance the quality and usability of raw data.

## Topics Covered:

### 1. <span style="color: #ff0000;">Data Cleaning:</span>
   - Handle missing values effectively.
   - Remove outliers to ensure data integrity.
   - Correct errors and inconsistencies in the dataset.
   - Eliminate duplicated rows for cleaner data.

### 2. <span style="color: #00ff00;">Data Integration:</span>
   - Combine data from multiple sources for a comprehensive dataset.
   - Techniques include Data Merging and Data Concatenating.

### 3. <span style="color: #0000ff;">Data Transformation:</span>
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

### 4. <span style="color: #ff00ff;">Data Discretization or Binning:</span>
   - Convert continuous data into discrete bins or categories for improved analysis and modeling.
