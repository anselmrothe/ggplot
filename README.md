# Plotting in R with ggplot

*This material is for my fellow PhD students who work with data every day but haven't made the big step to ggplot yet.*

## Getting started

### I haven't used R yet. How do I start?
To program in R, I like to work with [RStudio](https://www.rstudio.com/products/RStudio/).

### Ok, I installed RStudio. How can I use ggplot?
Install it by executing this line in RStudio (yes, it's actually ggplot2 we are talking about, the original ggplot is outdated):

`install.packages("ggplot2")`

You only need to install it once. But you need to activate it whenever you start a session with this:

`library(ggplot2)`

## Examples

### 1 Most simple example

```r
library(ggplot2)
x <- c(1, 2, 5, 1, 7, 3, 2, 4, 5, 7, 0, 3, 1)
y <- c(0, 4, 7, 4, 8, 2, 6, 3, 5, 4, 2, 7, 1)
df <- data.frame(x, y) # ggplot needs data in data frame format
ggplot(df, aes(x, y)) + geom_point() # scatterplot
```
### 2 Commute data set example

See [here](http://htmlpreview.github.io/?https://github.com/anselmrothe/ggplot/blob/master/html/commute.html).
We will go through this example step by step.
It's going to be fun!

### 3 Full cycle example

Full cycle:
1. Load data
2. Reshape data (see [additional page](2-reshape_data.md))
3. Plot data

[Full cycle example](http://htmlpreview.github.io/?https://github.com/anselmrothe/ggplot/blob/master/html/fullcycle.html)

### 

## Resources
(Subjective selection)

If I get stuck with a ggplot problem, I often just use google (for example "ggplot change order of colors"). Usually very efficient; leads you often to helpful answers on stackoverflow ([example](http://stackoverflow.com/questions/15251816/how-do-you-order-the-fill-colours-within-ggplot2-geom-bar)).

[ggplot cookbook](http://www.cookbook-r.com/Graphs/)

[ggplot docs](http://docs.ggplot2.org/current/)

[ggplot cheat sheet (long)](http://www.ceb-institute.org/bbs/wp-content/uploads/2011/09/handout_ggplot2.pdf)

[ggplot cheat sheet (short)](https://www.rstudio.com/wp-content/uploads/2015/03/ggplot2-cheatsheet.pdf)

[ggplot examples](http://www.di.fc.ul.pt/~jpn/r/GraphicalTools/ggplot2.html)

[ggplot examples 2](http://shiny.stat.ubc.ca/r-graph-catalog/)

### Advanced

[ggplot extensions](http://yutannihilation.github.io/allYourFigureAreBelongToUs)

## Live coding during the workshop

View here: https://www.getdatajoy.com/project/56390383649632dd2e9abbad
