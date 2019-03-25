---
title: "TrackProposal"
author: "Anthony DiCecco"
date: "March 23, 2019"
output: html_document
---

### Skill Track
# Data Engineering with R {#anchor}

Going from individual data manipulation to full data scale production data flows. Learn the techniques needed to apply big data processes to automate data for Data Scientists and Analysts. Compare different connection types, databases, and methods to process data to become a well-rounded Data Engineer!

R Language | 6 Courses

## Course 1 - Interacting with databases in R
   * Description - Connect to multiple types of SQL databases to start a data flow. This course will cover setting up and maintaining multiple connections to SQL databases. We will also cover best practices for interacting with production databases securely. 
   * Objective 1 - Learner will be able to use the `odbc` and `DBI` packages to connect to SQL Databases.
   * Objective 2 - Learner will be able to compare querying functions and differentiate between dbGetQuery, dplyr, and R Notebook's SQL Engine.
   * Objective 3 - Learner will be able to recognize best practices for running safe queries and credentials. 
   * Prerequisite course - Importing Data in R (Part 2) - covers basics on how to connect R to databases.
     
## Course 2 - Introduction to MondoDB in R
   * Description - Use the power of MondoDB to explore NoSQL data. This course provides an overview of capabilities and structure of handling unstructured data in a simple way.
   * Objective 1 - Learner will be able to create a local MondoDB server and connect a SSL.
   * Objective 2 - Learner will be able to demonstrate querying techniques to `query`, filter `fields`, `sort`, and `limit` data.
   * Objective 3 - Learner will be able to recommend best practices for importing and exporting local JSON files as well as use the `jsonlite` package.
   * Prerequisite course - Working with Web Data in R - for more background for working with JSON data and APIs.

## Course 3 - Introduction to AWS in R
   * Description - Connect to AWS Redshift and S3 buckets to manage data in the cloud. Utilize the `odbc`, `aws.s3`, and `aws.signature` packages to set up connections. Introduction to the benefits of using RStudio on an ec2 instance.
   * Objective 1 - Learner will be able to experiment with multiple ways to read from S3 buckets using the `get_object`, `s3read_using`, and `spark_read_csv` functions. 
   * Objective 2 - Learner will be able to compare working on a local machine to working on an AWS ec2 instance with RStudio. Usage of the `aws.ec2metadata`, `doMC`, and `doParallel` packages to get the most out of the cloud.
   * Prerequisite course - Introduction to Spark in R using sparklyr - covers basics of the sparklyr package.

## Course 4 - Introduction to HDFS in R
   * Description - Hadoop's Distributed File System is backbone for storing large data. This course will give an overview of HDFS and some initial tools to connect to HDFS solutions. 
   * Objective 1 - Learner will be able to describe the difference between traditional databases and HDFS.
   * Objective 2 - Learner will be able to demonstrate how to connect to and query data from a HDFS using `odbc`, `rmr`, `rhdfs`, and `rhbase`.
     
## Course 5 - Big Data Fundamentals with sparklyr
   * Description - Taking the basics of sparklyr to the next level with advanced data management. This course will cover development of data flows with spark data frames and feature transformations to get ready for modeling.
   * Objective 1 - Learner will be able to define best practices for creating a data flow utilizing lazy processing.
   * Objective 2 - Learner will be able to create effective data flows to maximize use of cluster computing.
   * Objective 3 - Learner will be able to compare accessing data in memory vs Resilient Distributed Datasets.
   * Prerequisite course - Introduction to Spark in R using sparklyr and Parallel Programming in R - covers basics of sparklyr package and concepts of how parallel processing works with R.

## Course 6 - ML Pipelines with sparklyr
   * Description - Take pipelines of data straight into machine learning models to complete analysis. Once models are built, they can be used in production to predict outcomes. This course will also cover reusing and refitting models. 
   * Objective 1 - Learner will be able to compose data flow diagrams to accompany a data pipeline. 
   * Objective 2 - Learner will be able to experiment with feature engineering techniques.
   * Objective 3 - Learner will be able to design and evaluate machine learning models to determine an optimal solution.
   * Prerequisite course - Modeling with Data in the Tidyverse - covers modeling in R.
