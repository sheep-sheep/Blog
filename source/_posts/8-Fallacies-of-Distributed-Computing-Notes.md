---
title: 8 Fallacies of Distributed Computing Notes
date: 2018-08-16 23:21:56
top: 10
tags: reading
---

### Fallacies of Distributed Computing Explained[^*]

[^*]: http://www.rgoarchitects.com/Files/fallacies.pdf

1. The network is reliable

   "Murphy will make sure it  happens in the most inappropriate moment."

   **infrastructure side: redundancy

   **software side:  communication medium; retry

2. Latency is zero

   "It will always take at least 30 milliseconds to send a ping from Europe to the US and back, even if the processing would be done in real time."

   You'd want to move as much data out in each of this calls.

3. Bandwidth is infinite

4. The network is secure

5. Topology(**布局**) doesn't change

   "In short, topology is changing constantly."

   Try not to depend on specific endpoints or routes.

   Another strategy is to abstract the physical structure of the network.

6. There is one administrator

7. Transport cost is zero

   "we have to do marshaling (serialize information into bits) to get data unto the wire."

8. The network is homogeneous.