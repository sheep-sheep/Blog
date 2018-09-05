---
title: System Design Notes
date: 2018-08-27 21:17:14
top: 9
tags: system design
---

1. How to approach? **5 S**

   Scenario

   ​	Users; Use case; inputs and outputs;

   Numbers

   ​	DAU; Request per second; Read heavy/Write heavy

   Service

   ​	Implement high level components.

   ​	Front-end; Middle layer; Back-end

   ​	Serial or Parallel

   Store

   ​	SQL/No-SQL;

   ​	Schema;

   ​	OOD;

   ​	How does one operation look like

   Scale

   ​	Address Bottlenecks

   ​	Horizontal Scaling

   ​	DB sharding

   ​	Caching

   ​	Load Balancer

2. Back-of-envelope calculations

   This is to handle the number part and give you an overview of the basic numbers and speed.

   1) Basic numbers:

![](C:\Users\Yang\Documents\GitHub\blog\source\images\numbers.png)

​	CPU 3Ghz --> 0.3 ns --> 0.1 ms --> 1 ms --> 10 ms --> 20 ms

Handy conversion guide:

- 2.5 million seconds per month
- 1 request per second = 2.5 million requests per month
- 40 requests per second = 100 million requests per month
- 400 requests per second = 1 billion requests per month

​	2) popular websites' DAU/MAU:

​		Twitter: 300m MAU

​	3) Database performance

​		How many reads/writes does MySQL support?

​		How many reads/writes does Casandra support?

To address the 40 *average* read requests per second (higher at peak), traffic for popular content should be handled by the **Memory Cache** instead of the database. The **Memory Cache** is also useful for handling the unevenly distributed traffic and traffic spikes. The **SQL Read Replicas** should be able to handle the cache misses, as long as the replicas are not bogged down with replicating writes. 

​	4) Load Balancer Performance

​		Nginx can distribute how many requests?



3. System Design Concepts

   