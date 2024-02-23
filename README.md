# RAPIDMINER STUDIO
RapidMiner is a Data Analytics and Data Science tool which provides the user all the
interactions with the data from preprocessing stage to model evaluation stage without
any use of programming language.
This RapidMiner is intended to support all the functionalities across the AI ecosystem.

## Prerequisites:
The major prerequisites required before using this tool, One should be aware of
basic calculus, algebra, Excel and basic workflow of machine learning models.

# BUSINESS ANALYTICS: DATA, MODELS AND DECISIONS
## Lab Assignment 1

### a)Data Quality Check:
a.1) In RapidMiner Studio, the data quality is checked by using the “Data Quality” operator. This operator  detect any bias in the dataset by calculating descriptive statistics of the dataset and visualizing the distribution of the data. It can also detect outliers and missing values. The “Data Quality” operator also provides information about the number of rows and columns in the dataset. 
a.2) To handle the data quality issues such as duplications and missing values, the “Data Cleansing” operator is  used. This operator allows the user to select the columns to be cleaned and specify the rules for cleaning the data. For example, the user can specify the rule to remove all duplicate values or to replace missing values with the median of the column feature in that specific “Region” variable. 
a.3) The number of rows and columns in the dataset is 18249 and 13, respectively.
### b)Data Cleaning and Preprocessing: 
b.1)In RapidMiner Studio, the first column in the dataset is removed by using the “Select Attributes” operator. This operator allows the user to select or deselect the attributes that should be included in the dataset. The ‘year’ variable can be treated as nominal by using the “Nominal to Numeric” operator. This operator allows the user to convert the nominal values to numeric values. 
![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/a1456d27-36f7-4562-85df-059180cf1f84)

b.2)To check for duplicate values and remove them, the “Data Cleansing” operator is used. This operator allows the user to select the columns to be cleaned and specify the rules for cleaning the data. For example, the user can specify the rule to remove all duplicate values. 
 ![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/3f102984-bfa7-4b4b-8725-0d13c4af6525)

b.3)To check for missing values, the “Data Cleansing” operator is also used. This operator allows the user to select the columns to be cleaned and specify the rules for cleaning the data. For example, the user can specify the rule to replace missing values with the median of the column feature in that specific “Region” variable. If most column values in a data record are missing, the data record can be removed. The correlation between the variables is found by using the “Correlation Matrix” operator. This operator calculates the correlation coefficient between all the variables in the dataset and visualizes the correlation matrix. The result of the correlation matrix is shown in the screenshot below. 
![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/cb1b433e-700a-47ff-b20b-54088f355fef)

b.4)The correlation between the variables can affect the model accuracy. If two variables are highly correlated, they might provide redundant information, which can lead to overfitting of the model. On the other hand, if two variables are not correlated, they can provide complementary information which can help improve the accuracy of the model.
![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/6f22cf29-7374-4c23-bc69-329aec4b1d31)


## Lab Assignment 2
### Part I
The variables included in the model as predictors were Passenger ID, sex, Pclas,  Fare, Embarked, Parch, Age and SibSP.These variables were flaged with either Orange or Green colors and also marked as shown below.


### Part II
Random forest was found to be the best algorithm for the prediction. This is because it had the highest AUC of 0.903, this led to producing the best outcome.

### Part III
Sex was the most important predictor in the model. This can be determined by the weights in the correlations as shown below.

### Part IV
The file for the Random forest algorithm is exported as RandomForestPredictions.xls

