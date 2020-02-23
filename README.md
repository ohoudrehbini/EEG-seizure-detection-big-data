# EEG-seizure-detection-big-data
# Application of Machine Learning in Epileptic Seizure Detection 
Ohoud Rehbini, PhD 

## Introduction and problem statements: 
Seizures are symptoms of a brain problem. They happen because of sudden, abnormal electrical activity in the brain. 

### Problem Statement 
machine learning approach to constructing patient-specific classifiers that detect the onset of an epileptic seizure through analysis of the scalp EEG, a non-invasive measure of the brain’s electrical activity.
This problem is challenging because the brain’s electrical activity is composed of numerous classes with overlapping characteristics. The key steps involved in realizing a high performance algorithm included shaping the problem into an appropriate machine learning framework, and identifying the features critical to separating seizure from other types of brain activity.

### Data source (how many datasets you have - format - dataset description)

The data is a big data were collected from MIT (CHB-MIT) public database. 
 The big data contains 23 cases (5 males and 17 females). Each cases contains one folder that has one seizures and/or more seizures detected. Some folders were collected in 1 hr others in 4 hrs long whereas other cases were collected in 2 hrs. 256 signals per second were recorded.
There are other signals were included in the data (considered as noise) such as ECG and VNS. The recored were saved in Europe data format (edf). The edf file contained 664 records and 182 signals were recorded as seizures in the total 23 cases.
However, in case of this study one cases (chb03) that has high recorded seizure activities and it was used to perform the algorithm to detect seizures and provide solution and future work for next step.

## Sample Information 
sample informaiton:
chb03-01 
- File Name: chb03_01.edf
- File Start Time: 13:23:36
- File End Time: 14:23:36
- Number of Seizures in File: 1
- Seizure Start Time: 362 seconds
- Seizure End Time: 414 seconds

## Solution structure (models type - features used - models scores- EDA )
Big Data ( > 2,000,000 from 23 cases ) two ways can be followed : 
1. pdf file converted to csv file using python 2.7 environment then the csv data can be used later in 3.7 python environment for modeling , feature engineering and visualization. ( the recommended one) 
2. pdf file can be read directly in python 3.7 environment using MNE library then we used model called ICA and brain decode library.

## file loaded: 
1. chb03.html and .ipynb are the selected data saved as CSV file . CSV file was too big to load on the GITHUB and i mentioned the resource of the data. 
2. edfcsv-2.py , .ipynb, html are the code for converting the edf file to cvs file for all the data we have on MIT. 
3. capstone-python2-enviro-final project-ohoud rehbini.html and .ipynb this file convert the edf file to csv. 
4. capstone-sezures-data-part3.html python 3.8 has all the data preprocessing , cleaning and modeling. 
5. README project explanantion. 


## modeling: 
we used : 
Logistic Regression …… 60.85%
Random Forest Classifier ….. 1.0%
SVC ……. 99.3%
Linear SVC ……. 53.4%
K neighbor Classifier …… 98.79%
GaussianNB …… 97.95%
PCA ……. 18.0%  

## Future Work and Next Steps: 
1. use powerful PC 
2. Solve the annotation problem 
3. Use CNN 
4. Use ICA in python. 

follow the blog ( https://ohoudrehbiniphd.video.blog/2020/02/23/application-of-machine-learning-in-epileptic-seizure-detection-machine-eeg/) 


