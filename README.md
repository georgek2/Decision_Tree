# Decision_Tree

 Using the DecisionTreeRegressor for ML
 
 > Model_One : All columns with categorical variables and missing values removed from the features.
 
 + Added a function to determine the best value for maximum leaf nodes
 
 > Model_Two : Imputing the missing values in the numerical columns.

 + Using the SimpleImputer function from Sk Learn.
 + The simpleImputer enables the filling of missing values in a given column. 
 + The effectiveness of this approach varies with the dataset. Meaning it have can a positive or negative          impact on your model's performance.
 + Different imputation strategies can be used. 
     * The mean, median, constant
 + Re-used the function in model one for optimum maximum leaf nodes, with the added features.
 
  > Model_Three: Imputing the numerical cols and label encoding the categorical columns with low  cardinality.
  
  + Imputing only the columns with not soo many missing values.
  + Cardinality is simply the number of unique entries in a categorical column.
  
  > Model using Pipelines.
   
   + Pipelines are better than manually imputing missing values as well as encoding the categorical variables.
   + Just declear the preprocessing steps: Set imputation strategies and the encoding to use.
   + Then, declare a preprocessor that bundles all the preprocessing steps.
   + Declare a pipeline that bundles the preprocessing steps and modelling altogether.
   + Feed the unpreprocessed training and validation sets to this pipeline.
   + Make predictions with it and valuate its performance.
  