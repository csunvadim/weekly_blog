---
layout:     post
title:      Parallel Processing for Data
date:       2020-02-21 05:20:33
summary:    Summary for week 4.
categories: jekyll pixyll
---

In the modern world data is the desire and need for data is ever-growing. 
Whether the it is Marketing, Research, or Finance, there are multiple things that each department needs to know. 
Recently, the concept of Big Data has been gaining popularity, with some companies wanting to process gigabytes and terabytes of data. 
However, data only has value if it is properlly processed, transformed and delivered the the people using it, and the larger the amount - the harder it is to produce quality results. 
The most efficent approach to process data is by using parallel processing.

There are many frameworks for parallel processing with most popular ones being Apache's Spark, Apache's MapReduce and Python's Dask, but eseentially the concept behind them is similar. 
In a standard sequential process, a data set of 10 rows, would take 10 iterations to complete, however, if there were 10 processes running in parallel, the same data set would be processed in one iteration total completed by each process. 
This ability allows for a great performance improvement, which made previously impossible amounts of data to process, become a reality. 
The most complicated part is synchronizing these processes and establishing a proper communication between them. 
For example, in sequential process if there is a failure - the entire process stops, however, in parallel structure, each process is individual, so if you need them all to stop in case of a failure, there needs to be specific logic for that.

In conclusion, while parallel processing is more complicated than sequential processing, the benefits it offers are enough to explain why it is growing more and more popular every day. 
Same process that would take 12 hours, can be reduced to as little as a couple of minutes with proper parallization. 