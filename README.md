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

# OUTPUT
![Screenshot (218)](https://user-images.githubusercontent.com/119657657/226257595-94a889fd-8fa1-4621-933f-d788b5af9ede.png)

![Screenshot (219)](https://user-images.githubusercontent.com/119657657/226258739-2e32b25a-4a62-4ce9-9b52-c112a91133ee.png)

![Screenshot (220)](https://user-images.githubusercontent.com/119657657/226258808-456f6482-0e9b-474d-834a-2e23e3225d7e.png)

![Screenshot (221)](https://user-images.githubusercontent.com/119657657/226258871-4ddbf4b4-0ca7-44d1-9100-c616750f7701.png)

![Screenshot (222)](https://user-images.githubusercontent.com/119657657/226258928-5d676416-a089-4a1f-9f72-a3f96bd8edee.png)

![Screenshot (223)](https://user-images.githubusercontent.com/119657657/226259015-172b7c6e-fb27-403b-a628-d413d107d06b.png)

![Screenshot (224)](https://user-images.githubusercontent.com/119657657/226259084-4d1067e0-2ff9-4f4a-a57d-429b8c4da4e6.png)

![Screenshot 2023-03-20 111416](https://user-images.githubusercontent.com/119657657/226259161-fd7d058b-a86d-45a2-a47d-fab2e8af8074.png)

![Screenshot (225)](https://user-images.githubusercontent.com/119657657/226259202-e01eddc8-9f87-40b9-b1b1-26440eaf9254.png)

#RESULT

The given Data is read and performed with data cleaning process and the cleaned file is saved.








