# RAPIDMINER STUDIO
## What is RapidMiner studio??
RapidMiner is a Data Analytics and Data Science tool which provides the user all the
interactions with the data from preprocessing stage to model evaluation stage without
any use of programming language.
This RapidMiner is intended to support all the functionalities across the AI ecosystem.

## Introduction On RapidMiner Studio:
The main motto of the RapidMiner tool is to collaborate and provide an interface
to perform all the data science work. From providing multiple datasets, Machine
Learning Algorithm, Visualizations and Model Deployment.
Below are the major establishments of this RapidMiner —
● This platform provides its user with different types of datasets where one can
directly use them to build the models. However, rapidminer also supports loading
data from different sources like Cloud, Relational Databases, NoSQL, Excel and
CSV files.
● The process of working with datasets is completely in drag and drop format. All
the preprocessing, model building and visualization can be done without any
code.
● We need not build any supervised or unsupervised machine learning algorithm
from scratch. RapidMiner tool also provides us all the required algorithms to
perform Regression, Classification and Clustering.
● We can train the data to provide optimal solutions. This also supports
hyperparameter tuning to build an efficient algorithm.
● RapidMiner also supports deploying our model into different platforms with the
help of certain interfaces.
● Once the model is deployed, with the help of interfaces we can collect and store
the real time data.



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
#### The Dataset
![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/e6ba8acd-ffd2-4ef9-9c3f-81bd9ab6a7a5)

The variables included in the model as predictors were Passenger ID, sex, Pclas,  Fare, Embarked, Parch, Age and SibSP.These variables were flaged with either Orange or Green colors and also marked as shown below.


### The RapidMiner studio
![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/7fd29833-d5b4-4527-adb6-6702af124499)

![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/8a7251b9-cb45-4525-a7c5-36dee9eab624)



### Part II
Random forest was found to be the best algorithm for the prediction. This is because it had the highest AUC of 0.903, this led to producing the best outcome.

![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/fe495744-bc8e-4c0f-934b-151f4d574838)



### Part III
Sex was the most important predictor in the model. This can be determined by the weights in the correlations as shown below.
![image](https://github.com/VincentOracle/RapidMiner-Studio-RandomForest/assets/104081669/9b0c14d2-4a14-4f7b-af7e-c4be2a36fae6)

### Part IV
The file for the Random forest algorithm is exported as RandomForestPredictions.xls

