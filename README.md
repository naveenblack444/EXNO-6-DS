# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 df=pd.read_csv("titanic_dataset.csv")
 df.head()
```
<img width="1277" height="417" alt="image" src="https://github.com/user-attachments/assets/48f5883d-500f-4b66-b242-5584798c8e0d" />

```
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot')
```

<img width="1286" height="583" alt="image" src="https://github.com/user-attachments/assets/04cace7a-ebea-4ee4-94a1-6dc0fb1243df" />

```
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
```
<img width="1277" height="588" alt="image" src="https://github.com/user-attachments/assets/01860a62-6951-4e07-afa9-1f6f8473be2c" />

```
plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
```
<img width="1238" height="724" alt="image" src="https://github.com/user-attachments/assets/2630ffe0-8bc0-40e7-8bfa-4508a21da240" />

```
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()
```

<img width="1278" height="592" alt="image" src="https://github.com/user-attachments/assets/97b422ba-afeb-4c42-8e79-b931873c2833" />

```
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
```
<img width="1272" height="575" alt="image" src="https://github.com/user-attachments/assets/12d1246b-adf9-4b3f-a7bb-b99e685dce3b" />

```
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```

<img width="1275" height="583" alt="image" src="https://github.com/user-attachments/assets/4a5f2cde-d91b-4216-860d-15f07ea945e0" />

```
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
```
<img width="1280" height="729" alt="image" src="https://github.com/user-attachments/assets/e0469da3-5ff7-4c12-9fa3-704462f94700" />

```
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
```
<img width="1276" height="593" alt="image" src="https://github.com/user-attachments/assets/44997fee-b379-4cc4-88ee-190008afe2bf" />

```
 sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
```
<img width="1279" height="715" alt="image" src="https://github.com/user-attachments/assets/a574923b-97b1-450f-8e9a-a4f85edd819d" />

```
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```

<img width="1286" height="668" alt="image" src="https://github.com/user-attachments/assets/e467b6f6-b830-4767-8a3c-e6b2ab0f559f" />





# Result:
 Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
