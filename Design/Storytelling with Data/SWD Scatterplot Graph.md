---
created: 2021-09-18T22:21:59 (UTC -04:00)
tags: []
source: https://www.storytellingwithdata.com/blog/2020/5/27/what-is-a-scatterplot
author: by Alex Velez
---

# scatterplot graph: what is it, how to use it with examples — storytelling with data

> ## Excerpt
> In this article, we will discuss the scatterplot graph via examples, how it is used to tell a story, provide useful design tips and share alternative views (bubble charts, connected scatterplots, plus more).

---
A scatterplot is a niche chart, but it’s one of my favorites! If you are a statistician or work in a technical field, a scatterplot might be your go-to graph type. However, if you don’t perform a lot of statistical analysis, then these charts may be unfamiliar. Regardless of your current comfort level, scatterplots are extremely useful to focus on the relationship between two series—a scenario that is common in both technical and non-technical fields. Let’s explore some of the basics of scatterplots via an example; I’ll also cover tips for designing more effective ones and discuss common variations (bubble charts, connected scatterplots, etc.), too!  

## **What is a scatterplot?**

A scatterplot shows the relationship between two numerical variables plotted simultaneously along both the horizontal and vertical axis. They are common in scientific fields and often used to understand data rather than to communicate with it. This is not to say you should never communicate with one, but you should take explicit steps to make sure your chart is clear to an unfamiliar audience (something you should do with all charts!). Let’s look at a scenario where a scatterplot works nicely to communicate a finding. 

Imagine you’re an analyst in the beauty industry and your company wants to formulate a new lip care product. Before embarking on this endeavor, you are asked to do some research to see if there is a hole in the market. You uncover that lip care products are polarizing between male and female buyers, so there is an opportunity to create a new product that bridges the gap.

You might consider showing the relationship between male and female rating scores using a scatterplot, like the one below.

![Original_Scatter.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501618462-UX66QMP7FJ1HO86037SC/Original_Scatter.png)

![Original_Scatter.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501618462-UX66QMP7FJ1HO86037SC/Original_Scatter.png?format=750w)

Here are a couple of things worth noting about the above chart.

-   **It’s exploratory in nature.** A scatterplot was likely used to uncover this finding. Many statistical software packages output scatterplots to test the correlation between two variables. Although the graph used in the discovery phase is not always ideal for communicating final insights, it works in this case. I can see both sets of rankings simultaneously and also emphasize the hole in the market. I’ve categorized and labeled the points to make this graph legible, but an alternative chart—one that is more familiar—could work as well ([check out this post to see three alternatives for comparing metrics](https://www.storytellingwithdata.com/blog/2017/10/13/novel-vs-the-boring-old-bar-chart)). It all depends on your audience and specific scenario.
    
-   **Be mindful of the variable placement on the axes.** In this example, it doesn’t matter which variable is along the horizontal or vertical axis, but that won’t always be the case. Sometimes you’ll have both an independent and a dependent variable. An independent variable is exactly what its name implies: it’s not affected by the other variable. A dependent variable is likely the thing you are trying to measure, meaning it _is_ affected by your independent variable. It’s common practice to place the independent metric along the horizontal or x-axis and the dependent variable along the y-axis. It’s not wrong to invert these, but it might be unexpected causing an initial bit of confusion.
    
-   **Scatterplots show dots, not lines.** Scatterplots are very similar to [line charts](http://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph) in that they both display two numerical values; however, scatterplots tend to focus on individual data points (depicted with a dot) rather than aggregating multiple points into one distinct line. 
    

In its standard form, as seen above, scatterplots show the relationship between two things, but it’s not uncommon to display more than two dimensions, especially when exploring your data. We’ll look at a few common multi-dimensional variations in a moment, but before we do, let’s break down how to read a scatterplot. 

## **How do you read a scatterplot?**

The bulk of this post is dedicated to how you can use scatterplots for explanatory purposes despite them being a more technical graph type. As mentioned before, if you do use a scatterplot, be aware that you may need to break it down for your audience, and if it's their first time looking at one of these charts, you may need to explain how to read it. I'll step you through the process I take when examining scatterplots as well as link to additional resources.

1.  **Check the axes.** One of the first things I do when reading _any_ graph is to scan each axis. It's especially important when reading scatterplots as they contain multiple variables, so it's necessary to determine which variable is along which axis. I should also mention that not all scatterplots will display similar variables; some might compare different metrics with varying units of measure and scale. Understanding this early on will make it easier to interpret the relationship once you start looking at the data.
    
2.  **Visualize sections.** In the above example, I created sections by grouping the points into quadrants. This is helpful not only for communicating the finding in the lip care scenario but also for uncovering it. The next time you look at a scatterplot, ask yourself what lines you can draw or what natural breaks and groupings exist that will help you make sense of the comparison. 
    
3.  **Identify the shape.** I often take a step back from the graph, so I can attempt to summarize the individual points into a unified shape. Are they all moving in a single linear direction? Or maybe it's more of an exponential curve? Do the points increase as my eyes move along the axis? Having a description in mind helps me uncover and explain the relationship. For instance, in this [cost per mile example](http://www.storytellingwithdata.com/blog/2018/10/1/swdchallenge-scatterplot), we can see that the data points form a u-shape. This means that the cost is relatively high for both shorter and longer uses, but as we drive an average amount, the cost is more manageable. Keep in mind that there may not be a discernible shape, which is a perfectly valid finding (and suggests a weak or non-existent relationship between the variables).
    

I'd be remiss to not share any warnings at this point. I can still hear my stat professors drilling this mantra into my head, "correlation does not imply causation." Just because you uncover a relationship doesn't mean you've identified the underlying cause. For instance, in the lip care example, we found that brands preferred amongst men are less preferred amongst women. Does this mean that if a male likes a brand, a female won't? Absolutely not, or there wouldn't be an opportunity to create a bridge product. We can use findings to inform and make educated decisions, but to generalize the insight would be a misuse of data. This applies to other chart types as well, however I find that scatterplots are more susceptible to misreadings. I think it's because they focus on the relationship, making it easy to both speculate and extrapolate. (For more data pitfalls check out [our review](http://www.storytellingwithdata.com/blog/2020/1/21/recommended-reading-avoiding-data-pitfalls) of Ben Jones’ latest book, Avoiding Data Pitfalls.) 

If you are interested in reading more about interpreting scatterplots, check out [Lisa Charlotte Rost's post](https://blog.datawrapper.de/weekly-chart-lifesatisfaction/), where she takes you through her process with a multi-dimensional scatterplot, the bubble chart. Speaking of which, let's discuss these variations next.

## **What are common variations of scatterplots?**

**Bubble charts:** Let’s imagine the lip care example includes another dimension (such as packaging type, price, the active ingredient, etc.). We can encode this third variable by altering the size, color, or even the shape of the data points. This is a bubble chart. Bubble charts are useful for showing multi-dimensional relationships, but this comes at a cost since they are tough to read. Once we change the size of the circles, we start encoding information by area. Our eyes are not very good at measuring area, so specific comparisons are harder to make. I should also mention that many graphing applications don’t offer canned bubble chart templates. This means someone has to calculate the correct area of each circle, which can introduce human error. Also, as we play with color and shapes, we ask our audiences to do a lot of mental work to process the information. People can typically only hold about four pieces of visual information in their short term memory at any given time, so be mindful of the cognitive effort placed on the reader! That said, there are fantastic examples of explanatory bubble charts, like Hans Roslin’s famous [BBC video](https://www.youtube.com/watch?v=jbkSRLYSojo). What makes Hans' explanation so effective is his willingness and enthusiasm to step his audience through his animated bubble chart. If you are considering a bubble chart—or any multi-dimensional graph for that matter—consider your audience and how much effort you want to spend explaining how to read your graph. 

**Connected scatterplots:** I think of a connected scatterplot as a hybrid between a traditional scatterplot and a line chart. There are still two dimensions along the x- and y-axis, but a third dimension, usually time, is layered on with lines. The challenge is that we are accustomed to reading time from left to right, so to see it moving in every direction from point to point can be unsettling. As with all variations, each graph has an ideal use case, and with thoughtful annotations, labeling, and focused attention can be made clear to any audience. To learn more, check out [Dan Zvinca’s guest post](http://www.storytellingwithdata.com/blog/2018/2/19/connecting-the-dots) on the many roles of lines and look at the example of Bill Rapp’s [January 2018 #SWDchallenge submission](http://www.storytellingwithdata.com/blog/2018/1/22/88-annotated-line-graphs) (below).

![connected.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590502810070-7QSN01YEZ3B9CM01ZABC/connected.png)

![connected.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590502810070-7QSN01YEZ3B9CM01ZABC/connected.png?format=750w)

**2x2 grid (conceptual scatterplot):** This isn’t a multi-dimensional view per se, but one that can be practical in a business setting. We often want to understand relationships between two things or explain how one decision might impact another. A conceptual scatterplot also known as a 2x2 grid, can help your audience make sense of these comparisons, because our visual system is much faster at processing information than our verbal system. For example, we might use one to explain the differences between presenting your data live verse communicating via a written document. The two variables are the amount of control you want to have and the amount of detail needed to get your point across. Notice how quickly it is to grasp when one medium is ideal over the other.

![quadrant.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590503151969-SE0P3RPPYUKHV7105XCP/quadrant.png)

![quadrant.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590503151969-SE0P3RPPYUKHV7105XCP/quadrant.png?format=750w)

## **What are tips for designing scatterplots?**

Here are a few formatting steps to consider when designing scatterplots.

-   **Declutter by removing trendlines.** During the analytical process, you might fit a model to describe the relationship shown in your scatterplot and display this model as a line through the data points. My preference—and I realize this may be controversial—is to remove the fitted line when communicating data. It adds clutter and if the underlying trend isn’t obvious then implanting a line might lead to contention or confusion (as seen in [this hurricane example](http://www.storytellingwithdata.com/blog/2017/10/1/how-youd-visualize-hurricanes)). 
    

![TREND.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501705548-STHHPAX4RPZZ3L0KM6AV/TREND.png)

![TREND.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501705548-STHHPAX4RPZZ3L0KM6AV/TREND.png?format=750w)

-   **Make overlapping data points transparent.** If many data points overlap, it may become hard to see each value or the volume of points in a particular section. One trick might be to play with the opacity of the data markers so that the individual data points are visible.
    

![opacity.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501738110-R9T0L8PFZDU13I66RWUA/opacity.png)

![opacity.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501738110-R9T0L8PFZDU13I66RWUA/opacity.png?format=750w)

-   **You don’t need a zero baseline.** Similar to [line charts](http://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph), scatterplots encode data by position along the axis. This means that [it isn’t necessary for your baseline to start at zero](https://www.storytellingwithdata.com/blog/2014/02/a-little-math-on-non-zero-baselines) in the same way it is for [bars](https://www.storytellingwithdata.com/blog/2012/09/bar-charts-must-have-zero-baseline). With that said, you should still be mindful anytime you deviate from the zero baseline as this may introduce confusion.
    
-   **Create sections and add labels for clarity.** Adding annotations and categorizing data points can make scatterplots easier to consume. In the lip care example, notice how the pithy descriptions not only work well in constrained spaces but they also make this graph easier to discuss. I can refer to the opportunity quadrant and you likely know what I mean! Without implementing a clear construct to read the scatterplot, the graph is highly exploratory and requires the reader to repeat the analysis to uncover the relationship. Check out the difference in the image below or read these two posts for additional examples of how to label and categorize scatterplots: [an example showing reach and engagement by country](https://www.storytellingwithdata.com/blog/2018/1/15/our-tools-dont-know-the-story) and [another example showing manager performance](http://www.storytellingwithdata.com/blog/2015/04/the-power-of-categorization).
    

![construct.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501771020-PYX5YORQLBVPZO9PHVPQ/construct.png)

![construct.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1590501771020-PYX5YORQLBVPZO9PHVPQ/construct.png?format=750w)

## **Where can I see more scatterplot examples?**

For additional examples, check out our SWD challenge featuring [scatterplots](https://www.storytellingwithdata.com/blog/2018/10/23/scores-of-scatterplots).
