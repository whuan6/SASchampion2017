# SASchampion2017

## Description
Based on the data of an airline company, a model was constructed to carry out loss warning, including loss probability model and customer portrait.

## Mining 
![Mining Process](https://github.com/whuan6/SASchampion2017/blob/master/miningProcess.png)

Taking 58,954 pieces of aviation customer data after data preprocessing **(DataPreprocessing)** as an example, customer loss prediction and value segmentation are respectively carried out through classification and clustering techniques in data mining.

Firstly, customer loss prediction **(ClassPrediction)** was carried out. Decision trees, random forests and gradient lifting trees were successively used for training and evaluation and comparison of classification performance indicators. In the mining process, a long time was spent on parameter adjustment. The results show that the classifier based on Boosting algorithm (GBDT) has better performance and lower error rate. In terms of the use of variables, the three variables -- the time from the last flight to the end of the observation window, the total ticket price in the second year and the maximum flight interval -- made a greater contribution to the prediction of customer loss.

Then k-medoids clustering **(Cluster)** was carried out for the non-loss and loss customer groups based on the mixed data **(ClusterPreprocessing)** type. The results showed that the non-loss group was divided into three categories: new customers with development prospects, old customers with loss warning and important old customers with high value level. The lost group can be divided into two categories: the lost customers with high value and the lost customers with low value, which can be classified and segmented according to the outstanding characteristics of customers.

## Result
The HTML version of this project running result can be accessed through the following link:

<https://whuan6.github.io/SASchampion2017/DataPreprocessing.html>

<https://whuan6.github.io/SASchampion2017/ClassPrediction.html>

<https://whuan6.github.io/SASchampion2017/ClusterPreprocessing.html>

<https://whuan6.github.io/SASchampion2017/Cluster.html>

ps: 
All data files are in data folder and the running image results are in the figure folder.
