---
name: Reportable Communicable Disease Cases in Illinois Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/cancer.jpg
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Reportable Communicable Disease Cases in Illinois,2011-2017

Group Member: Andy(Jiazhi) Wang  

netid:jiazhiw2




<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard2.json" style="width: 100%"></vegachart>


<div class="left">
{% include elements/button.html link="https://data.illinois.gov/dataset/635reportable_communicable_disease_cases_2010_2012" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AndyW1010/is445_final_part3/blob/main/Andy-Wang-finalpart3.ipynb" text="The Analysis" %}
</div>


The interactive dashboard created using Altair, which is a Python visualization library. The purpose of this dashboard is to explore the relationship between disease cases and year in Illinois. The data is sourced from Illinois government that collects disease incidence data over time. The dashboard is composed of two charts: a bar chart and a line chart.

The bar chart displays the total number of cases for each disease in the dataset. The diseases are displayed on the x-axis, and the total number of cases for each disease is displayed on the y-axis. The color of each bar is determined by an interactive selection that highlights the selected disease on both the bar chart and the line chart.

The line chart displays the number of cases for each disease over time. The x-axis displays the year, and the y-axis displays the number of cases. Each disease is represented by a different color line. By hovering over a disease on the bar chart, the corresponding line chart is filtered to only show data for that specific disease over time.This provides an easy way to see how the number of cases has changed for a specific disease compared to others in the dataset. Additionally, hovering over a bar displays the disease name and total number of cases, providing users with more detailed information.



## Contextual visualization 1

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart_1.json" style="width: 100%"></vegachart>

<div class="left">
{% include elements/button.html link="https://data.chhs.ca.gov/dataset/infectious-disease/resource/75019f89-b349-4d5e-825d-8b5960fc028c" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AndyW1010/is445_final_part3/blob/main/Andy-Wang-finalpart3.ipynb" text="The Analysis" %}
</div>

I create a bar chart using the Altair library in Python, which contains case counts and rates for selected communicable diseases—listed in the data dictionary—that met the surveillance case definition for that disease and was reported for California residents, by disease, county, year, and sex.
The x-axis of the chart displays the name of each disease, while the y-axis displays the number of reported cases for each disease.
The color of each bar represents the number of cases, with a color scale that goes from light blue (low cases) to dark blue (high cases). The chart is customized with font sizes, axis labels, and a title.
Overall, this chart is a useful way to visualize and compare the number of reported cases for different diseases, which can help identify patterns and trends in public health data.


## Contextual visualization 2
### Disease burden due to communicable diseases vs. GDP per capita, 2019
![avatar](/assets/pngs/disease-burden-to-communicable-diseases-vs-gdp.png)
<div class="center">
{% include elements/button.html link="https://ourworldindata.org/grapher/disease-burden-to-communicable-diseases-vs-gdp" text="Visualization Source" %}
</div>
The graph shows the relationship between the burden of communicable diseases and the Gross Domestic Product (GDP) per capita in different countries. We can compare the impact of communicable diseases in Illinois to the impact in other countries. This may provide insights into the severity of communicable diseases in Illinois and how it compares to other regions globally. Additionally, the visualization can help illustrate the relationship between disease burden and economic indicators such as GDP per capita.

