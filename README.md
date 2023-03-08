# Association rules and Items Recommend
This repository is one of the Homework in the datamaster course. The work is aimed to find the Association rules of the items purchasing by using the apriori libraly to get the insight.
[Unsupervised_Learning_Association_rules_Homework_github](https://github.com/Kritkikomo/Association_rules_datamaster/blob/main/Unsupervised_Learning_Association_rules_Homework_github.ipynb)
As the result I create the list of recomendation for each customer
![image](https://user-images.githubusercontent.com/112334326/223737467-1cbf2c36-7f37-4be6-8314-5871f4bc6bc4.png)

## Step by Step Explaination
This Association rules notebook aim to find the Items rule that will use for marketing strategy. Moreover, I create the Item Recommendation that base on the purchasing data that we have. 
The Notebook consists of 4 main step which is
* Step1 Loading the dataset
* Step2 DataPreparation
* Step3 Processing the data
* Step4 Get More insight 
So let's explore
### Step1  Loading the dataset
In this step we aim to Loading the data and understand the data.
![image](https://user-images.githubusercontent.com/112334326/223732266-0c0da0d3-fb0e-4d8c-8ba5-6ea5d2236e9b.png)
### Step2 DataPreparation
#### Step2.1 Data cleansing
In this step, we focus on cleaning the data and select only the using one. In this project we will focus only in United Kingdom.
![image](https://user-images.githubusercontent.com/112334326/223732716-58db8df4-0d4f-48bd-823a-eb16e5f1284c.png)
#### Step2.2 Preparing the data
After cleanig we preparing the data in the suitable form to use further.
![image](https://user-images.githubusercontent.com/112334326/223733282-a7c2c178-6f38-40dd-9da3-2622ca651f2b.png)
### Step3 Processing the data
#### Step3.1 Extract the association rule
I use the apriori library tho extract the association rule.
![image](https://user-images.githubusercontent.com/112334326/223733669-f1971f2e-f5c1-4b39-990e-b0d5067508d8.png)
#### Step3.2 Preparing more data for analytic
I create 3 more dataframe which is stock_df, Price_Quan and Totalvalue to use for analytic in the next step
Stock_df is parse the stock code in to the Description in order to facilitate the user.
![image](https://user-images.githubusercontent.com/112334326/223734316-19b1ed9f-32ea-406d-87a7-5f787b935a97.png)
Price_Quan is the indicator for Quantity and Price of each item in order to use this indicator to weight the Association rule.
![image](https://user-images.githubusercontent.com/112334326/223734476-978a64a2-9988-4eac-ab3b-3f455f0eb323.png)
 This value will use in the macro marketing section which we will use this value to evalute the rank of the rule
![image](https://user-images.githubusercontent.com/112334326/223735419-fe5628f0-2014-466d-b5f5-c849bbeb1d66.png)
### Step4 Get more insight
In this step I de fine 2 more parameter to facilitate the analyis which is  Expected value with Support and Expected value with Confidence.
![image](https://user-images.githubusercontent.com/112334326/223735937-3de1e590-8896-4c3d-b4af-7661e0e804a5.png)
then we calculate these 2 parameter and use it for mass marketing and micromarketing
Mass marketing is aim on mass amout of people which use the Expected value with Support.
![image](https://user-images.githubusercontent.com/112334326/223736723-27c06f1e-13e4-4a84-834d-6086d3af451e.png)

Micro markeing is aim for individual one which use the Expected value with Confidence.

![image](https://user-images.githubusercontent.com/112334326/223736845-662c920d-a526-472c-a6b0-b26f440539e6.png)
##### Recomendation for each customer
In this part I create the recommendation base on the itemprice that customer likely to purchase. And this is the result item that we will recommend the customer with the estimate value that we will gain.
![image](https://user-images.githubusercontent.com/112334326/223737467-1cbf2c36-7f37-4be6-8314-5871f4bc6bc4.png)

For the detail explanation please visit the notebook via this link.[Unsupervised_Learning_Association_rules_Homework_github](https://github.com/Kritkikomo/Association_rules_datamaster/blob/main/Unsupervised_Learning_Association_rules_Homework_github.ipynb)






