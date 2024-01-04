# Machine Learning 2.0

## Data Preprocessing:
Data preprocessing is a crucial step in the data analysis and machine learning pipeline. It involves several sub-tasks to prepare raw data for further analysis or modeling. The following topics are included in data preprocessing:

<ol>
  <li>Data Cleaning:
    <ul>
      <li>Handling `missing values`</li>
      <li>Removing `outliers`</li>
      <li>Correct `errors and inconsistency` from the dataset</li>
      <li>Removing duplicated rows</li>
    </ul>
  </li>
  <li>Data Integration:
    <ul>
      Combining data from multiple resources into a single dataset from more comprehensive analysis. It includes two techniques that are popular:
      <li>Data Merging</li>
      <li>Data Concatenating</li>
    </ul>
  </li>
  <li>Data Transformation:
    <ol>
      Modify the format or structure of the data to make it more suitable for analysis or modeling.
      <li>Handling Numerical Data
        <ol>
          <li>Scaling
            <ul>
              Method of converting data in equal range units. Using scikit-learn library for doing this, which offer us various methods.
              <li>Standardization(also called z-score scaling): `Convert data in range of [-3,3]. It can handle both +ve and -ve values`</li>
              <li>Min-Max Scaler: `Convert data in range of [0,1]. It can handle only +ve values. It cannot be applied to -ve values data points.`</li>
              <li>MaxAbs Scaler: `Convert data in range of [-1,1]. It can also handle both +ve and -ve values.`</li>
              <li>Robust Scaler: `Convert data in range of [-1,1]. Alongwith scaling, it also handle outliers effeciently.`</li>
            </ul>
          </li>
          <li>Normalization
            <ul>
              It includes Power Transformers, which helps to do scaling and also helps to normally distribute the data. Using scikit-learn library for doing this, which offer us various methods.
              <li>Box-Cox Transformer: `It handle values greater than 0. Not able to handle values equal to 0 and smaller than 0.`</li>
              <li>Yeo-Johnson: `It's just improvement in Box-Cox transformers. It able to handle both +ve and -ve values.`</li>
              <li>Log Transformer: `We can use it through numpy. Scikit-learn don't offer any method to do this task. It also convert large values into little smaller values.`</li>
              <li>
            </ul>
          </li>
          <li>Regularization</li>
        </ol>
      </li>
      <li>Handling Categorical Data</li>
    </ol>
  </li>
</ol>
