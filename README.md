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

### 6 phase of the CRISP-DM:

*1. Business Understanding*
     
The Business Understanding phase focuses on understanding the objectives and requirements of the project. Aside from the third task, the three other tasks in this phase are foundational project management activities that are universal to most projects:  

- *Determine business objectives:* You should first “thoroughly understand, from a business perspective, what the customer really wants to accomplish.”
- *Assess situation:* Determine resources availability, project requirements, assess risks and contingencies, and conduct a cost-benefit analysis.
- *Determine data mining goals:* In addition to defining the business objectives, you should also define what success looks like from a technical data mining perspective.
- *Produce project plan:* Select technologies and tools and define detailed plans for each project phase.

*2. Data Understanding*

Adding to the foundation of Business Understanding, it drives the focus to identify, collect, and analyze the data sets that can help you accomplish the project goals. This phase also has four tasks:   

- *Collect initial data:* Acquire the necessary data and (if necessary) load it into your analysis tool.  
- *Describe data:* Examine the data and document its surface properties like data format, number of records, or field identities.  
- *Explore data:* Dig deeper into the data. Query it, visualize it, and identify relationships among the data.  
- *Verify data quality:* How clean/dirty is the data? Document any quality issues.

*3. Data Preparation*

This phase, which is often referred to as “data munging”, prepares the final data set(s) for modeling. It has five tasks:  

- *Select data:* Determine which data sets will be used and document reasons for inclusion/exclusion.  
- *Clean data:* Often this is the lengthiest task. Without it, you’ll likely fall victim to garbage-in, garbage-out. A common practice during this task is to correct, impute, or remove erroneous values.  
- *Construct data:* Derive new attributes that will be helpful. For example, derive someone’s body mass index from height and weight fields.  
- *Integrate data:* Create new data sets by combining data from multiple sources.  
- *Format data:* Re-format data as necessary. For example, you might convert string values that store numbers to numeric values so that you can perform mathematical operations.

*4. Modeling*

What is widely regarded as data science’s most exciting work is also often the shortest phase of the project. Here you’ll likely build and assess various models based on several different modeling techniques. This phase has four tasks:  

- *Select modeling techniques:* Determine which algorithms to try (e.g. regression, neural net).  
- *Generate test design:* Pending your modeling approach, you might need to split the data into training, test, and validation sets.  
- *Build model:* As glamorous as this might sound, this might just be executing a few lines of code like “reg = LinearRegression().fit(X, y)”.  
- *Assess model:* Generally, multiple models are competing against each other, and the data scientist needs to interpret the model results based on domain knowledge, the pre-defined success criteria, and the test design.

*5. Evaluation*

Whereas the Assess Model task of the Modeling phase focuses on technical model assessment, the Evaluation phase looks more broadly at which model best meets the business and what to do next. This phase has three tasks:  

- *Evaluate results:* Do the models meet the business success criteria? Which one(s) should we approve for the business?  
- *Review process:* Review the work accomplished. Was anything overlooked? Were all steps properly executed? Summarize findings and correct anything if needed.  
- *Determine next steps:* Based on the previous three tasks, determine whether to proceed to deployment, iterate further, or initiate new projects.

*6. Deployment*

A model is not particularly useful unless the customer can access its results. The complexity of this phase varies widely. This final phase has four tasks:

- *Plan deployment:* Develop and document a plan for deploying the model  
- *Plan monitoring and maintenance:* Develop a thorough monitoring and maintenance plan to avoid issues during the operational phase (or post-project phase) of a model  
- *Produce final report:* The project team documents a summary of the project which might include a final presentation of data mining results.  
- *Review project:* Conduct a project retrospective about what went well, what could have been better, and how to improve in the future.
