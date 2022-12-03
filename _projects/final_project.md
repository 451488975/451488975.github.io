---
name: Netflix Has Far More Age Restrictive Contents Than You Think
tools: [Python, HTML, vega-lite]
image: assets/pngs/dataset-cover.jpg
description: Final project by Boyu Zhang, Phoebe Ling, River Liu, Shaojun Zheng
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Netflix Has Far More Age Restrictive Contents Than You Think
#### Author: Boyu Zhang, Phoebe Ling, River Liu, Shaojun Zheng

## Introduction
As one of the most popular movies and tv shows streaming platform, Netflix provides us countless entertaining contents to watch during every movie nights. But have you ever think about these questions when watching movies or tv shows on Netflix:

*What is average score of the movies in different year?*\
*Which genre has the most restrict-rated contents so I can avoid watching it with my children?*

Our project would help you answer these questions and hope we can give you a better understanding on some of the data behind Netflix.

## What Is The Average IMDB Score of Different Genres?
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_interactive1.json" style="width: 100%"></vegachart>

First, we want to explore the relationship between genre and imdb_score, whether a particular movie genre is more popular among audiences. So, we plotted a histogram with the X-axis representing the genre of the movie and the Y-axis representing the average imdb score of the movie. From the histogram, we can see that certain genres are indeed more popular with audiences. For example, history and war films have an average rating of over 7, while horror films have an average rating of under 6.

## How Many Movies Do Different Age Ratings have?
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_interactive2.json" style="width: 100%"></vegachart>

Next, we want to know the proportion of Movie Ratings and observe which grades of movies filmmakers like to shoot. So, we drew a histogram of movie ratings on the x-axis and the number of movies with each rating on the y-axis. The figure shows that the counts of TV-MA and R-rated movies are the largest, indicating that filmmakers tend to produce R (Under 17 requires an accompanying parent or adult guardian) and TV-MA (this program is specifically designed to be viewed by adults) movies. The producers and directors don't think too much about the children's movie market.

## How Many Movies Are There with Different Genres and Age Ratings?
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_interactive3.json" style="width: 100%"></vegachart>

In addition, we further understood the relationship between genre and movie rating, so we drew a heat map, the x-axis represents the subject matter of the movie, the y-axis represents the age rating of the movie, and the intersecting part represents both a movie genre and age certification from the number of movies, we can see that most of the drama-themed movies are TV-MA-rated, and most thriller-themed movies are R-rated.

## Interactive Dashboard

<span style="color:violet">*!!!Use your cursor to brush the top graph to see the changes in the bottom graph*</span>

<vegachart schema-url="{{ site.baseurl }}/assets/json/final_interactive.json" style="width: 100%"></vegachart>

The dashboard shows the number of shows and movies provided by Netflix by movies' or shows' primary genre and production country. An audience can use a mouse to select a range of countries and genres. The bar chart on the right side will show the average IMDB score of the movie or shows that match the condition the audience selected each released year.

## Conclusion

Netflix is one of the most popular over-the-top streaming services in the world. It is interesting to figure out what kind of movies and TV shows it provides and to infer their target audiences. Customers can also know if Netflix's service is suitable for them by seeing the analysis results of the Netflix dataset. We present the analysis in age, genre, and score.

In the first plot, we explored the quality of movies/shows by showing the average IMDb score of each genre with a histogram. We can see that certain genres are indeed more popular with audiences and get higher scores. Audiences who love history and war films may be satisfied with the films Netflix provides, but audiences who like to watch horror movies may feel disappointed with the films on Netflix, which have an average rating of under 6.

In the second plot, we showed the number of films in each rating. The figure shows that the counts of TV-MA and R-rated movies are the largest, indicating children and teenagers are not their target audiences. Even the family with children may not be the target as well.

In the third and fourth plots, we further explore the relationship between genre and movie rating and the relationship between genre and produced country by showing a heat map. This gives audiences comprehensive aspects of the genre, produced country, and moving rating.

Ultimately, we used a dashboard to show the relationship between primary genre, production country, released year, and the average IMDB score of films.

Those figures can help audiences comprehensively understand the films' features on Netflix and choose if this service is suitable for them.

<div class="left">
{% include elements/button.html link="https://query.data.world/s/7cdylzj6g2k4a7bahcloent6dhb3mf" text="Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/451488975/451488975.github.io/blob/main/python_notebooks/final_project_part 3.1.ipynb" text="Analysis" %}
</div>

