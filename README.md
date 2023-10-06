# Ex-01-Develop-a-program-to-Plot-a-time-series-data

## AIM:
To Write a Program to Plot a timeseries data market price of a commodity

## Equipments Required:
Hardware – PCs Anaconda – Python 3.7 Installation / Jupyter notebook

## Procedure:
1.import the matplotlib.pyplot and pandas

2.read the datasets using pandas

3.calculate the mean for dataset

4.Plot the data according to need and can be altered monthly, or yearly.

## Program:
```
/*
Plot a timeseries data  market price of a commodity 
Developed by: GOKUL VIJAYA RAMANUJA P
RegisterNumber:  212222240030
*/

import matplotlib.pyplot as plt
import pandas as pd
df=pd.read_csv("Dataset.csv",parse_dates=["Date"],index_col="Date")
df.head()
df["2022-01"]
df["2022-01"].Close.mean()
df["2022-04-01":"2022-07-31"]
df.Close.resample('M').mean()
mean=df.Close.resample('M').mean().plot(kind="bar")
mean=df.Close.resample('Y').mean().plot(kind="bar")
```

## Output:
### df.head()
![Screenshot 2023-10-06 154006](https://github.com/s-adhithya/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/113497423/ba1f793f-64d6-46c0-92ed-3f8c9b5557d9)

### Mean
![Screenshot 2023-10-06 154025](https://github.com/s-adhithya/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/113497423/9d4f01e2-106a-4060-9cc0-d78c2c292422)

### Monthly graph
![Screenshot 2023-10-06 154042](https://github.com/s-adhithya/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/113497423/64dd2270-7d09-46a2-92eb-de3bc855546b)

### Yearly graph
![Screenshot 2023-10-06 154054](https://github.com/s-adhithya/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/113497423/33be495d-5108-410b-89c8-7b4f86f7177c)


## Result:
Thus the program to implement to Plot a timeseries data market price of a commodity is written and verified using python programming.
