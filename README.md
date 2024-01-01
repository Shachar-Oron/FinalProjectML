# Machine Learning Project: Endometriosis Diagnosis Prediction
## Overview
This machine learning project is dedicated to predicting whether a patient is diagnosed with endometriosis. The initial dataset, sourced from a CSV file, contains diverse information including "age," "race," "BMI," and several other factors related to endometriosis symptoms.

## Introduction:
Endometriosis is a chronic progressive inflammatory disease that affects about 1 in 10 women in the population. In 
this disease, tissue similar to the lining of the uterus grows outside the uterus. This leads to inflammation and scar 
tissue forming in the pelvic region and (rarely) elsewhere in the body. There is no known way to prevent 
endometriosis. There is no cure, but its symptoms can be treated with medicines or, in some cases, surgery. For our 
final project in the “Machine Learning” course, we used a database that contains information on 144 female 
patients who are suspected of being diagnosed with endometriosis, of which 56 actually are. Our data contained all 
kinds of comprehensive details about the clinical characteristics of all the women, treatment background, daily life, 
and personal background. Our data is relatively limited because it takes an average of 10 years to diagnose the 
disease for each woman and today there is a lack of data concerning this disease. We chose to work with this 
database because two of the members of the group, Daniel and Shahar, are sick with the disease, and the issue is 
very close to our hearts. Our main goal in the project is to use machine learning algorithms in order to shed light on 
the disease, to understand whether there are prominent characteristics or whether the combination of them 
contributes to the condition. Because it is a “transparent” disease on which there is not enough data, we consider it 
an important task to do research on it and, among other things, we will also strive to understand what are the 
significant symptoms that help diagnose the disease.
Due to lack of space and page limitation, we will list here the main conclusions and the main graphs that helped us 
to analyze the data, while more detailed and in-depth information will be included in the pdf file.

## Data Cleaning with 'mice' Package
To enhance the quality of our dataset, we employed the 'mice' package in R for data cleaning. 'mice' specializes in handling missing data through multiple imputations, generating plausible values. This step ensures a more complete and accurate dataset, laying the foundation for robust model training.

## Exploratory Data Analysis (EDA)
Correlation Plot
An exploratory data analysis was conducted, including a correlation plot. This visual representation helps identify relationships between different parameters and guides the selection of features for exploration. The outcomes of this analysis are summarized in the 'FinalProjectML.pdf' file.

## Principal Component Analysis (PCA)
* PCA was performed to transform the dataset into a new set of uncorrelated variables, simplifying the complexity and dimensionality of the data.

## Machine Learning Algorithms
* The project employs various machine learning algorithms to predict endometriosis diagnosis. Key algorithms include:

**K-Nearest Neighbors (KNN)**
* KNN is used to classify patients based on the similarity of their features to those of their neighbors in the dataset.

**Support Vector Machine (SVM)**
* SVM is applied for classification, creating a hyperplane to separate patients into distinct diagnosis categories.

**K-Means Clustering**
* K-Means clustering is used for grouping patients with similar features, aiding in pattern recognition.

**Decision Tree**
* A decision tree model is employed to establish decision rules based on different features, aiding in diagnosis prediction.

##Project Files
**FinalProjectML.Rmd:**
* The R Markdown file containing the code for the analysis, including data cleaning, exploratory data analysis, and machine learning model implementations.

**FinalProjectML.pdf:**
* The PDF file showcasing visualizations and results obtained from exploratory data analysis, PCA, and machine learning algorithms.

##Running the Code
Ensure you have the required R packages installed:
--shel
install.packages("mice")
install.packages("class")   # for KNN
install.packages("e1071")   # for SVM
install.packages("cluster") # for K-Means
install.packages("rpart")   # for Decision Tree
Open and run the 'FinalProjectML.Rmd' file in your R environment.
--

Explore the analysis results in the generated 'FinalProjectML.pdf' file.

##Conclusion
This comprehensive project integrates data cleaning, exploratory data analysis, and multiple machine learning algorithms to predict endometriosis diagnosis. The inclusion of EDA, PCA, and various algorithms enhances our understanding of the dataset and provides insights for potential clinical applications.
