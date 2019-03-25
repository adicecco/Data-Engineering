---
title: "SampleExercise"
author: "Anthony DiCecco"
date: "March 23, 2019"
output: html_document
---

### Sample Exercise
# ML Pipelines with sparklyr {#anchor}

### Exercise
#### Baisc pipeline for a linear regression
Now that the data flow is documented with a diagram, we'll set up a simple pipeline for the data to pass through. The data flow will use dplyr functions `select()` and `mutate()` to create a blank pipeline that the data will flow through. Then we'll use this pipeline to pass the data through. Finally, we'll summarize the model to look at fit. 

### Instructions
The longley dataet is ready to be used and `dplyr` is already loaded to the R session.
   * Create an empty pipeline saved as `pipeline`
     * Select only the columns needed for the analysis: GNP, Unemployed, Employed, Population and Armed.Forces.
     * Create two new features, pcnt_unemployed as the ratio of Unemployed and Population and pcnt_af as the ratio of Armed.Forces and Population.
     * Fill in the linear model to use Employed, pcnt_unemployed, and pcnt_af to predict GNP
   * Pass the longley dataset through the pipeline and save as lm_model
   * View the summary of the saved lm_model
   
### Sample Exercise
```{r}
# longley is already available in the workspace

# create an empty pipeline using select and mutate to pass data to a linear model
pipeline <- . %>% select(___) %>% 
  # mutate data to create two new features pcnt_unemployed and pcnt_af
  mutate(pcnt_unemployed = ___, pcnt_af = ___) %>%
  # set up a linear model to pass new features to predict GNP
  lm(GNP ~ ___, data = .)

# pass the data through the pipeline and save as lm_model


# view the summary of the lm_model

```

### Sample Solution
```{r}
# longley is already available in the workspace

# create an empty pipeline using select and mutate to pass data to a linear model
pipeline <- . %>% select(GNP, Unemployed, Employed, Population, Armed.Forces) %>% 
  # mutate data to create two new features pcnt_unemployed and pcnt_af
  mutate(pcnt_unemployed = Unemployed/Population, pcnt_af = Armed.Forces/Population) %>%
  # set up a linear model to pass new features to predict GNP
  lm(GNP ~ Employed + pcnt_unemployed + pcnt_af, data = .)

# pass the data through the pipeline and save as lm_model
lm_model <- pipeline(longley)

# view the summary of the lm_model
summary(lm_model)
```

