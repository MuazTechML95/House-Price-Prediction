🏠 House Price Prediction Using Linear Regression
Project Overview
This project focuses on predicting house prices based on property features using a Linear Regression model. The workflow covers data preprocessing, feature engineering, model training, evaluation, and result interpretation.

1. Data Acquisition


Loaded the housing dataset (housing.csv) into a Pandas DataFrame.


Explored the dataset to examine rows, columns, and data types.



2. Data Cleaning


Missing Values Handling:


Numeric columns: Imputed with mean or median.


Categorical columns: Imputed with mode.




Removed irrelevant or non-informative columns (e.g., Id, MiscFeature, PoolQC).



3. Feature Encoding


Converted categorical features into numerical format using one-hot encoding.


Ensured no duplicate columns or data type inconsistencies remained.



4. Feature Selection


Selected features relevant to predicting house prices.


Dropped highly irrelevant or redundant features to improve model performance.


Target variable: SalePrice.



5. Train-Test Split


Split the dataset into training (80%) and testing (20%) sets.


Ensured no data leakage between train and test sets.



6. Model Training


Trained a Linear Regression model on the training set.


Linear Regression was selected as the baseline model for this task.



7. Model Evaluation


Predicted house prices on the test set.


Evaluated performance using:


RMSE (Root Mean Squared Error): 0.40


MAE (Mean Absolute Error): 0.29


R² Score: 0.67





8. Interpretation of Results


Analyzed model coefficients to understand feature impact:


Positive coefficients: Features that increase house prices.


Negative coefficients: Features that decrease house prices.




Identified key factors influencing house prices.



9. Model Saving


Saved the trained Linear Regression model using joblib.


Enables loading the model later to make predictions on new data without retraining.



10. Conclusion & Future Work


Linear Regression provides a baseline for house price prediction with moderate accuracy (R² ~ 0.67).


Model performance can be improved with:


Feature engineering and interaction terms


Scaling or transforming the target variable


Exploring advanced regression techniques
