# EXP-3-Implementation-of-log-transformation
## AIM:
Perform log transformation on international airline passenger data.
## ALGORITHM:

1. Import the required packages like pandas and numpy

2. Read the data using the pandas

3. Perform the data preprocessing if needed and apply log transformation.

4. Plot the data according to need, before and after log transformation.

5. Display the overall results.
## PROGRAM:
```
import numpy as np
import pandas as pd
data= pd.read_csv('AirPassengers.csv')
data.head()
data.dropna(inplace=True)
x=data['Month']
y=data['#Passengers']
data_log=np.log(data['#Passengers'])
X=data['Month']
Y=data_log
import matplotlib.pyplot as plt
plt.plot(x,y)
plt.xlabel('Original Data')
plt.plot(X,Y)
plt.xlabel('Log- Transformed data')
```
## OUTPUT:
## FIRST FIVE ROWS:
![image](https://github.com/swethamohanraj/EXP-3-Implementation-of-log-transformation/assets/94228215/717049ba-8cfe-41bd-8471-ce847016a6ed)

## BEFORE LOG TRANSFORMATION:
![image](https://github.com/swethamohanraj/EXP-3-Implementation-of-log-transformation/assets/94228215/65d249b4-fc7b-4c13-92b8-175eb2cf4f98)

## AFTER LOG TRANSFORMATION:
![image](https://github.com/swethamohanraj/EXP-3-Implementation-of-log-transformation/assets/94228215/af519eb1-a0ce-4bb7-ac9a-6a7d91ccb21e)

## RESULT:
Thus we have created the python code for the log transformation on international airline passenger
data.
