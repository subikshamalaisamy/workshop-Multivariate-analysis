# workshop-Multivariate-analysis

# Types of Bivariate Analysis:

import pandas as pd

data=pd.read_excel('/content/FlightInformation (1).xlsx')

data.head()

data.dtypes

data.info()

# (i) Numerical & Numerical 

import seaborn as sns

sns.scatterplot(y=data['Price'],x=data['Total_Stops'],data=data)

# (ii) Numerical & Categorical (20 marks)

sns.barplot(y=data['Price'],x=data['Source'],data=data)

# Multivariate Analysis (40 marks)

data.corr()

sns.heatmap(data.corr(),annot=True)

# Output:

![Screenshot (20)](https://user-images.githubusercontent.com/87276633/229766056-1cf13a99-95d3-489d-acbe-32fd9371ec50.png)
![Screenshot (21)](https://user-images.githubusercontent.com/87276633/229766112-fb572269-a078-4603-bc68-ea40904df188.png)
![Screenshot (22)](https://user-images.githubusercontent.com/87276633/229766146-be92b102-05ee-4a6d-8ad3-3c3dfd087796.png)
![Screenshot (23)](https://user-images.githubusercontent.com/87276633/229766169-0574fd63-da4b-42d5-bfed-a7aa4e0ccc55.png)
![Screenshot (24)](https://user-images.githubusercontent.com/87276633/229766203-9fe1b938-b8cb-413f-9262-d3c1868214ad.png)


