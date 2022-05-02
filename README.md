# Machine Failure Predictor
An ML model that uses a Decision Tree Classification Algorithm to predict what type of machine failure will occur given a set of operating variables.

## Steps
1. Imported the data from a kaggle csv file: https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification.
2. Cleaned the data using pandas.
3. Split the Data into Training/Test Sets using sklearn.model_selection.
4. Created a Decision Tree Classifier Algorithm model using sklearn.tree.
5. Trained the model to an average accuracy above 97% using sklearn.metrics.
6. Created a Persisting Model by dumping then loading the trained and tested model with joblib.
7. Created a Tree Graph Viz using sklearn.tree.

### About Dataset
The dataset consists of 10,000 data points stored as rows with 6 features in columns:
•	air temperature [K]: generated using a random walk process later normalized to a standard deviation of 2 K around 300 K
•	process temperature [K]: generated using a random walk process normalized to a standard deviation of 1 K, added to the air temperature plus 10 K.
•	rotational speed [rpm]: calculated from powepower of 2860 W, overlaid with a normally distributed noise
•	torque [Nm]: torque values are normally distributed around 40 Nm with an Ïƒ = 10 Nm and no negative values.
•	tool wear [min]: Minutes of tool wear to the used tool in the process.
•	Failure_Type: Type of failure as a result of given operating variables. 


