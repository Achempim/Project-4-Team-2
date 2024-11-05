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

<<<<<<< HEAD
2. Exploratory Data Analysis (EDA)
Various visualizations, created with Matplotlib and Seaborn, are used to analyze the distribution of charges and assess relationships between variables like age, BMI, smoking status, and region. Key visualizations include:

Histograms and KDE plots for distributions of charges, age, and BMI.
Scatter plots to show relationships between charges and features like age and BMI, colored by smoker status.
Box plots and bar plots for comparisons across demographic groups and regions.

3. Model Training and Evaluation
Three models are used in this project:

Initial Random Forest Classifier: Predicts if insurance charges are above or below the median, using binary classification.
Optimized Random Forest Classifier: Improves the initial model by tuning hyperparameters with GridSearchCV.
Polynomial Linear Regression (Ridge): Uses polynomial features and ridge regularization to improve the accuracy of charge predictions.
Each model is evaluated using cross-validation:

Random Forest models: Evaluated using accuracy scores.
Polynomial Linear Regression: Evaluated with R-squared.

4. Model Optimization
Using GridSearchCV, the Random Forest model’s hyperparameters (e.g., n_estimators, max_depth, min_samples_split) are tuned to achieve better performance.

5. Model Performance Comparison
A summary of each model's performance is saved to model_optimization_results.csv, detailing the score, metric, and hyperparameters for each model. A bar plot is generated to visualize and compare the model performance.

6. Visualizations
Predicted vs. Actual Charges: A scatter plot showing the accuracy of predictions for the best-performing model.
Model Performance Comparison: A bar plot comparing the accuracy and R-squared scores of each model.
Running the Project
Requirements
Python Libraries:
pandas
numpy
pyspark
scikit-learn
matplotlib
seaborn
Install the libraries using:

bash
Copy code
pip install pandas numpy pyspark scikit-learn matplotlib seaborn
Instructions
Clone the repository and navigate to the project folder.
Ensure the insurance dataset (insurance.csv) is in the project directory or specify the correct file path.
Run the main script (insurance_analysis.py) to perform data analysis, train models, and save the results.
Example Usage
bash

Copy code
python insurance_analysis.py
Outputs
model_optimization_results.csv: Contains the performance metrics and hyperparameters of each model.
Visualizations: The script will display various plots, including distribution plots, scatter plots, and model performance comparison.
Results and Insights
This analysis provides insights into the primary factors driving insurance charges, particularly smoking status and BMI. The optimized Random Forest model and Polynomial Linear Regression model offer valuable predictions for pricing strategies, with performance visualizations aiding in model comparison.

License
This project is licensed under the MIT License.
=======
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
>>>>>>> 8d4ce1780b7f23b248ce6534daf2e2f93e5586dd
