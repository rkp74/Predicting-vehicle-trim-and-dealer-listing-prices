# Predicting-vehicle-trim-and-dealer-listing-prices
Data Science Project



In this project, I tackled the challenge of predicting vehicle trim and dealer
listing prices using a dataset of used car listings. The provided dataset,
comprising various parameters related to the transactions, served as the
foundation for constructing predictive models.

● My Approach:-
1. Importing and Setup:
The implementation begins with importing essential libraries, including
Pandas, NumPy, XGBoost, and others. These libraries facilitate data
manipulation, visualization, modeling, and hyperparameter tuning.

2. Defining Functions:-
The approach adopts a modular structure by defining functions for data
exploration, cleaning, and transformation, as well as hyperparameter tuning
and evaluation metrics. This design enhances code readability and
promotes reusability.

3. Dataset Loading:-
The provided CSV files are loaded using Pandas to create the training
and test datasets. This forms the foundation for subsequent analysis and
modeling.

4. Exploration and Transformation:-
Exploratory Data Analysis (EDA) was conducted using visualizations with
Seaborn and Matplotlib. I handled missing values, encoded categorical
variables using OneHotEncoder and LabelEncoder, and standardized
numerical features.

5. Modeling Trim:-
Two separate models are built for predicting vehicle trim and dealer listing
prices. XGBoost is employed as a machine learning algorithm, utilizing the
XGBClassifier for classification (trim) and the XGBRegressor for regression
(price) tasks. This choice of algorithm is appropriate, as XGBoost is known
for its effectiveness in handling both classification and regression problems.
I created a pipeline that encompassed data preprocessing, dimensionality
reduction (PCA), and XGBoost modeling.

6. Hyperparameter Tuning:-
The approach demonstrates the use of Hyperopt for hyperparameter
tuning. The fmin function from Hyperopt is used with the TPE (Tree of
Parzen Estimators) algorithm. This allows the models to be fine-tuned for
optimal performance on the training data.

7. Predicting Trim for the Test Dataset:-
The trained XGBoost model was used to predict vehicle trim for the test
dataset ('Test_dataset.csv'). Predictions were stored in a CSV file for
submission.

8. Modeling Dealer Listing Price:
For predicting dealer listing prices, I employed the XGBoostRegressor.
Similar preprocessing and hyperparameter tuning were applied.

9. Metrics on Test Data:
Model performance was evaluated using appropriate metrics such as
R-squared, AUC, accuracy, and regression error metrics (MSE, MAE, etc.).

10. Saving Predictions as CSV
Predicted values for both vehicle trim and dealer listing price were saved
as a CSV file, satisfying the project's submission requirements.

● Reasoning:-
The chosen approach combines data preprocessing, feature engineering,
and model building, utilizing XGBoost as the machine learning algorithm
due to its versatility in handling both classification and regression tasks.
The inclusion of Hyperopt for hyperparameter tuning reflects the emphasis
on optimizing model performance. The use of various evaluation metrics
and the saving of predictions in a structured format align with the practical
goal of assessing and presenting the model's accuracy.'

● Conclusion:-
This project combined rigorous data analysis, thoughtful modeling, and
efficient hyperparameter tuning to create predictive models capable of
estimating vehicle trim and dealer listing prices. The methodologies
employed demonstrate the effectiveness of machine learning techniques in
solving real-world problems related to the automotive domain.
