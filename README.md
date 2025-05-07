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
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
```
```
x=[2018,2019,2020,2021,2022]
y=[15000,20000,25000,30000,35000]
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```

![image](https://github.com/user-attachments/assets/98f3a608-bf5b-4a44-afa6-cffd91b92488)


```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```

![image](https://github.com/user-attachments/assets/e4c57562-f902-4725-bb19-803e3b97598c)


```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```

![image](https://github.com/user-attachments/assets/cfbc04e3-1f4c-4760-a919-92ea57480098)


```
x=[2,8,10]
y=[11,16,9]
x1=[3,9,11]
y1=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x1,y1,color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

![image](https://github.com/user-attachments/assets/500a958e-6113-45ce-821c-dad7def2bd5d)


```
x=[1,2,3]
y=[7,3,9]
plt.plot(x,y,color='g')
plt.title("my first graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

![image](https://github.com/user-attachments/assets/86bd3279-5eb6-42a4-ae0c-0963fda75479)


```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.title('This is multi-line raph means two lines are same')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/19c34443-0593-4af1-a845-ce880f9d437f)


```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='red',markersize=12,label='spices')
plt.ylim(1,8)
plt.xlim(1,8)
plt.title('Line graph')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/323aa499-c499-40b6-b0c9-7d9a09a2d90a)


```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples,linestyle='dashed',linewidth=3,marker='*',markersize=12,color='green')
plt.show()
```

![image](https://github.com/user-attachments/assets/5b2fd3d8-78e1-4a5b-9d55-9159e0cba10b)


```
oranges=[2,4,6,7,8,12,45]
apples=[2,4,5,6,8,23,37]
years=[2019,2020,2021,2022,2023,2024,2025]
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='*')
plt.title("crop yields in kanto")
plt.xlabel('Years')
plt.ylabel('Yield(tons per hectare)')
plt.legend(['apples','oranges'])
plt.show()
```

![image](https://github.com/user-attachments/assets/b38d797c-cb3f-459b-bbf6-925e4b4076b9)


```
oranges=[2,4,6,7,8,12]
apples=[2,4,5,6,8,23]
years=[2019,2020,2021,2022,2023,2024]
plt.bar(oranges,apples)
plt.plot(years,apples,label='apples',marker='*')
plt.plot(years,oranges,label='oranges',marker='o')
plt.title("Fruit sales")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/39659563-0310-4a1b-ab69-16038dd8d2a0)


```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o',label='oranges')
plt.title("Yield of oranges(tons per hectare)")
plt.legend()
```

![image](https://github.com/user-attachments/assets/d67efcf3-7d54-4963-823b-8eaa0a837a22)


```
print("scatter plot is:")
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label='star',color='green',marker='*',s=30)
plt.title("my scatterplot!")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/8e9db69a-0155-4ed4-8c6d-52210e5f26a9)


```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='green',label='y1')
plt.fill_between(x,y2,color='blue',label='y2')
plt.fill_between(x,y3,color='red',label='y3')
plt.title("fill between is")
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/c6a0c54f-def5-47ce-a586-53f5c387dc98)


```
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title("stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

![image](https://github.com/user-attachments/assets/1fbfa352-f2d1-402b-9bc5-1da1201a1947)


```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,9,10,11,12,13])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100) # Changed linespace to linspace
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='spline')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/51209666-89d4-47a5-9226-b4e1ad109501)


```
values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()
```

![image](https://github.com/user-attachments/assets/533c44ea-0da7-4afc-a921-bbf6b0dd02f5)


```
ages=[2,5,70,40,45,50,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range1=(0,100)
bins=10
plt.hist(ages,bins,range1,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no.of people')
plt.title('my histogram')
plt.show()
```

![image](https://github.com/user-attachments/assets/54511fea-7d8f-4360-9801-59ef5ca9d3f7)


```
x=[2,1,6,2,4,8,9,4,2,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='green',alpha=0.5)
plt.show()
```

![image](https://github.com/user-attachments/assets/af67aff8-746e-49d2-b928-6e3496c03749)


```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![image](https://github.com/user-attachments/assets/33379f99-1fb5-4ccf-9422-f24c4ba1379d)


```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
```

![image](https://github.com/user-attachments/assets/9409c2f6-2ba0-4d01-897e-1d4b4e8b7b37)


```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/fb21773c-2cdc-4d11-bfb0-e37f934b9406)


```
labels='python','C+','ruby','java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,colors=colors,labels=labels,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![image](https://github.com/user-attachments/assets/ba9ae955-6079-4687-9252-437d34bcb391)






# Result:
Thus , all te data visualization techniques of matplotlib has been implemented successfully.
