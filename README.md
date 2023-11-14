# Ex-03 Univariate Analysis

## AIM
To read the given data and perform the univariate analysis with different types of plots.

## ALGORITHM

1)Read the given data.
<br>
2)Perform data cleaning process.
<br>
3)Visulaize and analyse the data using various plots.
<br>

## CODE AND OUTPUT
```
DEVELOPED BY: Ragavendran A
REG NO:212222230114
```
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
df=pd.read_csv("/content/iris (1).csv")
df.head()
df.tail()

df.nunique()
df.iloc[:,4].value_counts()
for i in range(0,df.shape[1]):
  print("-----------",df.columns[i],"------------")
  print(df.iloc[:,i].value_counts())
  print("---------------------------------------")
sns.countplot(x='species',data=df)

dfv=df.loc[df['species']=='virginica']
plt.plot(dfv['sepal_length'],np.zeros_like(dfv['sepal_length']),'*')
plt.xlabel('sepal length')
plt.show()
dfs=df.loc[df['species']=='setosa']
dfc=df.loc[df['species']=='versicolor']
plt.plot(dfs['sepal_length'],np.zeros_like(dfs['sepal_length']),'*')
plt.plot(dfc['sepal_length'],np.zeros_like(dfc['sepal_length']),'X')
plt.plot(dfv['sepal_length'],np.zeros_like(dfv['sepal_length']),'o')
plt.plot(dfs['sepal_length'],np.zeros_like(dfs['sepal_length']),'+')
plt.plot(dfc['sepal_length'],np.zeros_like(dfc['sepal_length']),'-')
plt.xlabel('SEPALLENGTH')
plt.show()
```
![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/509c072c-5f8c-4b92-830c-8ffd2c66a3b8)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/89354407-fc9a-417d-b892-2da3d258ae16)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/ece8baf1-7ead-4b93-8450-c3904ee35b92)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/cb7a101a-00d2-4261-ba48-dee5609c21c0)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/7f9c02ad-53fe-4d73-bbe0-ee5917f53c2d)


![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/915db0bc-0c15-4c4c-830e-964433da25a2)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/648de42c-250c-4e9c-b833-34362ce1c283)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/9b7a6e86-1454-46e7-b02c-2952a2f5d6e7)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/0ee00895-4b66-484b-84b0-f8ac3ae06041)


![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/e4551a44-022b-4bca-bcf4-70c47bcf3ced)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/a128e4c9-ff70-427e-ae13-3efbf1ebf2b9)

![image](https://github.com/gururamu08/ODD2023-DataScience-Ex-03/assets/118707009/2daf09ff-dbb1-43c6-b6a4-f993be17bd16)

## RESULT
Thus the univariate analysis can be implemented successfully.
