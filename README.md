# Ex03-Univariate-Analysis
### AIM
To read the given data and perform the univariate analysis with different types of plots.

### EXPLANATION

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### ALGORITHM

#### STEP 1

Read the given data.

#### STEP 2

Get the information about the data.

#### STEP 3

Remove the null values from the data.

#### STEP 4

Mention the datatypes from the data.

#### STEP 5

Count the values from the data.

#### STEP 6

Do plots like boxplots,countplot,distribution plot,histogram plot.

### PROGRAM
```
Developed by : RAJESHKANNAN M
Registration Number : 212221230081


import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()
df['Sales'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.boxplot(x='Sales', data=df)
sns.countplot(x='Postal Code',data=df)
sns.countplot(x='Sales',data=df)
sns.distplot(df["Postal Code"])
sns.distplot(df["Sales"])
sns.histplot(x='Postal Code',data=df)
sns.histplot(x='Sales',data=df)

```

### OUTPUT

![1](https://user-images.githubusercontent.com/93901857/192136689-99626a01-a2a6-47ea-934f-4e81004b4cf4.jpg)
![2](https://user-images.githubusercontent.com/93901857/192136693-50277ced-0c09-4252-af6b-09ad86424a20.jpg)
![3](https://user-images.githubusercontent.com/93901857/192136694-c593b920-460b-4541-a2cf-6ef16c320cf8.jpg)
![4](https://user-images.githubusercontent.com/93901857/192136696-bc05d30f-a9a3-4947-899f-2c1f15a3b590.jpg)
![5](https://user-images.githubusercontent.com/93901857/192136697-6eb24c0a-1c88-4fdf-9e3a-c620d32a7ae5.jpg)
![6](https://user-images.githubusercontent.com/93901857/192136698-6d55f071-cbdc-40b1-95ad-2fae502559f0.jpg)
![7](https://user-images.githubusercontent.com/93901857/192136699-59cfc6e0-09d3-4200-b86d-a5b11381f765.jpg)
![8](https://user-images.githubusercontent.com/93901857/192136700-efdfcbe1-dc70-4a18-93eb-3e333dc0d2f6.jpg)
![9](https://user-images.githubusercontent.com/93901857/192136701-f25355d2-6c90-47fb-bd29-c86009739dc1.jpg)
![10](https://user-images.githubusercontent.com/93901857/192136703-305bdee4-39d3-4094-9d2c-265591a5bf7a.jpg)

### Result

Thus we have read the given data and performed the univariate analysis with different types of plots.