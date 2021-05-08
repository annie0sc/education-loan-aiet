# AIET - IITH - Final Project - Classification of Imbalanced Dataset

## Introduction 

Hello! As part of our Certified Summer Program, we were tasked with a group name called 'Andrew NG' in honor of the computer scientist, and technology entrepreneur. We were free to choose our datasets and do some analysis using Machine Learning algorithms.

## Group Members

1. Annie Chandolu
2. Anusree Kanadath
3. Meenakshi Somisetty
4. Ravalika Reddy Aduri
5. Sushmitha Vulapalli

## Problem Statement

- Classifying Imbalanced Education Loan Dataset to give better prediction probability of sanctioning the loan when applying for H1-B1 Visa in the USA.
- ‘Accuracy' is not a good measure for evaluating the performance of the classifiers (Accuracy Paradox), and generalization being a big challenge for such a dataset other parameters have been considered to classify the data in a much better format.

## Datasets

We used few datasets from Kaggle, then preprocessed and split the data into training and testing sets:

1. [trainData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/trainData.csv)
1. [testData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/testData.csv)
1. [h1trainData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/h1trainData.csv)
1. [h1testData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/h1testData.csv)

## Models Used

We used *Naïve Bayes Classifier* and *K-fold Cross Validation* on the datasets which gave unsatisfactory results. Then we used *XGB Algorithm* which gave good results. We used four different parameters for better classification.

## Results

The table below is a comparison of all the AUCs calculated by changing the max_depth or the scale_pos_weight.

| Sl.No. | scale_pos_weight | max_depth | AUC |
|---|---|---|---|
| 1 | 1 | 7 | 0.602 |
| 2 | 1.18 x ratio | 7 | 0.754 |
| 3 | ratio | 7 | 0.754 |
| 4 | ratio | 5 | 0.752 |
| 5 | ratio | 20 | 0.758 |
**ratio = (no. of inputs in class 0) / (no. of inputs in class 1)**

Further analysis are recorded in our presentation.

## Links

1. Our code can be found in this python notebook: [Education Loan](https://github.com/annie0sc/education-loan-aiet/blob/main/EducationLoan_Final.ipynb)
1. The presentation can be found here for detailed analysis results: [Presentation](https://github.com/annie0sc/education-loan-aiet/blob/main/AIET_Final_Project.pptx)

Datasets:

3. [trainData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/trainData.csv)
4. [testData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/testData.csv)
5. [h1trainData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/h1trainData.csv)
6. [h1testData.csv](https://github.com/annie0sc/education-loan-aiet/blob/main/h1testData.csv)
