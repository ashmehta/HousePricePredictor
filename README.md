#HousePricePredictor
Overview

This project aims to predict the median house value in Boston suburbs using a variety of features. The dataset consists of various characteristics of the houses, such as the number of rooms, crime rate, property tax rate, and other socio-economic factors.

Dataset

The dataset is sourced from the Boston Housing dataset available via UCI Machine Learning Repository. The dataset has 506 rows and 14 columns, where each row represents a suburb in Boston, and the target variable is the median house value (medv).

Columns:
CRIM: Crime rate per capita
ZN: Proportion of residential land zoned for large lots
INDUS: Proportion of non-retail business acres per town
CHAS: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
NOX: Nitrogen oxide concentration (parts per 10 million)
RM: Average number of rooms per dwelling
AGE: Proportion of owner-occupied units built before 1940
DIS: Weighted distance to employment centers
RAD: Index of accessibility to radial highways
TAX: Property tax rate per $10,000
PTRATIO: Pupil-teacher ratio by town
B: Proportion of residents of African American descent
LSTAT: Percentage of lower status population
medv: Median value of owner-occupied homes in $1000s (target variable)
Approach

1. Data Cleaning
Checked for missing values and found no missing data in the dataset.
Ensured that all data types were correctly assigned for further analysis.
2. Exploratory Data Analysis (EDA)
Performed univariate analysis to visualize the distribution of the target variable medv (Median House Value).
Created scatter plots to explore relationships between features (e.g., number of rooms and house price).
Analyzed correlations between the features and the target variable using a correlation heatmap.
3. Feature Engineering
Scaled the numeric features using StandardScaler to standardize the dataset.
Used the scaled features for training the model.
4. Modeling
Used Linear Regression as a baseline model to predict house prices.
Split the data into training (80%) and testing (20%) sets.
Trained the model and evaluated it using Mean Squared Error (MSE) and R-squared.
Baseline Model Results:

Mean Squared Error (MSE): [Insert MSE value here]
R-squared: [Insert R-squared value here]
Visualizations

Distribution of Median House Value (medv):
The histogram showed the distribution of house prices across the suburbs, with a slight skew towards lower prices.
Relationship between Average Number of Rooms (RM) and Median House Value (medv):
A scatter plot was used to show the positive correlation between the average number of rooms and house prices, indicating that larger houses tend to have higher prices.
Correlation Heatmap:
A heatmap revealed that RM (average number of rooms) and LSTAT (percentage of lower status population) are strongly correlated with medv.
Conclusions

The analysis reveals that the average number of rooms (RM) and the percentage of lower status population (LSTAT) are two key features that strongly influence the median house value.
The baseline model using Linear Regression showed a decent performance but can be improved with more advanced techniques like decision trees, random forests, or boosting methods.
Next Steps

Experiment with more complex machine learning algorithms.
Fine-tune hyperparameters for better model performance.
Perform cross-validation to assess the model's generalization.
