# Cardiac Rhythm Classification

**1. Dataset:** the dataset is collected using the **AliveCor device**. It contains **8,528 single lead ECG recordings** lasting from 9s to just over 60s. You can find more information and download the dataset [here](https://physionet.org/challenge/2017/)

**2. Preprocessing**
The data is **_.mat_** file. To make it more convenient, **_mat2hdf5_** is utilized to convert the whole dataset into **_.h5_** format. 

**3. Reference**
File **_REFERENCE-v3_** contains the label of this dataset

**4. Machine Learning Model**
The **_AFib_Model_F_** file includes feature extraction and XGB model. 

**_List of features:_**
+ Average power of signals (1)
+ Statistical features of RR intervals (12): MRR, SDNN, RMSSD, pNN50, CV, Delta_RRI_max, Min_RR, Median_RR, Mean_R, Std_R, NADev, NADiff
+ Statistic features of P – wave (9): mean p1-p6, P-var, P-skewness, P-kurtosis
+ Statistic features of RR’s segments (4): mean, variance, skewness, kurtosis
