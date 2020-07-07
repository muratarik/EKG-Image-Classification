# EKG-Image-Classification

## 1. Problem Statement 

We want to predict behaviour of the EKG signals. Categories are normal beat, supraventricular ectopic beat, ventricular ectopic beat, and fusion beat.
Our client is healthcare providers and hospitals. Some patients need to be kept under observation and those patients are connected to EKG machines. It is impossible to put a person 7/24 to watch them. It will be better if we can obtain and analyze EKG data simultaneously to check if everything is in normal condition.
By analyzing EKG data we can inform healthcare providers immediately so they can take immediate action. Seconds might become important to save one’s life.

## 2. Dataset

I will be using data from a Kaggle project. The source link: https://www.kaggle.com/analiviafr/ecg-images

The original data is coming from Physionet's MIT-BIH Arrhythmia Dataset. There are 109445 samples in the dataset. Image Resolution is 196x128. They classified the data in five categories. Number of pictures in each category are as follow:

N (Normal beat)			: 90.589
S (Supraventricular ectopic beat) 	: 2.779
V (Ventricular ectopic beat) 		: 7.236
F (Fusion beat)			: 803
Q (Unknown beat)			: 8.038

I will use a convolutional neural network to solve this problem.
My deliverables will be the Jupyter notebook that includes codes and some notes. I will also report my method and findings in a final report. 

## 3. Data Wranling

This dataset has no separate train and test set. I downloaded the original dataset to my computer and created my own train and test sets. I chose a 0.2 split ratio. To make consistency I separated 20% of each category as a test set. This notebook is in my github. I made EDA on this notebook. 
After separation I uploaded my test and train sets as a private dataset into the kaggle.

## 4. EDA 

This data set is very clean. I plotted a few examples below. 
