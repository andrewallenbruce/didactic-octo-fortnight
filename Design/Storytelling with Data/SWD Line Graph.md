---
created: 2021-09-18T22:16:06 (UTC -04:00)
tags: data, visualization
source: https://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph
author: Mike Cisneros
---

# what is a line graph, how does a line graph work, and what is the best way to use a line graph? — storytelling with data

> ## Excerpt
> Line graphs (or line charts) are best when you want to show how the value of something changes over time. In this post, we’ll talk about how a line graph works, plus: how to build one that provides meaningful information and context, what kind of data can be shown on a line graph, how many lines can

---
Line graphs (or line charts) are best when you want to show **how the value of something changes over time,** or compare how several things change over time relative to each other. Whenever you hear that key phrase “over time,” that’s your clue to consider using a line graph for your data.

Line graphs are common and effective charts because they are simple, easy to understand, and efficient. Line charts are great for:

-   **Comparing lots of data** all at once
    
-   Showing **changes and trends** over time
    
-   Including important **context and annotation**
    
-   Displaying **forecast data** and uncertainty
    
-   Highlighting **anomalies** within and across data series
    

On the other hand, they are _not_ necessarily your best choice for:

-   Displaying **quantities** of things
    
-   Working with **categorical** data
    
-   Making **part-to-whole** comparisons
    
-   Showing **sparse** data sets
    

In this post, we’ll talk about how a line graph works, and how to build one that provides meaningful information and context to your audience. 

Then, we’ll answer some commonly asked questions about line graphs:

-   [What kind of data can be shown on a line graph?](https://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph/#kind-of-data)
    
-   [How many lines can I show at one time?](https://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph/#how-many)
    
-   [Does my y-axis have to start at zero?](https://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph/#zero)
    
-   [How much space should I leave at the top and bottom of my graph?](https://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph/#space)
    

In future articles, we’ll go into more detail about some special variants of line graphs, like the slopegraph and the area graph.  
  

## How does a line graph work?

Think of the lines on a line graph as little histories. 

-   First, we **measure the value of something we want to keep track of at different points in time.** For example, at the end of every month, our store wants to record how much money we brought in through sales.
    
-   Once we have lots of these measurements, **we plot those points on our graph, and then draw a line that connects those points,** to make it easier to see how those values rose, fell, or stayed the same over time. 
    

![6-month-basic.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087222394-UFYYTA0J72NZFCEST28H/6-month-basic.png)

![6-month-basic.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087222394-UFYYTA0J72NZFCEST28H/6-month-basic.png?format=750w)

But that’s not all we can do with line graphs!

In addition to drawing that line, [we can include other important contextual information on our graph.](https://www.storytellingwithdata.com/blog/2014/10/annotated-line-graph-from-uber) We can choose to [**mark, label, and/or annotate** individual points on our line;](https://www.storytellingwithdata.com/blog/2017/8/2/axis-vs-data-labels) we can add **reference lines and regions;** we can even include forecast data points, and **distinguish between actual and projected data** by [changing the look of our line and our data markers](http://www.storytellingwithdata.com/blog/2018/5/8/when-to-use-a-dotted-line).   

Here’s what a chart like that could look like.

![example.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087261439-UQ6O0YAEJ1H8SA8HX7CN/example.png)

![example.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087261439-UQ6O0YAEJ1H8SA8HX7CN/example.png?format=750w)

  
Our collected sales data is still shown on the chart, as the solid black line, but now we’ve been able to put that data into context.

-   A gray reference band shows what the **range of monthly sales totals** have been, and we’ve **labeled those specific values** as well.
    
-   A green line shows us what our **sales goal** is, to make it easy to see if our sales numbers were worth celebrating in any given month.
    
-   To reduce some visual clutter, **the data labels and most of the markers of individual points on our line have been removed.** Only the markers for the months in which we hit our maximum and minimum sales values remain, because they are important to the story we plan to tell with this graph. 
    
-   A dotted line shows the **projected sales** over the next three months.
    
-   **Annotations** at key moments in time explain the reasoning for the numbers, actions we took in response to those numbers, and our expectations.
    

Remember: line graphs work by emphasizing how our measured values change over time, or as a specified independent variable changes. We can take advantage of the white space in our line graphs to include informative context that helps an audience understand why these specific changes matter.

## What kind of data can be used on a line graph?

A typical line graph will have **continuous data** along both the vertical (y-axis) and horizontal (x-axis) dimensions. The y-axis usually shows the **value of whatever variable we are measuring;** the x-axis is most often used to show **when we measured it,** either **chronologically** or based on some **independent variable** (e.g., as we rev our old car’s engine, we measure the decibel level at different RPM)**.** 

While some line graphs do not use continuous data on the x-axis (particularly [slopegraphs](https://www.storytellingwithdata.com/blog/2014/03/more-on-slopegraphs) and [parallel coordinates](https://www.storytellingwithdata.com/blog/2018/2/19/connecting-the-dots) diagrams, which are specialized variants of line graphs), what we absolutely _can’t_ use on our x-axis is data that doesn’t have any meaningful relationship among the categories shown. 

Let’s say we have a **list of the first six months of 2020:** January, February, March, April, May, June. It would feel wrong to list them in any other order, because they are continuous and have an intrinsic order. January 2020 leads to February 2020, which leads to March 2020, and so on.

Let’s also say we have a **list of types of produce:** apples, pears, limes, lemons, dates, grapes. Unlike our list of months, one kind of produce doesn’t necessarily lead to the next. We could order them alphabetically, by size, by color, or randomly, and it wouldn’t feel unusual, because they have no intrinsic order, and are not continuous—they are categorical. 

 ![DO: Show a line of sales by month.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087896250-R3GZ6OFWYQRZUJRCJU3D/produce_monthly.png)

![DO: Show a line of sales by month.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087896250-R3GZ6OFWYQRZUJRCJU3D/produce_monthly.png?format=500w) 

DO: Show a line of sales by month.

 ![DON’T: Show a line of sales by category.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087907450-P1KFP117MZ482U21XP75/produce_categoricall.png)

![DON’T: Show a line of sales by category.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585087907450-P1KFP117MZ482U21XP75/produce_categoricall.png?format=500w) 

DON’T: Show a line of sales by category.

#block-yui\_3\_17\_2\_1\_1585086671526\_56564 .sqs-gallery-block-grid .sqs-gallery-design-grid { margin-right: -10px; } #block-yui\_3\_17\_2\_1\_1585086671526\_56564 .sqs-gallery-block-grid .sqs-gallery-design-grid-slide .margin-wrapper { margin-right: 10px; margin-bottom: 10px; }

**Line graphs only make sense when there is a meaningful relationship between successive points on the line.** Therefore, a grocery store could reasonably use a line graph to show their produce sales data by month, but using one to show sales differences among various types of produce isn’t recommended. [That would be better done in a bar chart.](http://www.storytellingwithdata.com/blog/2020/2/19/what-is-a-bar-chart)

## How many different lines can I put in one chart?

People have a hard time keeping track of more than **four or five things** simultaneously, so consider using that as your guideline. If you absolutely need to show more lines than that, try to use color, line weight, and labeling to focus on the most important lines or points.

![step5-averagewspaghetti.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088085655-8YT28QCZDVT0IM6C2AJ3/step5-averagewspaghetti.png)

![step5-averagewspaghetti.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088085655-8YT28QCZDVT0IM6C2AJ3/step5-averagewspaghetti.png?format=750w)

This graph above shows five years’ worth of data for annual diabetes rates of patients at our local medical center, Anytown Medical, as well as the rates for 12 other centers in our region. Since what we are likely to care about the most is our own center (particularly because our rates are low), we are using color, weight, and labeling to bring focus to Anytown and to the regional average, while also including the values for all other centers.

## Does the y-axis of a line graph have to start at zero?

When we look at line graphs, [we compare the lines to each other more than their height from the x-axis](https://www.storytellingwithdata.com/blog/2012/09/bar-charts-must-have-zero-baseline). By their nature, line graphs are better at showing the change of values over time than an exact quantity at each measured point. 

[Line graphs, therefore, are **not required to have a zero baseline;** but in most cases, **it is still advisable.**](https://www.storytellingwithdata.com/blog/2014/02/a-little-math-on-non-zero-baselines) It is less confusing to an audience if the y-axis starts at zero, since that is the normal expectation when seeing a chart for the first time. There should be compelling reasons to subvert those expectations.

Here are some specific cases for which **a zero baseline might not be optimal:**

### **The range of measurements is small, but the distance from the minimum value of those measurements to zero is large.** 

If our y-axis went all the way down to zero, these meaningful fluctuations would be impossible to perceive.

 ![DO: Start the axis at a logical value.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088328568-N71DZL4VV1CANX2G63EI/dailyvalgood.png)

![DO: Start the axis at a logical value.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088328568-N71DZL4VV1CANX2G63EI/dailyvalgood.png?format=500w) 

DO: Start the axis at a logical value.

 ![DON’T: Include zero if that obscures the data.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088328529-P5YFXGY8SITFZF1HAI7N/dailyvalbad.png)

![DON’T: Include zero if that obscures the data.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088328529-P5YFXGY8SITFZF1HAI7N/dailyvalbad.png?format=500w) 

DON’T: Include zero if that obscures the data.

#block-yui\_3\_17\_2\_1\_1585087989912\_20296 .sqs-gallery-block-grid .sqs-gallery-design-grid { margin-right: -10px; } #block-yui\_3\_17\_2\_1\_1585087989912\_20296 .sqs-gallery-block-grid .sqs-gallery-design-grid-slide .margin-wrapper { margin-right: 10px; margin-bottom: 10px; }

### **The relationship to zero is not meaningful.**

On some scales, like on a Fahrenheit scale, the position of “zero” is somewhat arbitrary (50 degrees isn’t twice as warm as 25 degrees), so if no data point would ever come close to zero, we shouldn’t feel obliged to include that as our baseline. Our graphs should include a range of reasonable values, providing the most meaningful context to a viewer.

 ![DO: Use a reasonable range of values.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088536506-8EH2VI07GYB0Q6SP7H4S/bodytemp.png)

![DO: Use a reasonable range of values.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088536506-8EH2VI07GYB0Q6SP7H4S/bodytemp.png?format=500w) 

DO: Use a reasonable range of values.

 ![DON'T: Include zero if it's a meaningless value.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088519478-J5BSL8UHO4E3XZ44CS72/bodytempbad.png)

![DON'T: Include zero if it's a meaningless value.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088519478-J5BSL8UHO4E3XZ44CS72/bodytempbad.png?format=500w) 

DON'T: Include zero if it's a meaningless value.

#block-yui\_3\_17\_2\_1\_1585087989912\_26074 .sqs-gallery-block-grid .sqs-gallery-design-grid { margin-right: -10px; } #block-yui\_3\_17\_2\_1\_1585087989912\_26074 .sqs-gallery-block-grid .sqs-gallery-design-grid-slide .margin-wrapper { margin-right: 10px; margin-bottom: 10px; }

### **Some of your measurements are negative.**

It might be important to include a horizontal line as a reference point for zero, but no data series on our graphs should cut across either of our axes. It’s preferable to make the minimum value of our y-axis lower than the minimum measured value of our data, so that our baseline is a boundary line for our data.

 ![DO: Keep the axis below the minimum data.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088685747-ISCJ9I9EKEDO352OLR35/negatives-good.png)

![DO: Keep the axis below the minimum data.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088685747-ISCJ9I9EKEDO352OLR35/negatives-good.png?format=500w) 

DO: Keep the axis below the minimum data.

 ![DON’T: Let the axis cut through the data.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088685751-3QM5I6598VBOD77K5C8N/negatives-bad.png)

![DON’T: Let the axis cut through the data.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1585088685751-3QM5I6598VBOD77K5C8N/negatives-bad.png?format=500w) 

DON’T: Let the axis cut through the data.

#block-yui\_3\_17\_2\_1\_1585087989912\_30593 .sqs-gallery-block-grid .sqs-gallery-design-grid { margin-right: -10px; } #block-yui\_3\_17\_2\_1\_1585087989912\_30593 .sqs-gallery-block-grid .sqs-gallery-design-grid-slide .margin-wrapper { margin-right: 10px; margin-bottom: 10px; }

**IMPORTANT!** In situations where your line graph has a non-zero baseline, it’s important to make that fact obvious to your viewer, so they are not misled by a zoomed-in perspective on your data.

## How much space should I leave at the top and bottom of my graph?

The specific answer to this question will vary with each graph you make. A useful starting point is to make **the range from your smallest value to your largest value take up about 70-80% of your graph’s available vertical space,** with a roughly equal amount of white space above and below it. 

From there, you can modify your axis range, and the position of the line or lines plotted on the graph, to suit your specific needs. The relative slopes of your lines won’t change, so do your best to select an axis range that lets you have round numbers for your axis labels, a reasonable amount of white space in the chart to include data labels and annotations, and is wide enough (if necessary) to show reference lines, like goals or projected values, that might be bigger or smaller than your smallest or largest measured value.

In every case, it’s important to be reasonable and thoughtful in how you present the data, in order for your audience to understand your message clearly.
