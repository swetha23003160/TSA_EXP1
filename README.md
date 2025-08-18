# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 14/08/2025

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt
file_path = 'dc (2).csv'
data = pd.read_csv(file_path)
data['date'] = pd.to_datetime(data['date'])
data.set_index('date', inplace=True)
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['volume'], label='Values', color='blue')
plt.title('Values over Date')
plt.xlabel('Date')
plt.ylabel('Volume')
plt.grid(True)
plt.legend()
plt.show()
```











# OUTPUT:

<img width="1203" height="643" alt="image" src="https://github.com/user-attachments/assets/4e214185-498a-4d20-88b6-a4fab97618a0" />





# RESULT:
Thus we have created the python code for plotting the time series of given data.
