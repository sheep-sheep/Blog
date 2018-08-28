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

   Basic numbers:

![](C:\Users\Yang\Documents\GitHub\blog\source\images\numbers.png)

CPU 3Ghz --> 0.3 ns --> 0.1 ms --> 1 ms --> 10 ms --> 20 ms

3. System Design Concepts

   

