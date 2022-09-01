---
created: 2021-09-18T22:22:37 (UTC -04:00)
tags: []
source: https://www.storytellingwithdata.com/blog/2020/7/27/what-is-a-slopegraph
author: by Mike Cisneros
---

# what is a slopegraph, how is it used, and what is it good for — storytelling with data

> ## Excerpt
> In this article, we will discuss the line graph variant called a slopegraph via examples, how it is used for both continuous and categorical data, reasons why you should or shouldn't use it, and additional resources for exploring more about it in depth.

---
 A slopegraph looks like a [line graph](https://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph), but with an important difference: there are only two data points for each line. This might sound like a small distinction, but in practice it means something important: that we can compare two categorical variables, which we couldn’t normally do in a regular line graph.

## How does a slopegraph work?

When we use slopegraphs, we are trying to show one specific thing: is the value in the first column higher, lower, or the same as the value in the second column? That change is easy to see when we connect those values with lines, because the lines will slope up or down, in the direction of the change.

The steeper the slope, the bigger the change; and, if one thing is going up more dramatically than its neighbors, a slopegraph will make that easier to see than a traditional line graph would.

## What kind of data can be used in a slopegraph?

Slopegraphs can be used with either continuous data or categorical data. 

-   For slopegraphs that show a beginning and end point in time, it shows how values have changed over the intervening period.
    
-   For slopegraphs that show categorical comparisons, it shows which data series are markedly different across the two categories, and in which direction.
    

### Continuous data: highlighting change over time

A line graph with multiple series, each measured at multiple points in time, can quickly become visually cluttered. If the values in each series tend to fluctuate over time, the noisiness in the graph can obscure overall patterns of growth or decline. When you’re more interested in communicating “change over time” rather than each individual time period’s variations—or if you want to emphasize one particular series that is rising or falling notably, compared to others—a slopegraph is an option to consider.

For example, take this line graph of diabetes rates at medical centers in our area.

![Line graph example showing diabetes rates from 2015 to 2019.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883672372-DT1F660ZILR4M5MTNU0Y/Line+graph+example.png)

![Line graph example showing diabetes rates from 2015 to 2019.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883672372-DT1F660ZILR4M5MTNU0Y/Line+graph+example.png?format=750w)

Each line represents one of our region’s thirteen medical centers. Our region, Anytown, had one of the lowest patient diabetes rates in the area for the past five years, but it seemed to tick upward notably between 2017 and 2019. 

A slopegraph can help to call that out more obviously, and can point out which other centers had a similar increase.

![Slope chart example showing diabetes rates from 2017 to 2019](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883701697-HBP4I9VINHHCRHKQ0900/Slopechart+example.png)

![Slope chart example showing diabetes rates from 2017 to 2019](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883701697-HBP4I9VINHHCRHKQ0900/Slopechart+example.png?format=750w)

### Categorical data: highlighting differences between two categories

When we compare two categories that have a common scale, a slopegraph can be an excellent way to show how things compare across those categories.

 Imagine, for instance, that we work for a movie studio. We released six films in 2019, and we want to compare the overall audience ratings of these movies with the ratings of people in the key 18-34-year-old demographic. We could show these results as paired bar charts:

![Grouped bar chart example showing audience ratings for 2019 films.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883750716-TM7MJPUX362O7AOD4EPI/Grouped+bar+chart+example.png)

![Grouped bar chart example showing audience ratings for 2019 films.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883750716-TM7MJPUX362O7AOD4EPI/Grouped+bar+chart+example.png?format=750w)

This view certainly makes it easy to compare the ratings of the key demographic to the overall ratings within a single film, but a slopegraph would make the differences across the entire slate of films more obvious and prominent. 

![Slope chart example showing audience ratings for 2019 studio films.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883791823-D4RNIQG5J0UHEQI8F0VX/Slopechart+example.png)

![Slope chart example showing audience ratings for 2019 studio films.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1595883791823-D4RNIQG5J0UHEQI8F0VX/Slopechart+example.png?format=750w)

(We can also “zoom in” to see the detailed differences between each category, because slopegraphs, like line charts in general, do not necessarily have to start with a zero baseline; bar charts do not allow us this flexibility.) 

## What are some reasons not to use a slopegraph?

When working with continuous, time-series data, it’s important to remember that slopegraphs, by design, show the difference between a starting point and an ending point ONLY. We are thus excluding any and all data from the middle part of our time period. If that information provides essential context, then using a standard line chart would be a better choice.

Slopegraphs are not the best choice for categorical data when there’s no real connection between the selected categories. (That’s when slopegraphs wind up looking like piles of dried spaghetti dropped on the floor.) An ideal categorical slopegraph uses related (but not necessarily causally related) categories. 

  
One last caveat is that slopegraphs, like all line graphs, are primarily meant to emphasize the change between two values, or the comparative rates of change across several series—not the absolute quantities of those values. Use a [bar chart](http://www.storytellingwithdata.com/blog/2020/2/19/what-is-a-bar-chart) if it’s important to convey that your sales grew by precisely 20% or $300,000; use a slopegraph to show that your sales went up faster than your competitors’, or that they increased while other offices’ sales decreased.
