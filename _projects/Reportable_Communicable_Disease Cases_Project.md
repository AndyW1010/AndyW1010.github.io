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




<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard.json" style="width: 100%"></vegachart>



The interactive dashboard I have created allows non-experts to easily explore and visualize the number of reported cases for different diseases over time. The bar chart displays the total number of cases for each disease, with the option to highlight a specific disease by hovering over it. In the barchart, the highlighted bar is colored in steel blue and the non-highlighted bars are grey.The line chart shows the number of cases per year, with the option to filter by disease type. By selecting a disease in the bar chart, the line chart will update to display only that disease's cases over time. This provides an easy way to see how the number of cases has changed for a specific disease compared to others in the dataset. Additionally, hovering over a bar displays the disease name and total number of cases, providing users with more detailed information.





## Contextual visualizations

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart_1.json" style="width: 100%"></vegachart>

<div class="left">
{% include elements/button.html link="https://data.chhs.ca.gov/dataset/infectious-disease/resource/75019f89-b349-4d5e-825d-8b5960fc028c" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>

I create a bar chart using the Altair library in Python, which contains case counts and rates for selected communicable diseases—listed in the data dictionary—that met the surveillance case definition for that disease and was reported for California residents, by disease, county, year, and sex.
The x-axis of the chart displays the name of each disease, while the y-axis displays the number of reported cases for each disease.
The color of each bar represents the number of cases, with a color scale that goes from light blue (low cases) to dark blue (high cases). The chart is customized with font sizes, axis labels, and a title.
Overall, this chart is a useful way to visualize and compare the number of reported cases for different diseases, which can help identify patterns and trends in public health data.

![avatar](assets/pngs/disease-burden-to-communicable-diseases-vs-gdp.png)
<div class="middle">
{% include elements/button.html link="https://ourworldindata.org/grapher/disease-burden-to-communicable-diseases-vs-gdp" text="The Data" %}
</div>

