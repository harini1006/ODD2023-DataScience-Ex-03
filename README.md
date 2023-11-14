# ODD2023-DataScience-Ex-03
## DATE:

### Aim:
To read the given data and perform the univariate analysis with different types of plots.

Explanation: Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm:
#### Step1:
Read the given data.

#### Step2:
Get the information about the data.

#### Step3:
Remove the null values from the data.

#### Step4:
Mention the datatypes from the data.

#### Step5:
Count the values from the data.

### Program:
```
Developed By : HARINI V
Register number: 212222230044
```

#### Superstore.csv:
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
#### Diabetes.csv:
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
#### employeesal.csv:
```
import pandas as pd
df=pd.read_csv("/content/employeesal.csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
### Output:
#### Superstore.csv:
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/d522a971-1908-4477-9d94-e19c2217aaef)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/83562c66-0326-4b8f-9c60-3361b97fe6df)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/4a31a22c-6379-4c7e-ad74-f54b24738124)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/6a578af7-19e7-4d1f-9458-79fd10b2cbb3)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/5b6cbc69-5751-4f5e-9b79-004f1b20b6c2)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/d57cf79b-38bc-444b-a1b6-be7be3ac26f2)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/34b10688-187c-4675-8bef-c1d23f422021)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/52302bcf-7e26-4827-ae82-35db0480ec97)


##### Diabetes.csv:
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/adf759ae-75e6-401d-8a6e-69fc19f42c64)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/b5d7a8c5-25bc-4815-a1b6-542ab246e2a0)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/fd9b2dae-e4a7-47ef-8bfc-8d9514058d67)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/604de982-862f-437a-a57c-337e4ce8435b)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/62ebece1-c4d7-4c8b-a959-8526284795cd)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/0a987a07-753c-46e5-b376-3bde5b9ef329)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/521be223-ec6d-4472-b04c-8f3a81933abf)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/da926a4c-167c-4a8e-aeab-3525e5ecded9)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/a6d65902-909f-4d5d-b829-b69fdcc5068e)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/678208dc-fa1e-4b75-84c1-3d49fe2f8da2)
![image](https://github.com/harini1006/ODD2023-DataScience-Ex-03/assets/113497405/d86a37ee-347d-432b-b36e-4df83914a7a0)




employeesal.csv:
image

image

image

image

image

image

image

image

image

image

image

RESULT:

Hence the univariate analysis is verified

