
# package dplyr()

# package tidyr()
[tidyr Introduction](http://blog.rstudio.org/2014/07/22/introducing-tidyr/) (focus on the `gather()` function, that's what you want)

# extra

## Factors

### get rid of factors
`x <- as.character(x)`

### specify new factors
`x <- factor(x, levels = c("subject_rel_freq", "model_prob"), labels = c("Human", "Model"))`
