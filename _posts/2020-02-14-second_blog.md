---
layout:     post
title:      Proper Cloud Architecture
date:       2020-02-14 10:40:39
summary:    Summary for week 3.
categories: jekyll pixyll
---

The cloud architecture has many various benefits versus on-premise. 
Amongsts those benefits are much better scalability, easier most cases better prices and cost efficency. 
However, even in order to best utilize the cloud architecture, the architect needs to understand the cloud, otherwise it is impossible to make the best architecture and usage is choices. 

Let's assume there are 10 pieces of code that need to be executed at various different intervals every single day. 
In the traditional on-premise system, there would be a server always running that would have a schedueler that would run these jobs. 
However, on cloud, this has many disadvantages, such as a chance of jobs running concurenntly and competing for resources, but the biggest disadvantage of this is the unnecessary expenses. 
While traditionally, it would make sense to have a server always running, in cloud - this is not always the case. 
Instead of having a server running at all times, it makes a lot more sense to schedule these 10 pieces of code directly in the cloud, for example, in AWS there are tools such as Lambda and CloudWatch that could be used for that. 
By using the cloud to schedule these coding jobs the business will only be paying for cloud resources as they are used which is much cheaper in contrast to paying for a server that is running constantly. 

Another example of proper architecture is scalability. 
In traditional architecture, it would be unusual to use code which is designed to utilize the maximum of resources of a machine. 
However, in cloud where you can have virtual computers available for usage as needed, it makes a lot of sense to write code designed to fully utilize the machine for which the business is paying.

In conculussion, while going to cloud is a very good options that comes with great benefits, it is important to fully understand these benefits in order to utilize them. 