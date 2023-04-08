# Ex03-Univariate-Analysis

# Aim  

To read the given data and perform the univariate analysis with different types of plots.  

# Explanation  

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.  

# Algorithm  

# Step 1  

Read the given data.  

# Step 2  

Get the information about the data.  

# Step 3  

Remove the null values from the data.  

# Step 4  

Mention the datatypes from the data.  

# Step 5  

Count the values from the data.  

# Step 6  

Do plots like boxplots,countplot,distribution plot,histogram plot.  

# Program

import pandas as pd  

import numpy as np  

import seaborn as sns  

df=pd.read_csv('SuperStore.csv')  

df  

df.head()  

df.info()  

df.describe()  

df.isnull().sum()  

df.dtypes  

df['Postal Code'].value_counts()  

sns.boxplot(x='Postal Code', data=df)  

sns.countplot(x='Postal Code',data=df)  

sns.distplot(df["Postal Code"])  

sns.histplot(x='Postal Code',data=df)  

# Output

![ex3 1](https://user-images.githubusercontent.com/128135244/229033359-82f4338c-95bf-4297-8e90-8c1923574b5a.png)



![ex 3 2](https://user-images.githubusercontent.com/128135244/229033387-bad77022-6d10-4662-b65b-28d4c0071abb.png)



![ex 3 3](https://user-images.githubusercontent.com/128135244/229033496-f3de587e-f04e-427b-abac-7f1048290dcb.png)



![ex 3 4](https://user-images.githubusercontent.com/128135244/229033524-9df83381-b0e3-403b-b7e7-16a9667b0880.png)



![ex 3 5](https://user-images.githubusercontent.com/128135244/229033582-b8deae65-90a1-4d74-960c-41c46a93b578.png)



![ex 3 6](https://user-images.githubusercontent.com/128135244/229033614-14c8fad8-fbb6-489d-97b4-8f1e04948103.png)



![ex 3 7](https://user-images.githubusercontent.com/128135244/229033636-d6835df8-0401-4932-8020-30a1b1c9322e.png)



![ex 3 8](https://user-images.githubusercontent.com/128135244/229033734-47fa6739-d99e-4a57-a5ec-451e9eb3a22e.png)



![ex 3 9](https://user-images.githubusercontent.com/128135244/229033762-ed81d563-d2d7-47d9-b499-0fc6e964c5dd.png)



![ex 3 10](https://user-images.githubusercontent.com/128135244/229033780-b4e773b9-e2b6-40c9-8c21-d22682d0833c.png)



![ex 3 11](https://user-images.githubusercontent.com/128135244/229033805-84f76e64-120f-4009-9946-3a3b36a45ff2.png)


## Result

Thus we have read the given data and performed the univariate analysis with different types of plots.
