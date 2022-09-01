---
created: 2021-09-18T22:21:16 (UTC -04:00)
tags: []
source: https://www.storytellingwithdata.com/blog/2020/5/14/what-is-a-pie-chart
author: by Elizabeth Ricks
---

# What is a pie chart and when to use it — storytelling with data

> ## Excerpt
> In this article we discuss pie charts, what they are, how and when to use them. We also share pie chart design tips and examples.

---
Pie charts are one of the most common types of data visualizations. They are also one of the most widely condemned and misused. The good news is they do have a proper use case and it’s easy to use them appropriately. 

In this post, we’ll discuss:

-   how a pie chart works 
    
-   two specific use cases for a pie
    
-   how to identify whether your data is better served as something _other_ than a pie 
    
-   design tips for creating an effective pie  
    

##   
What is a pie chart? 

A pie chart expresses a part-to-whole relationship in your data. Imagine an actual pie (I’ll let you choose your favorite variety!). Each slice represents one component and all slices added together equal the whole. Pies are perhaps so commonly used because, as Manuel Lima writes about in [The Book of Circles](https://www.amazon.com/gp/product/1616895284/ref=as_li_qf_asin_il_tl?ie=UTF8&tag=storytellingwithdata-20&creative=9325&linkCode=as2&creativeASIN=1616895284&linkId=32d9b45340a42e09f09b8e28f7b11584), humans gravitate to circles as the universal symbol of unity, perfection, and infinity. We like things to be whole—and understand how the respective pieces relate to the whole. A pie chart provides us this comfort of a part-to-whole relationship. 

Here’s a brief overview of how we consume a pie. Each pie slice has three visual components: its central angle, area, and arc length. Recent research by Robert Kosara and Drew Skau demonstrated that we read pie charts by area—or possibly in combination with arc length—which debunked some previously held beliefs that pies are read by angle. You can read more about their research in [an illustrated tour of the pie chart study results](https://eagereyes.org/blog/2016/an-illustrated-tour-of-the-pie-chart-study-results).  

Let’s look at an example. Imagine you have a portfolio of five products and you measure sales (in millions of dollars) for each. The sum of each individual product’s sales equals the total sales amount. You can see the part-to-whole relationship of each product’s contribution to the total in the pie below. In this instance, I put the total dollar volume at the top and labeled each segment with the percent of the total. Alternatively, I could have labeled each segment with the respective dollar amount. Which you choose is largely dependent on what you want your audience to see or do with the graph. 

![2_sales by product.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459527969-AMZ4OHKJ5ES2GLYKK9WV/2_sales+by+product.png)

![2_sales by product.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459527969-AMZ4OHKJ5ES2GLYKK9WV/2_sales+by+product.png?format=500w)

##   
When should I use a pie chart?

Pie charts are probably better than any other visual for expressing a part-to-whole relationship. When you hear “percent of…” or “part of…” that’s one indication a pie chart could meet your needs.

There are **two** **primary use cases for a pie chart:**

1.  If you want your audience to have a **general sense of the part-to-whole relationship in your data** and comparing the precise sizes of the slices is less important.
    
2.  To convey that one segment of the total is relatively **small** or **large.**
    

Our sales example supports the first use case. Suppose we want to focus on how much revenue a given product—or set of products—contributes to the total. Given our natural construct of how we read a clock, it’s fairly easy to tell that Product A makes up roughly a quarter of total revenue and that Products A, B, and C combined are roughly two-thirds of total revenue. For these general part-to-whole relationships, a pie chart could effectively convey that information.

The two pie charts below are examples of the second use case. With each of these, I can easily make one broad conclusion—one slice of the pie is relatively larger or smaller than the others.

![3_small and large.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459724938-6X8CLQN15A1LLB0IFAHD/3_small+and+large.png)

![3_small and large.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459724938-6X8CLQN15A1LLB0IFAHD/3_small+and+large.png?format=500w)

For applications with different datasets, check out Lisa Charlotte Rost’s examples in [what to consider when creating pie charts.](https://academy.datawrapper.de/article/127-what-to-consider-when-creating-a-pie-chart)

##   
When should I pass on the pie?

Generally speaking, pies should _not_ be used for evaluating the relative sizes of categories, comparing data across pies, and visualizing percentages that do not sum to 100%. Let’s look at an example of each.

**Comparing the size of categories**: Pie charts break down pretty quickly if we need our audience to have a more nuanced understanding of our data than simply big, small, or about the same. To illustrate, consider the following example. If I asked you to compare the size of slices C and D, which would you conclude is larger? Taking it a step further, how easily can you estimate how much bigger?

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459851502-IY52C2I5I5AFSE0TOIBI/image-asset.png)

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459851502-IY52C2I5I5AFSE0TOIBI/image-asset.png?format=500w)

This example demonstrates one limitation of data encoded as pie slices: humans’ eyes aren’t well-equipped to compare areas. The challenge becomes even more pronounced without a consistent baseline—like a y-axis in a horizontal bar chart—against which to make the visual comparison. As illustrated in the following, comparing the size of C vs D is much easier in the graph on the right. We’re also comparing one dimension (length) across two categories, instead of irregularly-shaped areas.

![5_hard and easy.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459918531-6CBO07VAGXW68OU76Y5P/5_hard+and+easy.png)

![5_hard and easy.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589459918531-6CBO07VAGXW68OU76Y5P/5_hard+and+easy.png?format=500w)

**Comparing data across pies:** this is a difficult task the things you aim to compare are separated visually and are located in different places on each pie. To illustrate, check out the pair of pies below, excerpted from Exercise 2.1 of [_Storytelling with Data: Let’s Practice!_](http://www.storytellingwithdata.com/books)

![6_new client tier share.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460011901-VEN102YQ0TP1IWWEKP26/6_new+client+tier+share.png)

![6_new client tier share.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460011901-VEN102YQ0TP1IWWEKP26/6_new+client+tier+share.png?format=500w)

Let’s say the primary comparison you want to highlight is how Tier B varies across the two breakdowns. Tier B is in different places across the pies—as a direct result of the variation between the two datasets. Because of this spatial separation, different positioning within the pie, and the irregular shapes of the segments, it’s hard to accurately judge the difference in magnitude. 

**Showing data that doesn’t sum to 100%:** if the slices sum to something other than 100%, it is wrong. By definition, the pie must depict a meaningful whole. 

![7_this does not make sense.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460085623-NMOIQDSGZV4PIPQZGIZ9/7_this+does+not+make+sense.png)

![7_this does not make sense.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460085623-NMOIQDSGZV4PIPQZGIZ9/7_this+does+not+make+sense.png?format=300w)

##   
I want to use a pie: how do I make a good one?

When using pie charts, here are a few quick design tips to make them more effective.  
  
**Avoid 3D and exploding effects.** These elements introduce unnecessary clutter and can distort the data. This inability to make an accurate visual comparison was validated in the aforementioned Kosara and Skau study, where study participants misjudged the values in exploding pie charts to a higher degree than the flat pie. 

![8_avoid 3d.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460194821-G09GL88P5BNC5LOHR5QB/8_avoid+3d.png)

![8_avoid 3d.png](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460194821-G09GL88P5BNC5LOHR5QB/8_avoid+3d.png?format=500w)

**Don’t have a ton of slices.** There isn’t an exact rule here, so approach with careful consideration towards your dataset and audience’s needs. You can improve readability by either de-emphasizing small categories with similarity of color (as shown in the following middle pie with grey) or by aggregating into an “All other” category, as illustrated on the right.

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460522164-URGI13X9NQ5BE6UF1D94/image-asset.png)

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460522164-URGI13X9NQ5BE6UF1D94/image-asset.png?format=750w)

**Sort your data meaningfully.** Check out the two pies below. On the left, the data is sorted alphabetically (beginning with apples at zero degrees). The right pie is sorted in descending order starting with the largest category (pineapple). This takes into account our natural construct of reading around a circle. 

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460586742-FGF3ERP8UGOD5OYLCYUX/image-asset.png)

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460586742-FGF3ERP8UGOD5OYLCYUX/image-asset.png?format=500w)

**  
Eliminate the legend and label the data directly**. Check out the difference in the following graphs. Labeling directly, as shown on the right, reduces the task of going back and forth between the legend and the data. Whenever possible, aim to label your slices directly with the value so long as there’s sufficient space to make the labels legible. 

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460651255-CUIX1YHERQSZZL633JQT/image-asset.png)

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460651255-CUIX1YHERQSZZL633JQT/image-asset.png?format=500w)

**  
Use color strategically.** When used sparingly, color is arguably the most important decision we make to focus our audience’s attention. Let’s assume we’d like to highlight Product A’s contribution to our sales portfolio. Which of the following pies more effectively draws your attention to Product A? 

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460715852-HXP8B7PMPN5CO9KBDHH4/image-asset.png)

![](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1589460715852-HXP8B7PMPN5CO9KBDHH4/image-asset.png?format=500w)

For another example of effectively designing a pie, check out [how to make a better pie chart](http://www.storytellingwithdata.com/blog/2020/2/26/how-to-make-a-better-pie-chart).  

##   
Where can I learn more about pie charts?

Here are some related resources to further your learning: 

-   **Practice** with the exercises [which graph would you choose?](https://community.storytellingwithdata.com/exercises/which-graph-would-you-choose) or [alternatives to pies](https://community.storytellingwithdata.com/exercises/alternatives-to-pies)
    
-   **Listen** to the podcast episode [it depends…](https://www.storytellingwithdata.com/blog/2018/2/6/it-depends)
    
-   **Discuss** in the community conversation [alternative part-to-whole approaches](https://community.storytellingwithdata.com/conversations/c2ce7f84-f2ed-4354-b947-7818c7b06afa)
    
-   **Read** the ongoing discussion and debate about the use cases for pies:
    
    -   [Alternatives to pies](https://www.storytellingwithdata.com/blog/2014/06/alternatives-to-pies) (SWD)
        
    -   [The great pie debate](http://www.storytellingwithdata.com/blog/2015/03/the-great-pie-debate) (SWD)
        
    -   [An updated post on pies](http://www.storytellingwithdata.com/blog/2017/1/10/an-updated-post-on-pies) (SWD)
        
    -   [Who made that pie chart?](https://www.nytimes.com/2012/04/22/magazine/who-made-that-pie-chart.html?_r=1) (New York Times)
        
    -   [Save the pies for dessert](https://www.perceptualedge.com/articles/visual_business_intelligence/save_the_pies_for_dessert.pdf) (Stephen Few)
        
    -   [F\*\*k it, let’s use pies](https://policyviz.com/2018/01/11/fk-it-lets-use-pie-charts/) (Jon Schwabish)
