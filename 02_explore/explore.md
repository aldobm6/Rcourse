Explore
========================================================
author: Wim van der Ham
date: 29/1/2018
autosize: true

Explore - Work Flow
========================================================

![Explore Work Flow](./explore_workflow.jpg)

ggplot2
========================================================

- ggplot()
- [geom_*](http://ggplot2.tidyverse.org/reference/index.html#section-layer-geoms)
- aes()

Examples in the `explore.R` file

Labels
========================================================

**Always** label your axis and use a title

Title should be a conclusion, not a description

Best Type of Graphics
========================================================

| Type of variable 1 | Type of variable 2 | Best Graphic |
| --- | --- | --- |
| Discrete | Discrete | geom_bar |
| Discrete | Continuous | geom_boxplot |
| Continuous | Continuous | geom_point* |

* When there is too much data, one of the variables has to be changed to discrete using `cut()`.

Pipe %>%
========================================================


```r
sin(sqrt(log(10)))
```

```
[1] 0.9985762
```


```r
library(tidyverse)
10 %>%
  log %>%
  sqrt %>%
  sin
```

```
[1] 0.9985762
```

dplyr - Most important functions
========================================================

| function | description | SQL |
| --- | --- | --- | --- |
| `select()` | Select specific columns | SELECT
| `filter()` | Filter rows dependend on a condition | WHERE
| `group_by()` | Make groups | GROUP BY
| `arrange()` | Sort | ORDER BY
| `summarise()` | Calculate some values per group |
| `mutate()` | Add a new column using a function |

dplyr - Examples
========================================================

Examples in the `explore.R` file