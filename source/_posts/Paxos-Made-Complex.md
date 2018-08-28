---
title: Paxos Made Complex
date: 2018-08-16 22:24:56
top: 10
tags: reading
---

"The Paxos algorithm, when presented in plain English, is very simple." said the author Lamport, however, I find out it has caused more confusion and questions for me after I finished the article. Most of the doubts come from 3 areas:

1. How does it work?
2. How do you implement it?
3. What're the advantages of this algorithm?

I hope as my reading activities continue those doubts can be cleared eventually! 



### Application

分布式存储系统&&分布式应用系统

paxos算法是一个比较完备的解决分布式一致性的算法

1是能够保证集群操作的顺序化，2在主机宕机重选之后集群操作的不丢失和可恢复 

[ZooKeeper](http://zookeeper.apache.org/)

