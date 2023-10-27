---
name: Covid-19 Death Cases in Illinois 
tools: [Python, HTML, vega-lite]
image: assets/pngs/cancer.jpg
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Covid-19 Death Cases in Illinois 




<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_atlas.json" style="width: 100%"></vegachart>


<div class="left">
{% include elements/button.html link="https://data.illinois.gov/dataset/635reportable_communicable_disease_cases_2010_2012" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AndyW1010/is445_final_part3/blob/main/Andy-Wang-finalpart3.ipynb" text="The Analysis" %}
</div>



