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
<vegachart schema-url="{{ site.baseurl }}/assets/json/new.json" style="width: 100%"></vegachart>

### Analysis Overview

The COVID-19 pandemic has significantly affected our world, altering our day-to-day lives in unprecedented ways. As part of our ongoing efforts to understand and interpret the progression of the disease, particularly in Illinois, we have developed a predictive model to forecast death cases in the coming years.

**Model Selection and Rationale:**  
We used the XGBoost model for our predictions. XGBoost is a gradient boosting framework that uses decision trees, and it's especially favored for its execution speed and model performance. For time series data like ours, capturing intricate patterns is of utmost importance. XGBoost, with its ability to handle non-linear relationships and potential interactions between features, seemed apt.

**Features Used:**  
- **Date**: We used the dates to extract month and year, which helped the model understand temporal trends.
- **County**: Each county might have different patterns based on population density, healthcare infrastructure, and other socio-economic factors.
- **Cases**: The number of cases can directly influence the number of deaths, and it's essential for our model.

**Results:**  
The interactive visualizations presented above show the predicted number of deaths for each county in Illinois for the years 2024 and 2025. From our predictions, it's evident that:
- There are certain months where a spike in death cases is predicted.
- Some counties are predicted to have higher death tolls than others.

**Limitations and Future Work:**  
While the model provides valuable insights, it's essential to note that predictions are based on historical data and might not account for future interventions, like the introduction of new vaccines or changes in public health policies. In the future, we aim to incorporate more external factors, refine our model, and possibly explore other predictive algorithms tailored for time series forecasting.

**Data Source and Analysis:**  
The data used for this analysis has been sourced from the official Illinois government database. For those interested in diving deep into the numbers and our model's intricacies, please find the links to the raw data and detailed analysis below.

<div class="left">
{% include elements/button.html link="https://data.illinois.gov/dataset/635reportable_communicable_disease_cases_2010_2012" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AndyW1010/is445_final_part3/blob/main/Andy-Wang-finalpart3.ipynb" text="The Analysis" %}
</div>
