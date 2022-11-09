---
name: Assignment_10
tools: [Python, vega-lite,altair,Jekyll]
image: assets/pngs/cars.png
description: This assignment is to get some more practice developing on the web, specifically exporting plots made in Python+altair+vegalite to your github repository.!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Group 15 - Vishwa Pancholi(vhp2) and Sonam Kumari (sonamk2)

Data Viz 1:

<vegachart schema-url="{{ site.baseurl }}/assets/json/sqaurefootage_wrt_bldgstatus.json" style="width: 100%"></vegachart>

Little more text :

Data Viz 2:

<vegachart schema-url="{{ site.baseurl }}/assets/json/usage_description.json" style="width: 100%"></vegachart>

Little more text :

Data Viz 3:

<vegachart schema-url="{{ site.baseurl }}/assets/json/heatmap_linechart.json" style="width: 100%"></vegachart>

Little more text :



## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

