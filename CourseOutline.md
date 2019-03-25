---
title: "CourseOutline"
author: "Anthony DiCecco"
date: "March 23, 2019"
output: html_document
---

# ML Pipelines with sparklyr {#anchor}

## Course 6 - ML Pipelines with sparklyr
   * Description - Take pipelines of data straight into machine learning models to complete analysis. Once models are built, they can be used in production to predict outcomes. This course will also cover reusing and refitting models. 
   * Objective 1 - Learner will be able to compose data flow diagrams to accompany a data pipeline. 
   * Objective 2 - Learner will be able to experiment with feature engineering techniques.
   * Objective 3 - Learner will be able to design and evaluate machine learning models to determine an optimal solution.

### Chapter 1 - Introduction to Pipelines
   * Lesson 1.1 - Introduction to the plumbing of data pipelines.
     * A learning objective: Compare `dplyr` and `sparklyr` packages to create a path
     * Some functions introduced/used: `select()`, `mutate()`, `filter()`, `summarize()`, `group_by()`, `lm()`
   * Lesson 1.2 - Visualize your data flow with DiagrammeR
     * A learning objective: Create a simple flow diagram to plan how the data will be processed.
     * Some functions introduced/used: `grViz()`
   * Lesson 1.3 - Basic pipelines for linear models
     * A learning objective: Write a basic data pipeline and run segments of the longley data set through linear models.
     * Some functions introduced/used: `select()`, `mutate()`, `filter()`, `summarize()`, `group_by()`, `lm()`

### Chapter 2 - Feature Transforming 
   * Lesson 2.1 - Basics of Feature Transforming
     * A learning objective: Select appropriate transforming functions to create additional variables to model on.
     * Some functions introduced/used: `ft_binarizer()`, `ft_bucketizer()`, `ft_quantile_discretizer()`, `ft_count_vectorizer()`
   * Lesson 2.2 - Flexible Feature Transformations
     * A learning objective: Demonstrate how SQL and dplyr can be used inside Spark for transformation flexibility.
     * Some functions introduced/used: `ft_dplyr_transformer()`, `ft_sql_transformer()`
   * Lesson 2.3 - Strings to Numbers (or reversed)
     * A learning objective: Modify strings to be stored as numeric columns as well as numeric to a string.
     * Some functions introduced/used: `ft_one_hot_encoder()`, `ft_index_to_string`, `ft_string_indexer()`
   * Lesson 2.4 - Feature Scaling 
     * A learning objective: Identify situations where scaling features is necessary.
     * Some functions introduced/used: `ft_elementwise_product()`, `ft_discrete_cosine_transform()`

### Chapter 3 - Pipeline Models
   * Lesson 3.1 - Implement pipelines with `sparklyr`
     * A learning objective: Apply sparklyr functions in place of dplyr to build data pipelines.
     * Some functions introduced/used: `sdf_mutate()`, `sdf_sort()`, `sdf_partition()`, `sdf_register()`, `sdf_sample()` 
   * Lesson 3.2 - Model those pipelines!
     * A learning objective: Choose the correct modeling technique to help answer questions with data. 
     * Some functions introduced/used: `ml_generalized_linear_regression()`, `ml_linear_regression()` `ml_logistic_regression()`
   * Lesson 3.3 - More models, more fun!
     * A learning objective: Organize and produce multiple models to better determine the best fit.
     * Some functions introduced/used: `ml_pipeline()`, `ml_decision_tree()`, `ml_random_forest()`, `ml_survival_regression()`

### Chapter 4 - Reuse and Refit Pipeline Models
   * Lesson 4.1 - Use pipelines to predict new data
     * A learning objective: Use a pipeline and model with new data to predict the results.
     * Some functions introduced/used: `sdf_predict()`
   * Lesson 4.2 - Save for later, load for now
     * A learning objective: Compose `ml_save()` and `ml_load()` functions to keep track to models for use when needed. 
     * Some functions introduced/used: `ml_save()`, `ml_load()`
   * Lesson 4.3 - Putting it all together
     * A learning objective: Compile resources learned to create a data flow to compare models and save the best performing one for production use.
     * Some functions introduced/used: `ml_fit()`
