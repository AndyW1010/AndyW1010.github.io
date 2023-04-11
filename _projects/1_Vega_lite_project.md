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
<vegachart schema-url="/assets/json/cars.json" style="width: 100%"></vegachart>


```
<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AndyW1010/is445-hw10/blob/main/Andy-Wang-HW10.ipynb" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AndyW1010/is445-hw10/blob/main/Andy-Wang-HW10.ipynb" text="The Analysis" %}
</div>

