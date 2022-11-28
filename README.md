# ML5G-PS-005_MLAB-NFP
This code present our results to ML5G-PS-005: Network failure prediction on CNFs 5GC with Linux eBPF.
Details about the challenge are available at https://challenge.aiforgood.itu.int/match/matchitem/64

### Team information 
Team: MLAB-NFP<br>
Members: Jiwon Lee, Bojian Du, Kentaro Matsuura, and Ryoma Kondo (from The University of Tokyo, Japan)<br>

## Report and slides
Our report and PowerPoint file of the slides of our presentation are the same file, titled "Regression-based Practical Network Failure Prediction on 5G Core Network Using AutoML", which is available [here](https://github.com/ITU-AI-ML-in-5G-Challenge/ML5G-PS-005_MLAB-NFP/tree/main/report%20%26%20slide).

## Code
The code and description is available [here](https://github.com/ITU-AI-ML-in-5G-Challenge/ML5G-PS-005_MLAB-NFP/tree/main/report%20%26%20slide).


# Background
Goal of this challenge is to check how early and accurately the future network failures can be predicted using 3 types of metrics
The target value for prediction is the number of registration failure at 10 minutes.


There are 2 different tasks.
In task 1, we used all 3326 metrics for predicting the number of registration failure at 10 mintues. 
In task 2, we selected a part of metrics for the same prediction.


# Evaluation
For evaluation, we calculated the f1 score. 

The f1 score was calculated at the prediction time, and also at different time up to 600 seconds, in order to check rather the prediction is applied for all data. Here, it is acknowledged as highly accurate when the f1 score is over 0.9.
