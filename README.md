<p align="center">
    <img src="https://howtolearnmachinelearning.com/wp-content/uploads/2021/04/coursera_machine_learning_ibm.png?raw=true" alt="IBM and Coursera Logos" width="926" height="133"/>
</p>

# Data Visualization with Python

This is the Final Project for Generative AI Course as a Part of IBM's Data Analyst Professional Certificate from Coursera.

I take on the role as a Data Analyst  by a Healthcare consultancy firm which has been conducting a survey on the state of global happiness annually. The World Happiness Report offers valuable insights into factors influencing happiness across countries. The firm wants me to produce a report to find out whether there are demographic, regional, and/or economic characteristics that lead to a better life.

As a Data Analyst, I will be assisting with this initiative and have been tasked with collecting data from various sources and identifying trends for this year's report on emerging skills.

### Task 1

The first task is to collect data about the factors that influencing happiness across countries. 

### Task 2

Once I've collected enough data, I will take the collected data and prepare it for analysis by using data wrangling techniques like finding duplicates, removing duplicates, finding missing values, and inputting missing values.

### Task 3

Now that the data is ready, I will apply statistical techniques to analyze the data and identify insights and trends like: What are the influence of GDP per capita on heaLthy life expectancy? What are the influence of GDP per capita on happiness score? What are the correlation between happiness factor vs happiness score?

### Task 4

In the fourth task, I'll focus on choosing appropriate visualizations based on the data I want to present using charts, plots, and histograms to help reveal my findings and trends. 

### Task 5

For task 5, I will employ Jupyter Notebook to create interactive dashboards to help analyze and present the data dynamically.

### Task 6

For the final task, I will use my storytelling skills to provide a narrative and present the findings of my analysis.

## Table of Contents

- [Data Description](#data-description)
- [Tools](#tools)
- [Deliverables](#deliverables)
  - [Task 1: Data Collection](#task-1-data-collection)
  - [Task 2: Data Wrangling](#task-2-data-wrangling)
  - [Task 3: Exploratory Data Analysis](#task-3-exploratory-data-analysis)
  - [Task 4: Data Visualization](#task-4-data-visualization)
  - [Task 5: Dashboard Creation](#task-5-dashboard-creation)
  - [Task 6: Presentation of Findings](#task-6-presentation-of-findings)
- [Stretch Goals](#stretch-goals)

## Data Description

The World Happiness Report is a landmark survey of the state of global happiness. The reports review the state of happiness in the world today and show how the new science of happiness explains personal and national variations in happiness. This is a public dataset available on the Kaggle website as World Happiness Report under the CC0: Public Domain license.

The dataset I am going to use comes from the following source: https://www.kaggle.com/datasets/unsdsn/world-happiness/data under a CCO: Public Domain License.

I will be given a subset of the original data set in this capstone project. I will explore, analyze, and visualize this dataset and present my analysis.

The dataset is available as a .csv file here.

The below table lists the questions asked in the survey and the column under which the response was collected.

<details>
 <summary><strong>View Table</strong></summary>
<table>
  <thead>
    <tr>
      <th>Column Name</th>
      <th>Question Text</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Country</td>
      <td>
        Name of the country.
      </td>
    </tr>
    <tr>
      <td>Region</td>
      <td>
        Region the country belongs to 
      </td>
    </tr>
    <tr>
      <td>Happiness Score</td>
      <td>A metric measured in 2016 by asking the sampled people the question: "How would you rate your happiness?"</td>
    </tr>
    <tr>
      <td>Happiness Rank</td>
      <td>Rank of the country based on the Happiness Score</td>
    </tr>
    <tr>
      <td>Lower Confidence Interval/td>
      <td>Lower confidence interval of the Happiness Score</td>
    </tr>
    <tr>
      <td>Upper Confidence Interval</td>
      <td>
        Upper confidence interval of the Happiness Score.
      </td>
    </tr>
    <tr>
      <td>Economy (GDP per Capita)</td>
      <td>
          The extent to which GDP contributes to the calculation of the Happiness Score
      </td>
    </tr>
    <tr>
      <td>Family</td>
      <td>
        The extent to which family contributes to the calculation of the Happiness Score
      </td>
    </tr>
    <tr>
      <td>Health (Life Expectancy)</td>
      <td>
        The extent to which life expectancy contributes to the calculation of the Happiness Score
      </td>
    </tr>
    <tr>
      <td>LearnCodeOnline</td>
      <td>Have you used online resources to learn coding?</td>
    </tr>
    <tr>
      <td>Freedom</td>
      <td>
        The extent to which freedom contributes to the calculation of the Happiness Score
      </td>
    </tr>
    <tr>
      <td>Trust (Government Corruption)</td>
      <td>
        The extent to which trust contributes to the calculation of the Happiness Score
      </td>
    </tr>
    <tr>
      <td>Generosity</td>
      <td>
        The extent to which generosity contributes to the calculation of the Happiness Score
      </td>
    </tr>
    <tr>
      <td>Dystopia Residual</td>
      <td>Dystopia is an imaginary country that has the world's least-happy people. The residuals, or unexplained components, differ for each country, reflecting the extent to which the six variables either over- or under-explain average 2014-2016 life evaluations. These residuals have an average value of approximately zero over the whole set of countries.</td>
    </tr>
  </tbody>
</table>

</details>

## Tools

- [`python`](https://www.python.org/downloads/) v3.12.2
- [`pandas`](https://pandas.pydata.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for managing the data.
- [`numpy`](https://numpy.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for mathematical operations.
- [`seaborn`](https://seaborn.pydata.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for visualizing the data.
- [`matplotlib`](https://matplotlib.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for additional plotting tools.
- [`folium`](https://python-visualization.github.io/folium/latest/) for geospatial data visualization such as choropleth maps.
- [`plotly`](https://plotly.com/python/) for interactive plotting tools.
- [`Google Looker Studio`](https://lookerstudio.google.com/overview) for dashboards.
- [`IBM Cognos Analytics`](https://www.ibm.com/products/cognos-analytics) for dashboards.

## Deliverables

### Task 1: Data Collection

- [x] Collecting Data Using Web Scraping
- [x] Exploring Data

### Task 2: Data Wrangling

- [x] Finding Missing Values
- [x] Determine Missing Values
- [x] Finding Duplicates
- [x] Removing Duplicates
- [x] Normalizing Data

### Task 3: Exploratory Data Analysis

- [x] Distribution
- [x] Outliers
- [x] Correlation

### Task 4: Data Visualization

- [x] Visualizing Distribution of Data
- [x] Relationship
- [x] Composition
- [x] Comparison

### Task 5: Dashboard Creation

- [x] Dashboards

### Task 6: Presentation of Findings

- [x] Final Presentation

## Stretch Goals

- [ ] Create Dashboard in Google Looker or Tableau
