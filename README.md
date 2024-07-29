# Exploratory-Data-Analysis-Sports
In this, we will be doing an analysis of the Indian Premier League from 2008 to 2019. We will be doing various visualizations considering the factors that might affect the winning or losing of a team in the IPL. We will be exploring around factors like:
1. The most successful teams.
2. Man of the match (player). 
3. Teams that win by wickets. 
4. Teams that win by runs.
5. Player with the most wide balls.  
6. Probability of winning the match if the Toss.

<b>Data Pre-Processing: </b>
To ensure data quality and improve model accuracy, several preprocessing steps are crucial. First, identify and handle missing values by either imputing or dropping rows. Next, check for and remove duplicate records. Remove irrelevant columns to simplify the dataset and standardize column names for consistency. Identify and address outliers to mitigate their impact on statistical analysis. Validate data entries to ensure they fall within expected ranges. Handle categorical variables, such as team or player names, using techniques like one-hot encoding. For imbalanced datasets, such as IPL matches with more samples from high win-rate teams, use SMOTE to generate synthetic samples of the minority class and balance the dataset. Apply cost-sensitive learning to assign higher costs to misclassifying low win-rate teams, improving the model's performance in predicting win rates.
<br>
<br>
<b>Data Exploration: </b><br>
For the understanding of the data, I used Tableau to understand the data through various plots and charts, this was my first time using Tableau so I had to work a lot on understanding how to use which plots in Tableau but I had time crunch on my deadlines as well, so I had to gain a firm grasp on Tableau simultaneously. I made use of other python libraries to get a better understanding of the data.
<br>
<br>
<b>Feature Selection: </b><br>
Using the correlation, I was able to make the feature selection for the prediction of the win rate of the team. Features related to player performance such as batting average, bowling average, strike rate, etc. were important for predicting the outcome of a match. Similarly, team-related features such as team composition, team performance in previous seasons, and venue were also important predictors.
<br>
<br>
<b>Model Selection: </b><br>
I used SVM for its ability to handle high-dimensional and imbalanced datasets. SVM can adjust the penalty parameter for the minority class, preventing bias towards the majority class. Using cost-sensitive learning, SVM assigns higher misclassification costs to the minority class, improving performance. The optimization problem adjusts the trade-off between margin maximization and classification error. In Python, SVM with cost-sensitive learning was implemented using SVC with class weights. Hyperparameter tuning, particularly the C parameter, balanced the data. In an imbalanced IPL dataset, where some teams have higher win rates, techniques like oversampling or generating synthetic data help address bias. Besides accuracy, the F-1 score was also used, indicating a balanced model performance. The model achieved a 95.3% accuracy and an F-1 score of 0.923, validating its effectiveness in predicting team win rates.
<br>
<br>







