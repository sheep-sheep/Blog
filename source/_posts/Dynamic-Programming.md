---
layout: 
title: Dynamic Programming
date: 2018-12-11 18:45:31
tags:
---

## Definition

Dynamic Programming is a special form of divide and conquer method, it's very useful when the subproblems overlap each other. By using a tabular method, it stores the computed result to accelerate the computation.

There're 4 steps to construct a solution to DP problems:
        1. Characterize the structure of an optimal solution(How to represent the problem using "last step" and "subproblem")
        2. Recursively build the value of an optimal solution(How to use a function to build the relationship)
        3. Compute the value of setup 2 typically in a bottom-up fashion(Initial Value[0, INF])
        4. Construct the solution from computed information(Bottom up)

## Top-down and Bottom-up

Both top-down and bottom-up can be used to solve the DP problems, but they have different though process and coding paradigm.

1. With Top-down:

   a. you have to start from the *final question* (F(N))

   b. each level reduce the problem to a smaller size, until you reach the *base case* and the problem is trivial to solve (F(N-1) or F(N/2) etc.)

   c. return the base case immediately (F(0) or F(1)) (**return type depends on the question**)

   d. don't forget to also return at each general case level (Build the relationship at this step)

   With Top-down, you can use **memoization** to reduce the time complexity.

   Time Complexity: O(N*)

   Space Complexity: O(height)

2. With Bottom-up:

   a. you have to start from the *base solution* (F(0) or F(1))

   b. each level build the solution to a larger size, until you reach the *final solution* (F(N-1) or F(N/2) etc.)

   c. return the *final solution* immediately (F(N))

   Time Complexity: O(N**2)

   Space Complexity: O(N**2)

3. Another way to separate the 2 methods is to check their implementation: 

   ​	Bottom-up is the Iterative implementation of Top-down

   ​	Top-down is recursive way which uses the stack to hold and wait for the return of F(N-1)

## Top-down and Backtracking

1. They have similar recursive call implementation

2. **They can all be treated as a Root-Leaf Path**

3. They have different way to verify the base case

4. backtracking usually have one global variable to record *curr* path
