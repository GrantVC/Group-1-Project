# Group-1-Project

## Data Sources
HAM10000_metadata.csv obtained from Kaggle. The data set contains images, diagnosis, diagnosis type, age, gender, and location of lesion. There are 7,470 unique lesion IDs.

## Technologies we are using:
1.	GoogleColab with Pandas to clean the data
2.	PGAdmin 4 to store the data
3.	SciKit-Learn to train the data
4.	JavaScript and HTML5 for the dashboard hosted on a server

## Machine Learning Algorithm  


Selected Approach: **Supervised Learning Model (labeled input and output data)**

Supervised learning type of problem for data mining: **Regression (predict numerical values based on various data points)**


For our project we will be using a supervised machine learning model as  it involves a series of functions that map an input to an output based on a series of example input-output pairs. For example from our dataset we could have the patient age as the input while the location of the skin cancer on the body as the output, and thus be able to predict the location of skin cancer on the body for different group ages. For supervised learning model there are two sub categories which are regression and classification, for our project regression model is more suitable as it would allow us to find a target value based on independent predictors this would allow us to find the relationship between a dependent variable and an independent variable. It is well noted that the output will be continuous. There are multiple types of regression models for all purposes of our project we will start with linear regression and decide if it needs to be changed later on. We can preform multiple linear regressions to find a plane of best fit for the data  or polynomial regression that finds a curve for best fit. Random forests regression might also be a viable option as it is a kind of ensemble learning techniques that build off over decision trees it however involves creating multiple decision trees using bootstrap data sets of original data then the model selects the highest number of nodes of predictions, basically more  it is a “majority wins” model.


For supervised learning the model iteratively makes predictions on the data to seek the right answer, thus it “learns” from the training dataset. This leads us to the conclusion that supervised learning is more accurate than unsupervised learning models, however for supervised leaning model human intervention to label the data is required.
