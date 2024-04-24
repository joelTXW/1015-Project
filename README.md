# SC1015 Data Science Project

Our team seeks to use hotel booking data extracted from the Hotels Reservation Dataset by Ahsan Raza on Kaggle, to determine which aspects of a booking can be accurate predictors  of whether that booking is cancelled.

## Important files:
Please read the jupyter notebook in the following order: Data Cleaning.ipynb, EDA.ipynb, Machine Learning.ipynb

### Datasets used
Contains .csv files of initially downloaded dataset (Hotel Reservations.csv), as well as the dataset after cleaning (Cleaned.csv).

### Data Cleaning Notebook (Data Cleaning.ipynb)
Our group performs data cleaning on the downloaded dataset. This includes
- Removing invalid data (invalid dates, 0 number of people booking, number of weekdays and weekends are 0 combined)
- Combining arrival year, month and date into a single variable “arrival datetime”
- Encoding variables (e.g. room type) into machine readable categorical values\
We proceed to output this to a new .csv file for analysis.

### EDA Notebook (EDA.ipynb)
Using the cleaned data, we perform univariate analysis of the 15 variables determined to have possible relevance to a booking’s status. Our group makes suggestions for the data distribution of each variable. 

In addition, we perform bivariate analysis of
- number of previous cancellations
- lead time\
With the variable of interest, “booking status”.

For all analysis of variables, data visualisation in the form of catplots, boxplots, histplots, violinplots, and/or heatmaps accompanies the analysis.

### Machine Learning Notebook (3 different algorithms) (Machine Learning.ipynb)
- Decision Tree Classifier
- Random Forest Classifer
- Implementation of GridSearchCV for Random Forest Classifier
- To tune the best hyperparameters for random forest
- Logistic Regression


## Conclusions
- Lead time is the best predictor of the outcome of whether a booking is cancelled
- Top predictors are able to achieve a high percentage of using all variables as predictors, in a bigger dataset where there is time and space constraints using top predictors only can help reduce time and space requirements
= Using Random Forest Classifier, we are able to use all the variables except date to accurately predict (88%) whether a booking is going to get cancelled or not

## Learnings:
- Cleaning invalid values of dataset and potentially
- Different encoders and their use cases
- One Hot Encoding
- Label Encoding
- How to analyse variables, both individually and in relation to the variable of interest, booking status
- New machine learning techniques
- Logistic Regression
- Random Forest Classifier
- GridSearchCV
- Advantages/Disadvantages of each learning model

References:
https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset
https://hospitalitytech.com/global-cancellation-rate-hotel-reservations-reaches-40-average

Contributors:
Joel Tan Xin Wei - Data Cleaning, Machine Learning
Philip Han - Exploratory Data Analysis, Data Visualisation

