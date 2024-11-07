# Project-4-Team-2

Insurance Charges Analysis and Model Optimization
Project Overview
This project analyzes insurance charges based on demographic and health-related factors, with the goal of identifying key drivers that influence insurance premiums. Additionally, it includes model training and optimization steps to predict insurance charges and compares different machine learning models to assess their performance.

The project involves data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning, and results visualization. It aims to uncover insights for insurers to optimize pricing strategies and provide personalized policy recommendations.

Repository Structure
insurance_analysis.py: The main code file containing data loading, preprocessing, model training, and visualization.
model_optimization_results.csv: A CSV file generated to store the performance and hyperparameters of each model.
README.md: Project documentation.
Project Steps

1. Data Loading and Preprocessing
The data is loaded using PySpark and converted to a Pandas DataFrame. After removing missing values, categorical variables are converted to numeric using one-hot encoding, and numerical features are standardized.

1. Download the attached project files and imports as necessary.
2. Initialize a Spark Session to import the CSV data and to convert to a Pandas DataFrame.
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Screenshot%202024-11-04%20202333.png)
3. After initializing the Spark session. We cleaned and standardized the data to prepare for modeling.
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Cleaning%20data.png?raw=true)
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Standardized%20values.png?raw=true)
4. After converting categorical values for one-hot encoding. The feature 'charges' was selected as the target variable and data was split into Training and Test sets.
Charges represents the amount of healthcare costs to the individual.
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Train%20and%20Test%20Set%20split.png?raw=true)
5. The initial model was evaluated through LinearRegression. The initial R-squared value was 0.73 and the initial Random Forest Classification Accuracy was 0.92.
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Initial%20model%20evaluation%20.png?raw=true)
6. Additional optimization through the use of sklearn and additional parameters. The new R-Squared value was 0.78 and Random Forest Classification Accuracy was 0.94.
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Optimization.png?raw=true)
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Optimization%202.png?raw=true)
7. The process and results both were converted to a Pandas DataFrame and saved to a CSV.
![alt text](https://github.com/Achempim/Project-4-Team-2/blob/main/Images/Process%20Results%20Save.png?raw=true)
