# Suspicious-Transaction-Prediction-and-Salesmen-Segmentation

### Problem Statement
Here is a large US electrical appliances’ retailer with many branches. Salesmen are given freedom to set the price at which they sell the products and also quantity of products based on various factors.  It means, for a single product, some salesmen may sell at a price higher/lower than others for some reasons. Similarly, constraint in terms of maximum or minimum quantity is not imposed. Thus, the average sale size and average quantity sold differ from transaction to transaction. These salespeople sell a set of products of the company and report these sales with a certain periodicity to the company. The data of transactions reported by the salespeople of the company over a short period of time is used for sales and productivity analysis. The data is of an undisclosed source and has been anonymized. Each row of data table includes information on one report by a salesman. This information includes his ID, report ID, product ID, the quantity and the total value reported by the salesman.

You are invited  to develop an error/fraud detection software. Towards building such system, you are required to develop a method to determine suspicious transactions which have high propensity to be error/fraud. The goal is to verify the veracity of these reports given past experience of the company that has detected both errors and fraud attempts in these transaction reports. The task boils down to build capability in terms of appropriate ratio analysis by studying similarities between products and salesmen to detect transactions that may indicate errors/fraud attempt by a sales person. 

You are expected to classify each report ID as Yes(suspicious) / No(not suspicious) / indeterminate(doubtful).

Towards achieving this goal and for other strategic purposes, you are also required to segment the salesmen into high risk, medium risk and low/no risk categories from the standpoint of propensity to error/fraud.

### Objectives
In this hackathon, you are expected 
  1. to do exploratory Data Analysis using visualizations
  2. to build the analytical framework to predict the propensity of suspicious transaction of each report using the transactions took place.
  3. to segment the salesmen into different risk categories from the standpoint of propensity to error/fraud which will be used for strategic purposes

### Data Information

About Data: 
Data consists of  the  transaction reports submitted by the salesmen.
Target attribute : "Suspicious"

### Data Files
"Details of the datasets:

Data consists of the transaction reports submitted by the salesmen which includes  the salesman ID, report ID, product ID, the quantity and the total value reported by the salesman.  

  1.   Datasets of transaction reports including the target attribute (Suspicious) :
         a.   Train.xlsx
         b.   Test.xlsx  ( The target attribute Suspicious is not available as it has to be predicted)

(Note:  Use Train.xlsx  for doing the cluster analysis and use Test.xlsx  for assigning the segment to the new  salesmen.)
(Note : Use train dataset for cluster analysis,  removing the target attribute Suspicious)

Hint: You may explore further to understand the domain and to do the feature engineering to handle the prediction task . You may create the aggregated/ratio features at  salesman level  and overall etc. For instance, ratio between quantity of transaction  &  mean quantity of all transactions &  ratio of total sales value of the transaction with average sales value of the transactions  from salesman level etc. 

Note: The features mentioned above are neither exhaustive nor completely useful.  You may need to think and explore to find the suitable features.

### Main Tasks

  1. Exploratory Data Analysis using visualizations in R Notebook or Jupyter notebook format . (Train.xlsx  should be used for this task)

      a)  What kind of insights did you find in the data after feature engineering?

      b)  Learning curves : what is your observation based on the learning curves? Is there any bias or variance problem in the data or none? How do you address this bias/variance issue in the data?

      c) Based on the learning curves observation, which model do you think is suitable for the data and why?  

  2. You are expected to build a framework that predicts each transaction report as Yes (suspicious) / No (not suspicious) / indeterminate (doubtful).
  For this purpose you may use traditional approaches and deep learning techniques as well to improve the accuracies on prediction.

  3. You are expected to do the salesmen segmentation on train data and assign appropriate segments to the  salesmen in test dataset.  (Note : Use train datasets for this task removing the target attribute ‘Suspicious’)

### Error Metric
Consider “recall”  for the class level “Yes” of Target attribute “Suspicious” as error metric and tune the model accordingly.


