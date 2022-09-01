---
created: 2021-09-18T22:24:17 (UTC -04:00)
tags: []
source: https://www.storytellingwithdata.com/blog/2020/9/24/what-is-a-table
author: by Alex Velez
---

# what is a table? — storytelling with data

> ## Excerpt
> In this article, we will discuss tables—what are they and how we process them. We'll share when to use a table to communicate data—or when not use them—along with useful design tips and examples.

---
### What is a table?

A table organizes data into a tabular structure, consisting of rows and columns. They are intuitive to read, reasonably easy to build, and they are incredibly flexible. Unlike some of the previous charts we’ve discussed—[bars](http://www.storytellingwithdata.com/blog/2020/2/19/what-is-a-bar-chart), [pies](http://www.storytellingwithdata.com/blog/2020/5/14/what-is-a-pie-chart), [lines](http://www.storytellingwithdata.com/blog/2020/3/24/what-is-a-line-graph), [etc](http://www.storytellingwithdata.com/chart-guide).—tables are not constrained to a specific type of data or underlying relationship. They might contain numerical values, text, symbols, or even a combination of data types. For these reasons, tables are common and favored by many. 

While seemingly simple on the surface, tables are more complex than they appear. It’s easy to think they are interchangeable with other basic visuals like bars and lines, but there is an important distinction to understand: **we process tables differently from graphs**. Tables interact with our verbal communication system, meaning we read them. Our eyes scan across rows and down columns. In comparison, graphs interact with our visual system. Our [visual system is much faster at processing large quantities of information](https://visualthinking.psych.northwestern.edu/publications/ZacksDecisionMakers2020.pdf), especially when there is a pattern or shape we want to convey. Understanding this up front helps us realize when it’s appropriate to use a table, or said another way when our audiences should read the data rather than decode a visual.

### When should you use a table to communicate data?

Let’s explore a handful of business scenarios where it makes sense to use a table.

-   **You have varied data.** Sometimes we need to communicate related metrics with multiple units of measure or varying ranges. Executive summaries, scorecards, demographic breakdowns and metadata are things that come to mind. In this case, the end-user will likely reference these items to look up specific values, so a table is an effective choice. Also, tables aren’t subject to the same two-dimensional space constraints as graphs, so it can be easier to display different units and ranges within a single view.
    
-   **Your audience has different needs.** Tables can be great when you have a diverse audience. I’ve already mentioned that tables are intuitive, but they also enable each end-user to look up specific values. If you anticipate your audience will want to scan for different data, tables can be a nice solution. 
    
-   **You’re reading line by line.** Discussing numbers and budget line items within a table are common among finance or accounting audiences. A former director of mine had an accounting background, and as a result, developed an affinity for tables. He learned how to spot patterns within tables so well that he requested data tables over graphs. I bring this up for a good reason—**if your audience has a strong desire for tables, recognize that this is another excellent reason to use them.**
    
-   **You’re supplementing the main story.** When communicating data for explanatory purposes, we rarely show all of the data, instead opting to highlight the main takeaways. There can be value in providing audiences with the complete dataset or additional breakdowns, especially if your audience will want to look up details at a later time or explore the data independently. To meet this need, consider linking to an underlying table or adding a detailed table to an appendix.
    

### When _shouldn’t_ you use a table to communicate data?

There will always be exceptions, but two main instances come to mind when it may _not_ be ideal to use a table. Both of these scenarios relate to how we process tables.

1.  **You are presenting your data live—in person or virtually.** If you share a data table in a live presentation, your audience is likely going to start reading it. Unfortunately, we cannot actively listen and read simultaneously: if your audience is reading the table, they’ve tuned you out. In this situation, I’d recommend a graph (generally, less taxing and time-consuming to process) over a table. If you are required to use a table during a presentation, consider how your audience will interpret it. Can you pause, giving them time to read, and then continue talking? Is there a way to limit unnecessary rows and columns or direct attention to a subset of the data, making the table faster to digest?
    
2.  **You want to emphasize a pattern or shape in the data.** Imagine you want to share a seasonal pattern you’ve identified within some continuous monthly data. To spot this in a table, you’d have to compare and hold several monthly values in your head, which is a mentally taxing process. If there is a pattern or something significant about the shape of your data, a graph will be a better choice over a table. That said, it’s possible to add visual components to a table—will explore this further momentarily.
    

### How can you design a _better_ table?

Nearly every tip shared below has to do with making tables easier to scan. Tables typically contain large amounts of detail, so **we should take intentional steps to make them easy to consume.**   
**Clarify horizontal or vertical.** Tables are consumed either across rows or down columns. Prevent your audience from assuming which way to scan by adding visuals cues. There are several ways of doing this; two of my preferred methods are to add a summary series and leverage white space. If I anticipate my audience will want to summarize the data in a total or average, then adding a summary series—_and_ visually differentiating it—can save them a step and guide them when reading.

![Side-by-side comparison of how to format a data table.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913349630-3HRDA6ZXZTZLKMKU2656/Data+table+formatting.png)

![Side-by-side comparison of how to format a data table.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913349630-3HRDA6ZXZTZLKMKU2656/Data+table+formatting.png?format=1000w)

**Remove unnecessary borders and shading.** Many table defaults include heavy borders and shading. These can help separate headers from the data or establish categories and summary values, but their presence should be minimal. My preference is to use border lines over shading since it allows me to then use color more strategically—as in a heatmap (more on this next).

![Format a table using minimal borders and shading.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913381606-FWSUX54S31EA4WC0Q3SD/Data+table+borders.png)

![Format a table using minimal borders and shading.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913381606-FWSUX54S31EA4WC0Q3SD/Data+table+borders.png?format=1000w)

**Incorporate a visual element.** Consider adding visual elements to help draw attention to the most important data or to communicate a pattern. You could add color, sparklines, or even data bars. One specialized case is known as a heatmap, where saturation of color is used to visually represent relative values. See the related posts on [improving a table](http://www.storytellingwithdata.com/blog/2019/10/29/how-i-improved-the-table), [embedding horizontal bars](http://www.storytellingwithdata.com/blog/2012/02/grables-and-taphs), and [a heatmap makeover](http://www.storytellingwithdata.com/blog/2020/10/15/a-heatmap-makeover) for specific examples.

![Add visual elements in a data table like heatmapping and embedded bars.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913250613-7WM7EQEO7VV8WHMX2L79/Grapple+a+visual+table.png)

![Add visual elements in a data table like heatmapping and embedded bars.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913250613-7WM7EQEO7VV8WHMX2L79/Grapple+a+visual+table.png?format=750w)

**Order intentionally.** When we process a page, we typically start at the top and move from left to right, in a zig-zag pattern down the page. This is also true for a table and can help us decide how to order rows and columns. If there is an important metric or summary value, it may make sense to move this to the upper left of the table—so it’s one of the first things your audience sees. Keep in mind that this won’t be appropriate in all scenarios. If your table includes a time component, for example, consider leveraging the natural construct of time moving from left to right—even if recent data is most important.

**Use super-category labels.** Creating higher-level labels adds structure to a table, making it easier to navigate. Super-category labels also have the added benefit of limiting redundancy (check out this related post on [the power of categorization](http://www.storytellingwithdata.com/blog/2015/04/the-power-of-categorization)). Consider the case of an executive summary table containing KPIs for a handful of business units. Instead of listing each KPI separately, group related KPIs together, so someone can quickly identify all related measures for a specific department.

**Align thoughtfully.** A number of approaches exist for how to justify data within a table. One popular preference is to left-align text and right-justify numbers. This is a great guideline, but not a rule. Instead, aim to be thoughtful about the alignment you use. Does center alignment allow for white space to visually distinguish columns? If using decimals, is it easier to compare relative values if you align decimals points? Play with different options and see which works best for your data. (On a related note, certain typefaces allow for tabular alignment creating columns of numbers; to learn more, read Matthew Ström’s article on [designing better tables](https://medium.com/mission-log/design-better-data-tables-430a30a00d8c).)

![Sample column alignments in a data table: mixed, centered and decimal alignment.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913310652-WZOSLFP5DZ5D83K4D19I/Data+table+alignments.png)

![Sample column alignments in a data table: mixed, centered and decimal alignment.](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1600913310652-WZOSLFP5DZ5D83K4D19I/Data+table+alignments.png?format=750w)

When a table is designed well, its form enables useful function. The organized, tabular structure fades to the background, allowing audiences to quickly find pertinent details.
