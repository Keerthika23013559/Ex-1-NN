<H3>ENTER YOUR NAME:KEERTHIKA M P</H3>
<H3>ENTER YOUR REGISTER NO:212223240071</H3>
<H3>EX. NO.1</H3>
<H3>DATE:29-04-2026</H3>
<H1 ALIGN =CENTER> Introduction to Kaggle and Data preprocessing</H1>

## AIM:

To perform Data preprocessing in a data set downloaded from Kaggle

## EQUIPMENTS REQUIRED:
Hardware – PCs
Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## RELATED THEORETICAL CONCEPT:

**Kaggle :**
Kaggle, a subsidiary of Google LLC, is an online community of data scientists and machine learning practitioners. Kaggle allows users to find and publish data sets, explore and build models in a web-based data-science environment, work with other data scientists and machine learning engineers, and enter competitions to solve data science challenges.

**Data Preprocessing:**

Pre-processing refers to the transformations applied to our data before feeding it to the algorithm. Data Preprocessing is a technique that is used to convert the raw data into a clean data set. In other words, whenever the data is gathered from different sources it is collected in raw format which is not feasible for the analysis.
Data Preprocessing is the process of making data suitable for use while training a machine learning model. The dataset initially provided for training might not be in a ready-to-use state, for e.g. it might not be formatted properly, or may contain missing or null values.Solving all these problems using various methods is called Data Preprocessing, using a properly processed dataset while training will not only make life easier for you but also increase the efficiency and accuracy of your model.

**Need of Data Preprocessing :**

For achieving better results from the applied model in Machine Learning projects the format of the data has to be in a proper manner. Some specified Machine Learning model needs information in a specified format, for example, Random Forest algorithm does not support null values, therefore to execute random forest algorithm null values have to be managed from the original raw data set.
Another aspect is that the data set should be formatted in such a way that more than one Machine Learning and Deep Learning algorithm are executed in one data set, and best out of them is chosen.


## ALGORITHM:
STEP 1:Importing the libraries<BR>
STEP 2:Importing the dataset<BR>
STEP 3:Taking care of missing data<BR>
STEP 4:Encoding categorical data<BR>
STEP 5:Normalizing the data<BR>
STEP 6:Splitting the data into test and train<BR>

##  PROGRAM:
```
from google.colab import files
import pandas as pd
import io
from sklearn.preprocessing import StandardScaler
from sklearn.preprocessing import MinMaxScaler
from sklearn.model_selection import train_test_split
df.isnull().sum()
df.fillna(0)
df.duplicated()
df['EstimatedSalary'].describe()
scaler = StandardScaler()
inc_cols = ['CreditScore', 'Tenure', 'Balance', 'EstimatedSalary']
scaled_values = scaler.fit_transform(df[inc_cols])
df[inc_cols] = pd.DataFrame(scaled_values, columns = inc_cols, index = df.index)
df
x = df.iloc[:, :-1]
y = df.iloc[:, -1]
print("X Values")
x
print("Y Values")
y
x_train, x_test, y_train, y_test = train_test_split(x, y, test_size = 0.2, random_state = 42)
print("X Training data")
x_train
print("X Testing data")
x_test
print(len(x_test))
print(len(y_test))

```


## OUTPUT:
<img width="841" height="405" alt="image" src="https://github.com/user-attachments/assets/7b24ffe0-5935-4f05-b7c8-a2249918e245" />

<img width="845" height="444" alt="image" src="https://github.com/user-attachments/assets/00329507-71cd-470f-80df-ba27fb12d794" />

<img width="851" height="673" alt="image" src="https://github.com/user-attachments/assets/3aaf59c6-c3c3-43ea-a6c8-1d4e7aa2e7d2" />

<img width="836" height="656" alt="image" src="https://github.com/user-attachments/assets/8ca2c917-bab3-431e-8471-50344fa64ada" />

<img width="815" height="331" alt="image" src="https://github.com/user-attachments/assets/fc3f96e2-9a6e-4031-8326-0ed02abea694" />
<img width="815" height="331" alt="image" src="https://github.com/user-attachments/assets/0a8f1f81-7cec-496c-b285-0e551f54fd2d" />
<img width="821" height="728" alt="image" src="https://github.com/user-attachments/assets/abea72d9-86eb-46ac-b480-eeb4a2666e9b" />
<img width="431" height="86" alt="image" src="https://github.com/user-attachments/assets/16375ccd-9778-493e-bca6-112179a2d5fb" />




## RESULT:
Thus, Implementation of Data Preprocessing is done in python  using a data set downloaded from Kaggle.


