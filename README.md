# Stroke-Prediction-Using-Classification-Models
Stroke Prediction

Abstract
Machine Learning and AI  techniques are rapidly becoming veritable tools that assist businesses and healthcare industry draw actionable insights. 
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
The  report  also  illustrates  the  data 
visualization and pre-processing methods that are essential to perform before giving the data 
to  machine/deep  learning  models
These techniques have provided the platform for the quick digitalization of healthcare information management and for the developing of Electronic  Health  Records  (EHR).  Machine Learning and AI have also assisted in implementing quick and comprehensively automated procedures in disease detection among the vulnerable individuals at an early stage, so that accelerated processes of referral, counselling, and treatment can be initiated. (Penikalapati and Rao, 2020)
This  paper purposes of  identifying 
the  best  models  of  Machine  Learning  duly  supported  by  their 
performance indices, utility aspects, constraints, and critical issues in 
the  specific  context  of  their  effective  application  in  healthcare 
analytics for the benefit of practitioners and researchers
The purpose of this project is to identify the best Machine Learning model based on its performance indices, constraints, and critical issues in the specific context of their effective application on the chosen dataset.
developing  Electronic  Health  Records  (EHR)  for 
implementing quick and comprehensively automated procedures in 
disease detection among the at-risk individuals at an early stage, so 
that accelerated processes of referral, counseling, and treatment can 
be initiated
developing  Electronic  Health  Records  (EHR)  for 
implementing quick and comprehensively automated procedures in 
disease detection among the at-risk individuals at an early stage, so 
that accelerated processes of referral, counseling, and treatment can 
be initiated
This project considered a real-world dataset in healthcare where patterns are found in the dataset by using common data-mining tools and machine learning algorithms to predict cases of stroke occurrence in patients. Below is my report generated after performing the required tasks on an approved dataset.
Introduction
My dataset is on the prediction of stroke which according to the World Stroke Organisation, has already reached epidemic proportions. Globally 25% adults over the age of 25 are likely to have stroke in their lifetime. It is also estimated that 12.2 million people worldwide will have their first stroke episode this year and an average of 6.5 million people will die as a result of complications from stroke. As much as 110 million people in the world have experienced stroke (Bonita et al., 2004).

The dataset contains attributes that are considered as indicators in the detection of stroke in individuals. I have visualized the dataset graphically with comparison to the categorical and numerical features. The distribution of dataset along with the distribution of target class(stroke) is also visualized

I have considered the dataset as a classification model using, Linear Regression, K-Nearest Neighbour, Support Vector Machine and Random Forest Classifier as the classification  algorithms. The feature extraction plays a vital role in the classification models.
The main objective of this project is to achieve maximum accuracy of stroke prediction.
Data Exploration
The data exploration process was done using python-pandas libraries. The data set contains 12 attributes and 5110 features 
Attributes
1.	id: unique identifier of each patient. This has no impact on the performance of our model and was dropped
2.	Gender: "Male", "Female" or "Other"
3.	Age: age of the patient
4.	Hypertension: 0 if the patient is not hypertensive, 1 if the patient has hypertension
5.	Heart disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6.	Ever_married: "No" or "Yes"
7.	Work_type: "children", "Govt_job", "Never_worked", "Private" or "Self-employed
8.	Residence_type: "Rural" or "Urban"
9.	Avg_glucose_level: average glucose level in blood
10.	Bmi: body mass index of the patient. 
11.	Smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
12.	Stroke: This is the target class with 1 if the patient had a stroke or 0 if not
During the data cleaning phase it was discovered that 201 patient’s bmi records are with null values. I considered filling the null values with  the average bmi  since the modal class of the patients fall within this class range.
One patients’ gender information was recorded as “others”, this was dropped as it is negligible and will not  have any meaningful impact on the outcome of the result.
After cleaning  and  visualizations, I checked the strength of correlation between the attributes. (Mckinney, 2018). I also considered the Variance Inflation factor(VIF)  to Check for multicollinearity features by displaying the variance inflation factor (VIF). This assisted me narrow  this to a classification problem rather than regression. (Swamynathan, 2017)

Data Pre-processing/Data Scaling
Before splitting my dataset, it was observed that the dataset was not balanced. The dataset was skewed towards the majority class of 95.1% who were without stroke and minority class of 4.9% who were with stroke.
To avoid imbalanced dataset modelling, I used the RandomOverSampler package in Scikit learn to resample my dataset. The training dataset was set 20% and random_state at 42

Data Modelling
I used the Linear Regression, K-nearest Neighbour, Support Vector Machine and Random forest classification algorithms to achieve the below accuracy predictions.
•	Accuracy score Linear Regression:		  0.75
•	Accuracy score K-Nearest Neighbours:	  0.86
•	Accuracy score Support Vector Machine:	  0.77
•	Accuracy score Random Forest Classifier:	  0.91

From all the classification algorithms used, Random Forest Classifier performed best with accuracy score of 94% . In order to improve on this result I used the Random Forest Hyperparameter Tuning and the accuracy was improved to 92%. 

Evaluation report
To further evaluate my report the ROC curve of the Random Forest result was displayed.
A review of the confusion matrix shows the following result
TN:	933 Numbers of negative cases classified as negative
FN:	27 Numbers wrongly classified as Negative
FP:	57 Numbers wrongly classified as positive	
TP:	5 Numbers of positive cases, classified as positive


Conclusion
At the end of the data modelling, the Random Forest Classifier performed best with 92% accuracy and therefore was adopted as my best prediction model.
