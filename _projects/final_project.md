---
name: Chicago Food Inspection
tools: [Python, vega-lite,altair,Jekyll]
image: assets/pngs/building.png
description: This article will help in determining where to eat in chicago in order to be safe and which areas of the city should be avoided.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Where to eat safely in Chicago ?





######              - Vishwa Pancholi(vhp2) and Sonam Kumari (sonamk2)



When visiting a different city, we frequently wish to sample the local cuisine. We occasionally worry about whether the food we intend to purchase is secure and up to hygienic standards. I'd like to take you on a quick tour of Chicago, the third-largest city in the United States. We'll look at where to dine to stay safe and which parts of the city to avoid. 

Our database has more than 29 thousand rows with information pertaining to location , address, risk, inpsections , results and much more. Although the primary database has 17, not all of them are necessary for analysis. Information concerning location (latitude and longitude), the kind of food spot, the kind of inspection, the outcome of the control, and risk are the most crucial.

Lets start by examining the ditribution of food faciliity by categories.

<vegachart schema-url="{{ site.baseurl }}/assets/json/testing.json" style="width: 100%"></vegachart>


We can observe from above that Restaurants and diners has most records which makes sense but strange thing observed was about the Banquet Halls present in chicago. How come there were only 4 inspections of the same. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/risk_bar.json" style="width: 100%"></vegachart>

Let's now examine the risk type. Risk can be classified as high, medium, or low. Over 70% of the audited locations had high risk. The second one is medium and has a participation rate of about 20%. The third one is low risk (every 11 spot has such a risk). There are also a few places which come under all risk types.
<vegachart schema-url="{{ site.baseurl }}/assets/json/result_bar.json" style="width: 100%"></vegachart>

Now coming to results , we observe that most facilities got pass(more than 50%).The second one is "Fail"; following control, almost 6 thousand people don't receive a favorable impression. Popularity also works with restrictions (more than 10% of spots produced that result). Rarely do circumstances arise where doors are closed, a location isn't suitable for control, or even doesn't exist.

<vegachart schema-url="{{ site.baseurl }}/assets/json/heatmap1.json" style="width: 100%"></vegachart>
It's time to compare the information we know about the danger and various kinds of controls. Combination passes and high risk are the most common (almost half of controls). The second one (4762) is fail and high risk. The last combination over 10% pass with medium risk. There appears to be no relationship between these two factors.


<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboards_1.json" style="width: 100%"></vegachart>
The dashboard represents 2 graph, first one is the heat map which is similar to one represented before and it provides information about relationship between results and risk. The color of the tile helps in determining the number of records of facility category for each combination, a tile from it can be chosen to further see the stacked bar chart for distribution of various facility categories. We observe that only grocery stores which provide food have 'All' type of risk category and result as no entry.There are no facilities which low risk and business not located. Coming to the most relevant combination as determined above, is of Pass with high risk and the stacked bar chart shows that most of the records are restaurants.

To conclude we can say that more than 50% of facilities pass inspection without any requirements (20% fail).Most places have a first category of danger (high).No restaurant facility has a lower risk profile more frequently than eateries.The center has the maximum spot density (around Chicago Theater, Millenium Park and Willis Tower).In Chicago, there is no spatial separation between different risk and control kinds.


Refrences :
- Dataset : https://data.cityofchicago.org/Health-Human-Services/Food-Inspections/4ijn-s7e5
- https://vega.github.io/vega-lite/docs/type.html#:~:text=The%20supported%20data%20types%20are,%22%20%2C%20and%20%22geojson%22%20.
- https://altair-viz.github.io/



<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/Vishwa79/vishwa79.github.io/main/python_notebooks/clean_food_inspection.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Vishwa79/vishwa79.github.io/blob/main/python_notebooks/group15-pancholi-vishwa-kumari-sonam-final-project.ipynb" text="The Analysis" %}
</div>

