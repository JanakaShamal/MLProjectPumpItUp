# Pump It Up: Data Mining the Water Table  – 170576J

**Procedure:**
1.	Understanding the data – There are lot of categorical data with many unique values in the dataset. So it is needed to encode those data by using relevant encoding techniques. And also, this is a multi-target (multi-class) program.
2.	Exploratory data analysis (EDA)
  focused on data types, distribution, null, zero & missing values in the dataset and filled them with the mean (numerical columns), Unknown or most frequently occurred values (categorical values).
3.	Drop features
  After data analyzing step, dropped quantity_group, source_class, source_type, quality_group, payment_type, extraction_type_class, extraction_type & waterpoint_type_group columns. These columns are not very useful because some of the data & information in these columns are also in the other columns of the dataset or target value doesn’t depend on these features. 
4.	Data preparing
  -	Encoding categorical variables using Label Encoding.
  - Scaling data using robust scaling (doesn’t increase the accuracy)
5.	Feature selection.
  - Sequence feature selection techniques to identify features with high accuracy
    -	Random Forest
    -	XGBoost
    -	CatBoost
    -	KNN
  -	Correlation analyzing
  -	Training data on Random Forest and Selecting most important features by using feature rankings.
6.	Generating new features using PCA & check for the accuracy gain.
7.	Training & evaluating models using 5-fold cross validation
  -	Random forest (highest accuracy)
  -	Catboost
  -	XGBoost




