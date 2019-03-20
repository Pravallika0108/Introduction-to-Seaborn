## Introduction

In this article we will learn how to plot the data using seaborn

Seaborn is a library used for Data Visualization which built on top of Matplotlib and offers many advanced data visualization capabilities.

The dataset we are going to use to draw our plots will be titanic dataset which is downloaded by default with the seaborn library.

The dataset contains  891 rows and 15 coloumns 

The objective we use here is to show type of plots that show distribution of data using function`distplot()`

## Distribution of data using functions distplot() and jointplot()

If in case you doesn't have library just use the `pip` function to install package `seaborn` as shown below.

```python
!pip install seaborn 
```
Now import the library

```python
import matplotlib.pyplot as plt
import seaborn as sns
```
We name it as `Distributional plots`. This shows the statistical distribution of the data. 

distplot() shows the distribution of the data for a single column. The column name is passed as a parameter to the `distplot()` function.
Let us execute the below script and see how the price of the ticket for each passenger is distributed. 

```python
sns.distplot(df[ 'fare' ])
```

![alt text](https://drive.google.com/drive/u/1/search?q=type:image)

