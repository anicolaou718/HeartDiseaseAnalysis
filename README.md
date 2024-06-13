# HeartDiseaseAnalysis
A program that implements EDA, data augmentation and machine learning algorithms on a medical data set to identify key features that affect the 10 year survival of Heart Disease patients.

This project was done for a data mining course and was inspired by a book called "Blink". 

The book spoke about how people make inferences or decisions on "gut feelings" and these gut feelings are actually based on previous information that our conscious isn't privy to but information that has been stored by the unconscious. 

In the book, it discussed how doctor's would look at a Heart disease patient's medical report and decide whether the patient should recieve treatment to prevent heart disease. These doctor's struggled to know whether to prescribe the patient with the medication so an analysis on patients with heart disease was done to highlight salient features that impacted the patient's development of Heart disease. 

Due to the heart disease analysis, doctor's were able to predict at that time with over a 75% accuracy of which patients would benefit from a preventive treatment vs those who wouldn't.

In this project I perform data cleaning/preprocessing by removing or replacing any null/outlier values and converting any string values to numerical values.

For the visualization, I used heatmaps and histograms to see the layout of the data better. There was a slight imbalance in the data so oversampling/undersampling (Smote/NearMiss) was used. Oversampling gave better results and it's the resampling I normally prefer since it doesn't remove any data from the dataframe.

Without resampling, the ML models were bias to the majority class and had an over 70% accuracy at guessing the majority class. In this dataset, the minority class had more use in predicting than the majority due to the minority class being the values of the patients that were inflicted with the disease. 

I included code with the resampling (undersampling/oversampling) and without to just have the comparison of the values. Resampling should only be done on training data and not testing data or else bias is introduced. 

The machine learning models I used were Logistic regression, Support Vector Machines and Random Forest. 

The results were evaluated with ROC curves and classification reports. 


