# Project-4-Team-2

Overview

An evaluation of health insurance cost data collected regionally throughout the United States(US). 


How to utilize the information for future uses

1. Download the attached project files and imports as necessary.
2. Initialize a Spark Session to import the CSV data and to convert to a Pandas DataFrame.
![alt text]("C:\Users\ormis\Desktop\Project-4-Team-2\Images\Screenshot 2024-11-04 202333.png")


3. After initializing the Spark session. We cleaned and standardized the data to prepare for modeling.



4. After converting categorical values for one-hot encoding. The feature 'charges' was selected as the target variable and data was split into Training and Test sets.
Charges represents the amount of healthcare costs to the individual.

5. The initial model was evaluated through LinearRegression. The initial R-squared value was 0.73 and the initial Random Forest Classification Accuracy was 0.92.

6. Additional optimization through the use of sklearn and additional parameters. The new R-Squared value was 0.78 and Random Forest Classification Accuracy was 0.94.

7. The process and results both were converted to a Pandas DataFrame and saved to a CSV.