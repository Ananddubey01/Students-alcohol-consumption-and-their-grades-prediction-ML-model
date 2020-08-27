Using Machine learning models to relation between Student's alcohol consumption and their grades.

Link to the competition: https://www.kaggle.com/uciml/student-alcohol-consumption Link to my solution on Kaggle: https://www.kaggle.com/grandmaster619/alcohol-consumption-grade-pred-beginners-notebook

Student's alcohol consumption is a serious problem accross the globe. In that situation Kaggle came up with the dataset of predicting the cases.

About the dataset:

It contains 2 file - train.csv and test.csv These files holds data for 173 countries and daywise confirmed cases and fatalties of total 70 days. Also, these details are specified province region wise.

Now, firstly I started with feature engineering.

    There were no null values for Province_Region hence no need for data cleaning.

    Some Date feature are of type Object. So, conversion to integet type is done by mapping an object type value with a unique integer using sklearn feature called preprocessing.

    Now, I had to replace all the object type data into numericals. Followed by this, I dropped the columns that are ob type object so that the dataframes now have only numerical type features.

Training models on dataframes and generating root mean squared lograthmic error:

After splitting the data into train and test, I have used the following models:

1.Logistic Regression

2.Decision Tree Regressor

Out of all I got the best score with Decision Tree Regressor.
Thanks for reading :-)
