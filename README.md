# Data Visualization Using Python
Python offers several plotting libraries, namely Matplotlib, Seaborn, and may other such data visualization packages with different features for creating informative, customized, and appealing plots to present data in the most simple and effective way.

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

Let's consider the apple and manggo yield (tons per hectare) in Kanto. Let's plot a line graph using this data and see how the yield of apples and manggo changes over time. We are going to both plot by using Matplotlib and Seaborn as follows:

`Using Matplotlib`

```python
plt.plot(years, apples)
plt.plot(years, manggo)

plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')

plt.title('Crop Yields in Kanto')
plt.legend(['Apples', 'Manggo'])
```
![image](https://github.com/Aisyahrahmap/IT-Specialist-Data-Analytics-3/assets/166115307/bc50f730-3665-4783-880e-beec89b9ef61)


# CRISP-DM
CRISP-DM or CRoss Industry Standard Process for Data Mining is a process model with six phases that naturally describes the data science life cycle. It’s like a set of guardrails to help you plan, organize, and implement your data science (or machine learning) project.

### 6 phase of the CRISP-DM
**1. Business Understanding**  
The Business Understanding phase focuses on understanding the objectives and requirements of the project. Aside from the third task, the three other tasks in this phase are foundational project management activities that are universal to most projects:  
a. **Determine business objectives**: You should first “thoroughly understand, from a business perspective, what the customer really wants to accomplish.”  
b. **Assess situation:** Determine resources availability, project requirements, assess risks and contingencies, and conduct a cost-benefit analysis. 
c. **Determine data mining goals:** In addition to defining the business objectives, you should also define what success looks like from a technical data mining perspective.  
d. **Produce project plan:** Select technologies and tools and define detailed plans for each project phase.

**2. Data Understanding**
Adding to the foundation of Business Understanding, it drives the focus to identify, collect, and analyze the data sets that can help you accomplish the project goals. This phase also has four tasks:  
a. **Collect initial data:** Acquire the necessary data and (if necessary) load it into your analysis tool.
b. **Describe data:** Examine the data and document its surface properties like data format, number of records, or field identities.
c. **Explore data:** Dig deeper into the data. Query it, visualize it, and identify relationships among the data.
d. **Verify data quality:** How clean/dirty is the data? Document any quality issues.
