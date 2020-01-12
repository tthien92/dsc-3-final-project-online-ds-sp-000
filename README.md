
# Classifying Hand Gestures of Myoelectric Armband


## Introduction

Prosthetic limbs have helped numerous people resume their normal lives even after an accident. Prosthetics, such as an arm, can usually be controlled by cables linking elsewhere in the body (e.g. one arm can be used to control the other). However, this can be cumbersome and redundant. However, myoelectric prosthetics are more advanced because they can read the electric signals of existing, contracting muscles, which can then be used to control the prosthetic. 

Because individual users may have varying electric signals, it is crucial to collect user-specific data and create an effective model that can correctly interpret the intentions of the user. The following dataset on kaggle has been collected by Kirill Yashuk and shows readings from 8 sensors from a Myo armband designed to pick up electrical signals of muscle contractions. Each reading corresponds to one of four different hand postures:

0 - rock

1 - paper

2 - scissors

3 - 'ok'

This investigation will utilize a variety of supervised learning models to correctly classify each reading. A conclusion will be presented at the end to summarize results.


## Table of Contents

- 0.csv - Readings for *rock* hand gesture

- 1.csv - Readings for *paper* hand gesture

- 2.csv - Readings for *scissors* hand gesture

- 3.csv - Readings for *ok* hand gesture

- student.ipynb - Python notebook for project

## Project Steps

1. Combination of csv files

2. Scaling with StandardScaler

3. PCA Analysis to reduce components from 64 to 44 features

4. Models built with five different machine learning algorithms

## Project Results

1. Five models with default parameters created with Pipeline and evaluated on accuracy
    1. Naive_Bayes pipeline test accuracy: 55.50%
    2. Tree pipeline test accuracy: 52.25%
    3. Random_Forest pipeline test accuracy: 66.17%
    4. SVM pipeline test accuracy: 89.46%
    5. XGBoost pipeline test accuracy: 68.48%
    
2. Random Forest, SVM, and XGBoost in conjunction with Bayes Optimization and Grid Search for hyperparameter optimization
    1. Random Forest
        1. Grid Search Accuracy - 62.96%
        2. Bayes Accuracy - 68.82%
    2. XGBoost
        1. Grid Search Accuracy - 85.18%
        2. Bayes Accuracy - 85.26%
    3. SVM 
        1. Grid Search Accuracy - 86.00%
        2. Bayes Accuracy (rbf) - 89.40%
        3. Bayes Accuracy (polynomial) - 88.94%
        


