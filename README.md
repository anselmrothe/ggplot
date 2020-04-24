# Plotting your data with ggplot in R

## Getting started

Install R (about 1 minute): [download here](https://cloud.r-project.org/)

Install RStudio (about 1 minute): [download here](https://rstudio.com/products/rstudio/download/#download)

Install ggplot (about 1.5 minutes):
- open RStudio
- type into the console in RStudio: `install.packages('tidyverse')` and hit enter
- If it asks "Do you want to install from sources the packages which need compilation?" type `no` and hit enter

## Examples

### 1 Most simple example

```r
library(tidyverse)
x <- c(1, 2, 5, 1, 7, 3, 2, 4, 5, 7, 0, 3, 1)
y <- c(0, 4, 7, 4, 8, 2, 6, 3, 5, 4, 2, 7, 1)
df <- tibble(x, y) # ggplot needs data in data frame format
ggplot(df, aes(x, y)) + geom_point() # scatterplot
```
### 2 Commute data set example

See [here](http://htmlpreview.github.io/?https://github.com/anselmrothe/ggplot/blob/master/html/commute.html).
We will go through this example step by step.
It's going to be fun!

### 3 Full cycle example

*This example doesn't exist yet -- Getting the data into the right shape for plotting is a skill on its own, so this could become the content of for a future workshop.*

Full cycle:

1. Load data
2. Reshape data
3. Plot data

###

## Resources
(Subjective selection)

If I get stuck with a ggplot problem, I often just use google (for example "ggplot change order of colors"). Usually very efficient; leads you often to helpful answers on stackoverflow ([example](https://stackoverflow.com/questions/3777174/plotting-two-variables-as-lines-using-ggplot2-on-the-same-graph/)).

[ggplot cheat sheet](https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf)

[introduction to ggplot by the master himself](https://r4ds.had.co.nz/data-visualisation.html)

[another comprehensive introduction](https://r-graphics.org/index.html)

[examples with code (1)](http://www.sthda.com/english/wiki/be-awesome-in-ggplot2-a-practical-guide-to-be-highly-effective-r-software-and-data-visualization)

[examples with code (2)](https://datacarpentry.org/R-ecology-lesson/04-visualization-ggplot2.html)

[ggplot main page](https://ggplot2.tidyverse.org/)

[bad plots](https://www.biostat.wisc.edu/~kbroman/topten_worstgraphs/)


