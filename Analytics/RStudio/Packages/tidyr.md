---
tags: rstudio/packages, tidyr, cleaning
author:
alias:
related:
---

# tidyr

## Reference
[Tidy data • tidyr](https://tidyr.tidyverse.org/articles/tidy-data.html)
[Function reference • tidyr](https://tidyr.tidyverse.org/reference/index.html)

## Overview

The goal of tidyr is to help you create **tidy data**. Tidy data is data where:

1.  Every column is variable.
2.  Every row is an observation.
3.  Every cell is a single value.

Tidy data describes a standard way of storing data that is used wherever possible throughout the [tidyverse](https://www.tidyverse.org/). If you ensure that your data is tidy, you’ll spend less time fighting with the tools and more time working on your analysis. Learn more about tidy data in `[vignette("tidy-data")](https://tidyr.tidyverse.org/articles/tidy-data.html)`.

## Installation

```
# The easiest way to get tidyr is to install the whole tidyverse:
install.packages("tidyverse")

# Alternatively, install just tidyr:
install.packages("tidyr")

# Or the development version from GitHub:
# install.packages("devtools")
devtools::install_github("tidyverse/tidyr")
```

## Cheatsheet
![[tidyr_data_cleaning.pdf]]

## Getting started

```
library(tidyr)
```

### tidyr functions fall into five main categories:
1. “Pivotting” which converts between long and wide forms. tidyr 1.0.0 introduces [`pivot_longer()`](https://tidyr.tidyverse.org/reference/pivot_longer.html) and [`pivot_wider()`](https://tidyr.tidyverse.org/reference/pivot_wider.html), replacing the older [`spread()`](https://tidyr.tidyverse.org/reference/spread.html) and [`gather()`](https://tidyr.tidyverse.org/reference/gather.html) functions. See [`vignette("pivot")`](https://tidyr.tidyverse.org/articles/pivot.html) for more details.
2. “Rectangling”, which turns deeply nested lists (as from JSON) into tidy tibbles. See [`unnest_longer()`](https://tidyr.tidyverse.org/reference/hoist.html), [`unnest_wider()`](https://tidyr.tidyverse.org/reference/hoist.html), [`hoist()`](https://tidyr.tidyverse.org/reference/hoist.html), and [`vignette("rectangle")`](https://tidyr.tidyverse.org/articles/rectangle.html) for more details.
3. Nesting converts grouped data to a form where each group becomes a single row containing a nested data frame, and unnesting does the opposite. See [`nest()`](https://tidyr.tidyverse.org/reference/nest.html), [`unnest()`](https://tidyr.tidyverse.org/reference/nest.html), and [`vignette("nest"`)](https://tidyr.tidyverse.org/articles/nest.html) for more details.
4. Splitting and combining character columns. Use [`separate()`](https://tidyr.tidyverse.org/reference/separate.html) and [`extract()`](https://tidyr.tidyverse.org/reference/extract.html) to pull a single character column into multiple columns; use [`unite()`](https://tidyr.tidyverse.org/reference/unite.html) to combine multiple columns into a single character column.
5. Make implicit missing values explicit with [`complete()`](https://tidyr.tidyverse.org/reference/complete.html); make explicit missing values implicit with [`drop_na()`](https://tidyr.tidyverse.org/reference/drop_na.html); replace missing values with next/previous value with [`fill()`](https://tidyr.tidyverse.org/reference/fill.html), or a known value with [`replace_na()`](https://tidyr.tidyverse.org/reference/replace_na.html).
    
## Related work
tidyr [supersedes](https://lifecycle.r-lib.org/articles/stages.html#superseded) reshape2 (2010-2014) and reshape (2005-2010). Somewhat counterintuitively, each iteration of the package has done less. tidyr is designed specifically for tidying data, not general reshaping (reshape2), or the general aggregation (reshape).

[data.table](https://rdatatable.gitlab.io/data.table) provides high-performance implementations of `melt()` and `dcast()`

If you’d like to read more about data reshaping from a CS perspective, I’d recommend the following three papers:

-   [Wrangler: Interactive visual specification of data transformation scripts](http://vis.stanford.edu/papers/wrangler)
    
-   [An interactive framework for data cleaning](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2000/CSD-00-1110.pdf) (Potter’s wheel)
    
-   [On efficiently implementing SchemaSQL on a SQL database system](https://www.vldb.org/conf/1999/P45.pdf)
    

To guide your reading, here’s a translation between the terminology used in different places:

| tidyr 1.0.0   | pivot longer | pivot wider |
| ------------- | ------------ | ----------- |
| tidyr < 1.0.0 | gather       | spread      |
| reshape(2)    | melt         | cast        |
| spreadsheets  | unpivot      | pivot       |
| databases     | fold         | unfold      |

