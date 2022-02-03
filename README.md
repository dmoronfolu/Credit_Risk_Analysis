# Credit_Risk_Analysis
Overview

Credit risk is an inherently unbalanced classification problem as good loans easily outnumber risky loans. Due to this risk, we are to employ the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. 

In this analysis, we will perform the following to evaluate our models:

	Oversample the data using RandomOverSampler and SMOTE algorithms

	Undersample the data using the ClusterCentroids algorithm

	Use a combinational approach of over and undersampling using the SMOTEENN algorithm

	Compare BalancedRandomForestClassifier and EasyEnsembleClassifier (machine learning models used to reduce risk. We will compare the two models’ ability to predict credit risk)

Results

	Naïve Random Oversampling: The balanced accuracy score is 65%. The high-risk precision has a low positivity at 1% and the recall is at 61%, with F1 score of 2%.
 
<img width="796" alt="Naive Random Oversampling" src="https://user-images.githubusercontent.com/85265504/152279480-d726a1f8-5b48-41c5-8674-f1cac1dd1b0c.png">

	SMOTE Oversampling: The accuracy score for the SMOTE algorithm was 62%, with a high-risk precision of very low positivity at 1%, average recall is at 64%. 

<img width="800" alt="SMOTE Oversampling" src="https://user-images.githubusercontent.com/85265504/152279493-6a456fb0-ba86-4c2b-afd9-0a62ee896b8d.png">
 
	Cluster Centroids Resampling: The balanced accuracy score is at 51%, high risk precision of 1%, overall recall score of 43%

<img width="809" alt="Cluster Centroids Resampler" src="https://user-images.githubusercontent.com/85265504/152279519-0b8f919d-1871-42f8-bbb5-588dcdf1202f.png">

	SMOTEENN Combination Sampling: The balanced accuracy score is at 62%,  high risk precision of 1% and overall recall score of 54%

<img width="809" alt="SMOTEENN" src="https://user-images.githubusercontent.com/85265504/152279648-c3c8371c-35a0-476e-a5f1-d3ba8dd8f1e4.png">

	Balanced Random Forest Classifier: The balanced accuracy score for this algorithm is at 79%, high risk precision is at 4% and average recall is at 91%

<img width="800" alt="Balanced Random Forest Classifier" src="https://user-images.githubusercontent.com/85265504/152279697-e38c249f-3742-4d63-bab3-a370e74b9402.png">

	Easy Ensemble Classifier: The balanced accuracy is at 93%, high risk prediction is 7%, with high risk recall at 91% and F1 score of 14%

<img width="800" alt="Easy Ensemble AdaBoost Classifier" src="https://user-images.githubusercontent.com/85265504/152279722-990a5087-0316-46c7-bb0a-5cec232095ea.png">

Summary

In the first deliverable, we calculated the accuracy score, a confusion matrix was generated, and an imbalanced classification report was generated for the three algorithms used.

In the second deliverable, we used the SMOTEENN algorithm to resample the data from the first deliverable and predict Credit risk. And in the third deliverable, we used the BalancedRandomForestClassifier and EasyEnsemble Classifier to resample the data and predict Credit Risk. For each algorithm used, we calculated the accuracy score, confusion matric and imbalanced generated the imbalanced classification report. 

Of all the algorithms used to predict the credit risk for this analysis, the Easy Ensemble AdaBoost Classifier had the highest balanced accuracy score of 93%, low positivity high risk score of 7%, and a recall score of 91%. Therefore, I would recommend the Easy Ensemble Classifier algorithm due to its accuracy score and its ability to detect high risk credit. 
