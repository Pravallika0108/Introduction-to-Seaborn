## Introduction

Seaborn is a library used for Data Visualization which built on top of Matplotlib and offers many advanced data visualization capabilities. It also provides high-level interface to draw statistical graphs.

Though `seaborn` library can be used to draw various types of plots like matrix plots, grid plots etc. In this article we will see how to draw distributional plots using `distplot()`. For this we are going to use the titanic dataset which contain 891 rows and 15 columns. which is downloaded by default with the `seaborn` library.

But for the demonstration we will be using only a few rows as shown below.

## Distribution of data using functions distplot() and jointplot()

The `seaborn` library can be downloaded in 2 ways. If you are using `pip` installer for the python libraries you can execute the following command.

```python
pip install seaborn 
```
Alternatively if you are using conda distribution of Python you can execute the following command.

```python
conda install seaborn
```

{We name it as `Distributional plots`. This shows the statistical distribution of the data. 

distplot() shows the distribution of the data for a single column. The column name is passed as a parameter to the `distplot()` function.
Let us execute the below script and see how the price of the ticket for each passenger is distributed.

```python
import matplotlib.pyplot as plt
import seaborn as sns

sns.distplot(df[ 'fare' ])
```
The dataset contains 891 rows, the preview of 4 rows with 15 columns is shown below.   

| | survived | pclass | sex | age | sibsp | parch | fare | embarked | class | who | adult_male | deck | embark_town | alive | alone|
| --- | --- | ---- | ---- | --- | ---- |
| 0 | 0 | 3 | male | 22.0 | 1 | 0 | 7.2500 | S | Third | man | True | NaN | Sounthamtopn | no | False |
| 1 | 1 | 1| female | 38. 0 | 1 | 0 | 71.2833 | C |First | women | False | C | Cherbourg | yes | False |
| 2 | | 1 | 3 | female | 26.0 | 0 | 0 | 7.9250 | S | Third | women | False | NaN | Southamptom | yes | True |
|3 | 1 | 1 | female | 35.0 | 1 | 0 | 53.1000 | S | First | women | Flase | C | Southampton | yes | False |


