# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
``` 
import pandas as pd
df = pd.read_csv("Loan_data.csv")
print(df)

df.head(5)

df.describe()

df.info()

df.tail()

df.shape

df.columns

df.isnull().sum()

df=df[~df.duplicated()]
print(df)

df.dropna()
df.dropna(axis=1)

df.fillna()

```

# OUTPUT:
![Screenshot (218)](https://user-images.githubusercontent.com/119657657/226257595-94a889fd-8fa1-4621-933f-d788b5af9ede.png)

