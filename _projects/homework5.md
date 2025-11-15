---
name: Homework 5
tools: [Python, Altair, VegaLite]
description: Submission for HWK 5
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Chart 1

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot1.vl.json" style="width: 100%"></vegachart>

This plot shows sightings by U.S. state. The bar graph visually depicts the total number of Bigfoot sightings by U.S. state, based off of the BFRO dataset reports. In the plot, each bar represents how many total sightings were reported. I used quantitative encoding for the X-axis to depict the number of sightings, and nominal encoding for the Y-axis for the state. I chose the red color scale to highlight the intensity throughout the plot. Darker red means more sightings, so viewers are quickly draw to the higher-sighting states. The data transformation process consisted of counting and grouping rows by each state using the groupby Pandas function.

# Chart 2

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot2.vl.json" style="width: 100%"></vegachart>

This plot shows the interactive sightings over time by each region. The interactive scatterplot highlights Bigfoot sightings over time, being filtered by U.S. region. The X-axis is encoding the year each report was made, while the Y-axis represents the latitude to highlight geographic variation. I included a dropdown menu that lets users select a region (Midwest, West, South, or Northeast). This selection filters the interacrive data using Altair's selection_point with the binding_select control. This makes the visualization more interactive and engaging, while allowing users to find regional trends easily.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/anantyak/anantyak.github.io/blob/master/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
