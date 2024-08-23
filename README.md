# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

# AIM:
To Develop a python program to Plot a time series data (Settle weather).
# ALGORITHM:

# PROGRAM:
'''
import pandas as pd
import matplotlib.pyplot as plt
file_path = '/content/seattle_weather_1948-2017.csv'
df = pd.read_csv(file_path)
df['DATE'] = pd.to_datetime(df['DATE'])
df.set_index('DATE', inplace=True)

plt.figure(figsize=(14, 7))
plt.plot(df.index, df['PRCP'], label='Precipitation')
plt.plot(df.index, df['TMAX'], label='Max Temperature')
plt.plot(df.index, df['TMIN'], label='Min Temperature')
plt.xlabel('Date')
plt.ylabel('Value')
plt.title('Weather Data Over Time')
plt.legend()
plt.grid(True)
plt.show()
'''










# OUTPUT:






# RESULT:
Thus we have created the python code for plotting the time series of given data.
