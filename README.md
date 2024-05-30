# TASK-3
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt 
import seaborn as sns
from datetime import datetime

data = pd.read_csv('C:\\Users\\rgukt\\Desktop\\householdtask3.csv')
display(data.head(10))

#scatter plot with year against own
plt.scatter(data['year'], data['own'])
plt.title("scatter plot")
plt.xlabel('year')
plt.ylabel('own')
plt.show()

#line chart with year against own
plt.plot(data['year'])
plt.plot(data['own'])
plt.title("line chart")
plt.xlabel("year")
plt.ylabel("own")
plt.show() 

#Bar chart
plt.bar(data['year'], data['own'])
plt.title('Bar chart")
plt.xlabel("year")
plt.ylabel("own")
plt.show()

#histogram
plt.hist(data['income'])
plt.title("Histogram")
plt.show()

