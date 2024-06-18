Dataset: https://www.kaggle.com/datasets/sahirmaharajj/college-exam-results-sat
Summary of Analysis and Modeling
Dataset Description:
The dataset contains SAT scores for various schools, including the number of test takers and mean scores in critical reading, mathematics, and writing. The columns are:

DBN: School code
School Name: Name of the school
Number of Test Takers: Number of students who took the test
Critical Reading Mean: Mean score in critical reading
Mathematics Mean: Mean score in mathematics
Writing Mean: Mean score in writing
Steps Performed:

Data Loading and Initial Exploration:

Loaded the dataset using pandas.
Displayed the first few rows and summarized the dataset to understand its structure.
Identified missing values in the dataset.
Data Cleaning:

Dropped rows with missing values to ensure a clean dataset for analysis.
Converted the 'Number of Test Takers' column to integer type for consistency.
Exploratory Data Analysis (EDA):

Visualized the distribution of SAT scores (critical reading, mathematics, and writing) using histograms.
Examined the relationships between the number of test takers and mean scores using scatter plots.
Predictive Modeling:

Selected 'Critical Reading Mean' and 'Mathematics Mean' as predictor variables to predict 'Writing Mean'.
Split the dataset into training (80%) and testing (20%) sets.
Trained a linear regression model on the training data.
Made predictions on the testing data.
Model Evaluation:

Evaluated the model using Mean Squared Error (MSE) and R-squared metrics.
Mean Squared Error (MSE): 106.56 (lower MSE indicates better fit)
R-squared: 0.967 (high R-squared indicates that 96.7% of the variance in the writing scores is explained by the model)
Visualized the model's performance by plotting actual vs predicted writing scores.
Results:
The linear regression model demonstrated excellent performance, with a high R-squared value (0.967), indicating that the model explains a significant portion of the variance in writing scores. The low MSE (106.56) further confirms the accuracy of the predictions. The scatter plot of actual vs predicted writing scores showed that most points are close to the 45-degree line, validating the model's predictive power.
