# Doceree


### Explaination Video : (https://drive.google.com/drive/folders/1Kll0edcL_iRFZdGCuehTIlVcbGDpuMJH)

## Brief Description of the Problem at hand: 
### OBJECTIVE: 
#### To build a robust and explainable machine learning solution to accurately classify if a user belongs to the Healthcare Professional (HCP) category and identify their specialization(Taxonomy) from ad server logs.
### PROBLEM DESCRIPTION:
#### * The ad server logs contain valuable information such as browser details, IP addresses, geographic locations, search patterns, site URLs, and more.
#### * Ad server logs provide insights into user behavior and characteristics.
#### * We need to determine if a user belongs to the HCP category and their specialization taxonomy.
#### * The solution could be used for various applications including targeted marketing of medical products to healthcare professionals, information gathering for medical research and analysis, and many more.
#
### Solution proposed and description:

#### * We propose two different models to address the problem:

#### -> HCP Identification:
#### Utilized an Extreme Gradient Boosting approach.
#### Achieved an accuracy of 99.1%.
#### This model accurately classifies users as HCPs or non-HCPs.

#### -> Taxonomy Prediction:
#### Implemented a Random Forest model.
#### Achieved an accuracy of 91.2% .
#### This model accurately predicts the specialization taxonomy for identified HCPs.

### Approach
#### DATA PREPROCESSING:
##### Label Encoding: Converted string-type columns into numerical representations.
##### Redundant Column Removal: CHANNELTYPE column, consistently set as 'Website', was removed.
##### TAXONOMY Column Handling: Removed for HCP identification model and retained as the dependent variable for Taxonomy prediction.
##### Missing Value Treatment: Replaced missing values with 0.
##### Data Split: 80% of data for training, 20% for validation.

#### MODEL SELECTION AND RESULTS:
##### The training data was fitted into several models, and their accuracies were compared: XGBoost, ExtraTrees Classifier, Random Forest, ANN, Bagging Classifier, ADABoost, Gradient Boost, Naive Bayes, and Explainable ##### Boosting Classifier.
##### XGBoost had the highest accuracy in HCP identification among other approaches as it is robust and can perform well in the case of large and imbalanced datasets using techniques like tree pruning and regularization.
##### Random Forest had the highest accuracy in Taxonomy classification among other approaches as it can handle multiple categorical features well.





