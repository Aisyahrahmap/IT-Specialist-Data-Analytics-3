# Data Visualization Using Python
Python offers several plotting libraries, namely Matplotlib, Seaborn, and may other such data visualization packages with different features for cerating informative, customized, and appealing plots to present data in the most simple and effective way.

## Matplotlib and Seaborn
Matplotlib and Seaborn are Python libraries that use for data visualization. They have inbuilt modules for plotting different graphs.

`1. Matplotlib`
- It is used for basic graph plotting like Line Chart, Bar Graphs, etc.
- It mainly works with datasets and arrays.
- Matplotlib acts productively with data arrays and frames. It regards the aces and figures as objects.
- Matplotlib is more customizable and pairs well with Pandas and Numpy for Exploratory Data Analysis.
  
`2. Seaborn`
- It is mainly used for statistics visualization and can perform complex visualizations with fewer commands.
- It works with entire datasets.
- Seaborn is considerably more organized and functional than Matplotlib and treats the entire dataset as a solitary unit.
- Seaborn has more inbuilt themes and is mainly used for statistical analysis.

```python
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns
```

## Line Chart
A line chart is a graph that represents information as a series of data points connected by a straight line. In line charts, each data point or marker is plotted and connected with a line or curve.

Let's consider the apple and manggo yield (tons per hecater) in Kanto. Let's plot a line graph using this data and see how the yield od apples changes over time. We are going to both plot by using Matplotlib and Seaborn as follows:

`Using Matplotlib`

```python
plt.plot(years, apples)
plt.plot(years, manggo)

plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')

plt.title('Crop Yields in Kanto')
plt.legend(['Apples', 'Manggo'])
```
![image](https://github.com/Aisyahrahmap/IT-Specialist-Data-Analytics-3/assets/166115307/f117d72e-77f9-40a4-a8a3-0c5fdb510cee)

