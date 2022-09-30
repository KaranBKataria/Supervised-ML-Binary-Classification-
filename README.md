# Supervised-ML-Binary-Classification-

Deploying Logistic Regression to train a supervised learning binary classifier model to determine where a given patient has Breast Cancer or not. 

Step-by-step Process Overview:

1) Once the relevant libraries were imported, I performed basic EDA on the dataset to test the cleaniness of it - looked out for missing values, duplicated data, incorrect data types

2) The next step was to perform more advanced EDA and Data Visualisation to test the relationships between a given patients' tumour being malignant (cancerous) or benign(non-cancerous) and the other features.

   This was intially carried out by producing boxplots to see the basic relationships and identifying which features had an association with a tumour being maligant or    benign. These columns included radius_mean, perimeter_mean and more. 

   Once some insight was formed into the associations, I produced histograms to reinforce these possible associations to confirm whether there was some existing          relationships. 

3) It was now time to move onto the Feature Engineering/Transformation phase. First transformation I made was to use NumPy to transform the diagnosis (label) column to    be converted into numerical categorical data (1 for malignant and 0 for benign) 

4) Once the relevant features were identified, they were noted and labelled as a variable called 'features'. The next step was to perform Feature Engineering/Transformation, namely standardization, to allow the features to be in the correct format for Logistic Regression. 

   This was performed using Scikit-Learn and the StandardScaler function. 

5) The next step was to import train_test_split function from Scikit-Learn to split the dataset into training data and test data. The size of the test data was 25% of    the original dataframe. 

6) Now for the modelling. 

   I imported the LogisticRegression function from Scikit-Learn to now deploy logistic regression on the training data (both the predictors and the label).
   
7) Now it came time to assess the model performance. To do this, I used the accuracy and precision metrics as well as the confusion matrix (using scikit-learn) and discovered the model was 96% accurate and precise. 

   Moreover, I printed to the terminal the coefficients of the deployed model to discover which features had the most impact of a given patient having breast cancer      given a one-unit increase in their value. The features with the heaviest weighting included area_se, radius_worst, perimeter_worst, area_worst, concavity_worst and    concave points_worst.


Improvements:

In order to improve the accuracy, I am going to deploy other classification algortithms such as Binary Decision Trees and plot a ROC curve to determine the optimal algorithm and classification threshold to maximise model performance.

I will also perform k-fold cross validation to determine which algorithm is optimal in classifying whether cancer is present or not for a given patient. 
