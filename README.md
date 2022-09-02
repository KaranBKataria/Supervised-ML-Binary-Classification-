# Supervised-ML-Binary-Classification-

Deploying Logistic Regression to train a supervised learning binary classifier model to determine where a given patient has Breast Cancer or not. 

Step-by-step Process Overview:

1) Once the relevant libraries were imported, I performed basic EDA on the dataset to test the cleaniness of it - looked out for missing values, duplicated data, incorrect data types

2) The next step was to perform more advanced EDA and Data Visualisation to test the relationships between a given patients' tumour being malignant (cancerous) or benign(non-cancerous) and the other features.

This was intially carried out by producing boxplots to see the basic relationships and identifying which features had an association with a tumour being maligant or benign. These columns included radius_mean, perimeter_mean and more. 

Once some insight was formed into the associations, I produced histograms to reinforce these possible associations to confirm whether there was some existing relationships. 

3) It was now time to move onto the Feature Engineering/Transformation phase. First transformation I made was to use NumPy to transform the diagnosis (label) column to be converted into numerical categorical data (1 for malignant and 0 for benign) 

4) Once the relevant features were identified, they were noted and labelled as a variable called 'features'. The next step was to perform Feature Engineering/Transformation, namely standardization, to allow the features to be in the correct format for Logistic Regression. 

This was performed using Scikit-Learn and the StandardScaler function. 

5) The next step was to use the Scikit-l
