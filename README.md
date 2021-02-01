# Machine Learning - Exoplanet Exploration

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

This project aims to build machine learning models to classify exoplanets from the raw dataset. 

![exoplanets.jpg](Images/exoplanets.jpg)

I built two different machine learning models -Logistic Regression and Random Forest Classifier to classify the exoplanets. Find below a detailed summary of the process used to build these models and a detailed report about the two models' findings and performance comparison.

## Data Exploration
* Read the data from CSV file into a dataframe
* Cleaned the dataset by eliminating columns and rows containing null values
* Analysed the data features
* Checked data unbalance in target value, i.e., Class

![Data_Unbalance_In_Target_Values.png](Images/Data_Unbalance_In_Target_Values.png)

## Model 1 - Logistic Regression
Followed the below process to create a Logistic Regression model that classified the exoplanets.

### Data Preprocessing
* Defined predictors and target values
* Used `MinMaxScaler` to scale the numerical data.

### Model Evaluation with all 40 features
* Separated the data into training and testing data.
* Trained the model and evaluated the model against test dataset.
* Used `GridSearch` to tune model parameters.
* Evaluated model performance
```
Training Data Score: 0.8897577722677856
Testing Data Score: 0.88558352402746
```
