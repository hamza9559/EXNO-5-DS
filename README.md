# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

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
import matplotlib.pyplot as plt
x1= [1,2,3]
y1= [2,4,1]
plt.plot(x1,y1,label= "line1")
x2= [1,2,3]
y2= [4,1,3]
plt.plot(x2,y2,label= "line2")
plt.xlabel("x axis")
plt.ylabel("y axis")
plt.title("Two line on the same graph!")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/d81db1f6-9dcb-4612-afa1-4df23fafca13)

```
x= [1,2,3,4,5,6,7,8]
y= [5,2,4,2,1,4,5,2]
plt.plot(x,y,color= "green",linewidth= 3,linestyle= "--",marker="o",markerfacecolor='blue',markersize=12)
plt.xlim(1,8)
plt.ylim(1,8)
plt.xlabel("x axis")
plt.ylabel("y axis")
plt.title("Some cool customizations!!!!")
plt.show()
```
![image](https://github.com/user-attachments/assets/8597173a-136a-4e30-9151-061395bbf706)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
```
Text(0, 0.5, 'Yield(tons per hectare)')

![image](https://github.com/user-attachments/assets/c45dccd3-3285-4a42-925f-35dcb9bd9e40)

```
x_values= [0,1,2,3,4,5]
y_values= [0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color='blue')
plt.show()
```
![image](https://github.com/user-attachments/assets/12f132e2-428a-470d-91cc-428f734f8afa)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
```
![image](https://github.com/user-attachments/assets/631cb1ed-b132-427f-a03b-09768f5cb121)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("Sine wave form")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/user-attachments/assets/d431853d-0324-479f-a93f-e9854d498127)

```
import matplotlib.pyplot as plt
import numpy as np
#Create some random data
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]

y2 = [5, 7, 9, 11, 13]

y3 = [2, 4, 6, 8, 10]

#Create the plot
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()

```
![image](https://github.com/user-attachments/assets/308be07e-364f-436c-9303-e0e4ad44ab9f)

```
plt.stackplot(x, y1, y2, y3, labels=['Line 1', 'Line 2', 'Line 3'])

plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/466b0ec3-60f5-46c1-baf1-a93d30cac994)

```
import matplotlib.pyplot as plt

# heights of bars
height = [10, 24, 36, 40, 5]

# labels for bars

names = ['one', 'two', 'three', 'four', 'five'] # plotting a bar chart
c1 = ['red', 'green']
c2=['b', 'g']
# we can use this for color
plt.bar (names, height, width=0.8, color=c1)

# naming the x-axis

plt.xlabel('x - axis')

# naming the y-axis

plt.ylabel('y - axis')

# plot title

plt.title('My bar chart!')

# function to show the plot

plt.show()
```
![image](https://github.com/user-attachments/assets/c68156a8-cc98-4066-953c-d8bcc689f63f)

```
x = [2,8,10]

y = [11,16,9]

x2 = [3,9,11]

y2 = [6,15,7]

plt.bar(x, y,color='r')

plt.bar(x2, y2, color = 'g')

plt.title('Bar graph')

plt.ylabel('Y axis')

plt.xlabel('X axis')

plt.show()
```
![image](https://github.com/user-attachments/assets/175255bd-4495-480e-86ff-ef487f0d3685)

```
import matplotlib.pyplot as plt

# frequencies

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
#setting the ranges and no. of intervals

range = (0,100)

bins = 10

# plotting a histogram

plt.hist(ages, bins, range, color='green', histtype='bar', rwidth=0.8)

# x-axis label

plt.xlabel('age')

# frequency label

plt.ylabel('No. of people')

# plot title

plt.title('My histogram')

# function to show the plot

plt.show()
```
![image](https://github.com/user-attachments/assets/c1e6e660-7854-470c-8279-c45f31724f07)

```
import matplotlib.pyplot as plt

#generate fake data

x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1] #plot for a histogram

plt.hist(x, bins = 10, color='blue', alpha=0.5)

plt.show()
```
![image](https://github.com/user-attachments/assets/6d616455-c25e-47b4-9649-2eed59b70942)

```
import matplotlib.pyplot as plt
import numpy as np
data=np.random.normal(loc=0, scale=1, size=100)
data
```
![image](https://github.com/user-attachments/assets/cd1108c4-fd7c-4ffb-8635-f9e7303552d1)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Value')
ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/d6aa51a5-8265-4524-a2c1-418ed91e863c)

```
import matplotlib.pyplot as plt

# defining labels

activities = ['eat', 'sleep', 'work', 'play']

# portion covered by each label

slices = [3, 7, 8, 6]

# color for each label
colors = ['r', 'y', 'g', 'b']

# plotting the pie chart

plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '81.1f88')

# plotting legend

plt.legend()

# showing the plot

plt.show()
```
![image](https://github.com/user-attachments/assets/a86bf308-23d2-435b-9a47-8691c2c8eef0)

```
# Data to plot

labels = 'Python', 'C++', 'Ruby', 'Java'

sizes = [215, 130, 245, 210]

colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']

explode = (0, 0.4, 0, 0.5)

# Plot
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)

plt.axis('equal')

plt.show()
```
![image](https://github.com/user-attachments/assets/b9a959da-9441-4fab-9f9e-9e75168a5e3f)


# Result:
  Hence, Data Visualization using matplot python library for the given datas are executed successfully.
