---
name: Group 9 Homework 10
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: Homework 10 by Boyu Zhang, Phoebe Ling, River Liu, Shaojun Zheng
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 10
#### Author: Boyu Zhang, Phoebe Ling, River Liu, Shaojun Zheng

## Plot 1
<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_1.json" style="width: 100%"></vegachart>

The first graph explores the total number of License types. The X-axis is the name of each License Type, which is nominal data, while the Y-axis records the total number of License types, which is quantitative data. The encoding Type we use is bar chart Y. Bar Chart can clearly and intuitively display the number of different License types.

In this figure, we did the data conversion because MaxRowsError appears when I try to create a drawing that will directly embed a dataset with more than 5000 rows, so we simply disable MaxRowsError.

## Plot 2

*Use your cursor to brush the left graph to see the changes in the right graph!!!*

<vegachart schema-url="{{ site.baseurl }}/assets/json/sidebyside.json" style="width: 100%"></vegachart>

The heatmap shows how many licenses each state and status, and the bar chart shows how many licenses each type. We used 'ordinal' in encoding type because it is easy for audiences to find the category they are interested in. The heatmap uses color gradients to show the number of licenses. The bar chart used Phoebe Ling's homework #9 plot2, but we changed the color display to the heatmap's color display. Because nowhere can we show the number in the heatmap, we use color to express the amount. We are interested in all kinds of licenses instead of a specific category, so we didn't use Python to filter the data. We use the original dataset to make the plot.

We are not satisfied with just knowing the number of licenses. We want to understand the amount of licenses in different states and their status. The interactive dashboard can help us see the amount of each type under specific state and status.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/451488975/451488975.github.io/blob/main/python_notebooks/group9_homework10.ipynb" text="The Analysis" %}
</div>

