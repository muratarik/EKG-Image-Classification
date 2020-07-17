# EKG-Image-Classification

This Kaggle project can be found on this link: https://www.kaggle.com/mmtazmuratark/ecg-images-prediction-cnn-pytorch-in-python.

## 1. Problem Statement 

We want to predict behaviour of the EKG signals. Categories are normal beat, supraventricular ectopic beat, ventricular ectopic beat, and fusion beat.
Our client is healthcare providers and hospitals. Some patients need to be kept under observation and those patients are connected to EKG machines. It is impossible to put a person 7/24 to watch them. It will be better if we can obtain and analyze EKG data simultaneously to check if everything is in normal condition.
By analyzing EKG data we can inform healthcare providers immediately so they can take immediate action. Seconds might become important to save one’s life.

## 2. Dataset

I will be using data from a Kaggle project. The source link: https://www.kaggle.com/analiviafr/ecg-images

The original data is coming from Physionet's MIT-BIH Arrhythmia Dataset. There are 109445 samples in the dataset. Image Resolution is 196x128. They classified the data in five categories. Number of pictures in each category are as follow:

N (Normal beat)			                : 90.589
S (Supraventricular ectopic beat) 	: 2.779
V (Ventricular ectopic beat)    		: 7.236
F (Fusion beat)			                : 803
Q (Unknown beat)		              	: 8.038

I will use a convolutional neural network to solve this problem.

My deliverables will be the Jupyter notebook that includes codes and some notes. I will also report my method and findings in a final report. 


## 4. Exploratory Data Analysis

This data set is very clean. I plotted 6 images from each category as an example. my plots will be found under plots folder.

## 3. Data Wrangling

This dataset has no separate train and test sets. All images are categorized under its own subfolder with the same name. These folders are in the “../input/ecg-images/MITBIH_img” folder. For model training we need to split the dataset and also if you are working on Kaggle you have to copy your files under “../working” subfolder. I chose a 0.2 split ratio. For this reason I created “../working/test” and “../working/train” subfolders on Kaggle.. These test and train folders have 5 subfolders. From each categorical subfolder(“../input/ecg-images/MITBIH_img/ ”), the first 20% of the images are copied to its related test subfolders and the rest are copied to related train subfolders.

## 4. Predictive Modeling

Predictive models are run at Kaggle servers. GPU is used because GPU is faster than CPU. Convolutional Neural Network(CNN) is used for classification. I used the PyTorch package. PyTorch package is more flexible than other packages.

THANK YOU

MURAT


