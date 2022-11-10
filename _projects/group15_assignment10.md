---
name: Assignment_10
tools: [Python, vega-lite,altair,Jekyll]
image: assets/pngs/building.png
description: This assignment is to get some more practice developing on the web, specifically exporting plots made in Python+altair+vegalite to your github repository.!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Assignment 10

##### Group 15 - Vishwa Pancholi(vhp2) and Sonam Kumari (sonamk2)


Data Viz 1:

Relationship between mean square footage and building status

<vegachart schema-url="{{ site.baseurl }}/assets/json/sqaurefootage_wrt_bldgstatus.json" style="width: 100%"></vegachart>

The above scatter plot shows the relationship between mean sqaure footage and building status. We have considered quantitative encoding for square footage and nominal for building status. We have not used any specific colour scheme for the plot.The x axis ranges from 0 to 20,000. In progress buildings have most sqaure footage.

Data Viz 2:

Agency Frequency

<vegachart schema-url="{{ site.baseurl }}/assets/json/agency_frequency.json" style="width: 100%"></vegachart>

In the above graph we can see the frequency each agency. We have considered nominal encoding for agency name as it is categorical variable.We have not used any particular color scheme for this plot. Department of Natural Resource has the highest count of records which is nearly 3,250.

Data Viz 3:

Interactive Usage Description over years

<vegachart schema-url="{{ site.baseurl }}/assets/json/usage_description.json" style="width: 100%"></vegachart>

In the above interactive graph we have plotted the Year Constructed on X axis and sum of square footage on Y-axis. The usage description is used as legend and the color is dependent on it. We have considered temporal enciding for year constructed, quantitative for square footage and nominal for usage description.The color scheme of tableau20 is dependent on legend(usage description). When you click on any legend (usgae description) , the data for that particular selection is highlighted.

Data Viz 4:

Interactive heat map and line chart

<vegachart schema-url="{{ site.baseurl }}/assets/json/heatmap_linechart.json" style="width: 100%"></vegachart>

In the above graphs the first one is a heatmap that shows a relationship between Usage Description and Agency Name on Y-axis and X-axis respectively.We have considered nominal encoding for usage desciption and agency name while for square footage we have taken quantitative encoding. The color of heat map is represented by median of Square Footage. When we are selecting any value(tile) here accordingly the plot in the side line graph shows mean of square footage over Year Acquired for that particular usage description and agency name selection. In the second graph which is interactive we have also used building status for legend and define color. We have taken temporal encoding for year acquired , quantitative for square footage and nominal for building status.I have taken tableau20 to define color which is represented by building status.



<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Vishwa79/vishwa79.github.io/blob/main/python_notebooks/group15-pancholi-vishwa-kumari-sonam-assignment10.ipynb" text="The Analysis" %}
</div>

