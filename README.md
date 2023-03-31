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

