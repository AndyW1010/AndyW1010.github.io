---
name: Vega Lite Example Project
tools: [Python, HTML, vega-lite]
image: /assets/pngs/pic.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 10



## Search The Data & Methods
<vegachart schema-url="/assets/json/chart1.json" style="width: 100%"></vegachart>
```
Reference：
Homework 9 code. I use similar graph to homework 9."I created a scatter plot visualization using Vega-Lite to display the relationship between the year a building was acquired and its square footage. The primary feature I wanted to highlight with this visualization was the trends between these two variables."

Design:
x: This is encoding the Year Acquired variable as a time-based axis, using the timeUnit parameter set to 'year', which tells Altair to aggregate the data by year. The data is also being cast to a temporal data type using the :T shorthand.
y: This is encoding the Square Footage variable as a quantitative axis, represented as a continuous axis (Q).

color: This is encoding a constant value (alt.value('red')) as the color of the points. I chose red because I think red is more attention-grabbing.
Difference bewteen this graph and homework 9: The 'opacity' encoding is added to the chart in the given code using the 'alt.condition' function. This sets the opacity of the selected points to 1 and the opacity of unselected points to 0.2.

Interactivity:
The graph includes the brush selection tool. This allows the user to select a range of data points by clicking and dragging their mouse over the chart. By selecting a range of points, the user can zoom in on a particular time period or range of square footage values, allowing them to identify trends and outliers that may be hidden in the dataset. This will make the plot clear to see.

Transformation:
The data aggregation is performed by Altair to group the Year Acquired variable by year.
```

<vegachart schema-url="/assets/json/chart2.json" style="width: 100%"></vegachart>
```
Desciption:
The chart is displaying the total square footage of buildings in each congressional district where the square footage is greater than 200,000. The x-axis is showing the congressional district and the y-axis is showing the total square footage.

Design：
The x-axis is using an ordinal scale to display the congressional district values, and the y-axis is using a quantitative scale to display the total square footage. The tooltip is encoding both congressional district and total square footage values as ordinal and quantitative scales respectively.

Data transformation：
I filter the data to only show buildings with a square footage greater than 200,000. This is being accomplished using the transform_filter() function, which is filtering the data based on the value of the 'Square Footage' column.

```



<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AndyW1010/is445-hw10/blob/main/Andy-Wang-HW10.ipynb" text="The Analysis" %}
</div>

