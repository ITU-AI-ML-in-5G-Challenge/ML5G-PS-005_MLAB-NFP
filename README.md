# ML5G-PS-005_MLAB-NFP
Presentation Title: Regression-based Practical Network Failure Prediction on 5G Core Network Using AutoML

Team: MLAB-NFP

Team members: Jiwon Lee, Bojian Du, Kentaro Matsuura, Ryoma Kondo of The University of Tokyo, Japan

# Network Failure Prediction main links
Details about the challenge are available at https://challenge.aiforgood.itu.int/match/matchitem/64

Datasets are available after registration

# Descriptions
writen by Google Colaboratory

# Background
Goal of this challenge is to check how early and accurately the future network failures can be predicted using 3 types of metrics
The target value for prediction is the number of registration failure at 10 minutes.


There are 2 different tasks.
In task 1, we used all 3326 metrics for predicting the number of registration failure at 10 mintues. 
In task 2, we selected a part of metrics for the same prediction.


# Data tuning
Training Data:
Use different strategies for normal and abnormal cycles. For normal cycles, downsample the whole cycle by getting few rows at a constant interval. For abnormal cycles, use the data at early stage of failure event, for early prediction. Here, use the same number of rows for both normal and abnormal cycles to avoid data imbalance. 


Output Data:
Use the number of registration failures at 10 minute of the same cycle to predict the number of registration failures at 10 minutes at any time in the cycle.


# Evaluation
For evaluation, we calculated the f1 score. 

The f1 score was calculated at the prediction time, and also at different time up to 600 seconds, in order to check rather the prediction is applied for all data. Here, it is acknowledged as highly accurate when the f1 score is over 0.9.
