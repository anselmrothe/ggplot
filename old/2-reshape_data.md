
# Package dplyr()
Awesome package to work with *data frames* in R.
In general, but especially if you use ggplot, you use data frames for your data.
I see two levels of expertise with dplyr, but before we start let me mention this thing: `%>%`
This is a special operater that makes it a lot easier to write and read your R code.

```r
## A note about the 'pipe' operator %>% from the dplyr package
library(dplyr)

# Usually you have function(argument1, argument2, ...)
x <- 1:5
mean(x)

# With the %>% operator, you have argument1 on the left and the function to the right
x %>% mean

# all later arguments are written as usual, it only works for the first argument
sum(x, 3, 4)
x %>% sum(3, 4)

# often you want the output of the first function to be the input of the next function
# now you can make long chains that are easy to read
sqrt(sum(mean(exp(x))))
x %>% exp %>% mean %>% sum %>% sqrt

# press cmd + shift + m
```

## dplyr beginner
*Assume `x` is a data frame with some rows and columns.*

### I want only columns A and B
`x %>% select(A, B)` (which is the same as `select(x, A, B)`)

### I want to drop columns G and H
`x %>% select(-G, -H)`

### I want only rows where values in column A are larger than 3
`x %>% filter(A > 3)`

`...`

## dplyr advanced

`...`

- `group_by`
- `summarize`
- `mutate`

[dplyr Introduction](https://cran.rstudio.com/web/packages/dplyr/vignettes/introduction.html) (advanced)

# Package tidyr()
[tidyr Introduction](http://blog.rstudio.org/2014/07/22/introducing-tidyr/) (focus on the `gather()` function, that's what you want)

# Other stuff

## Factors

### get rid of factors
`x <- as.character(x)`

### specify new factors
`x <- factor(x, levels = c("subject_rel_freq", "model_prob"), labels = c("Human", "Model"))`
