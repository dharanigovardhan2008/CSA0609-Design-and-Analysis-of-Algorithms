# Problem Statement

## Comparative Analysis of Dynamic Programming and Greedy Algorithms for Optimization Problems

### Course Details

- **Course Code:** CSA06
- **Course Title:** Design and Analysis of Algorithms
- **Assessment Tool:** Assessment Tool 3 – Comparative Analysis
- **Course Outcome:** CO4 – Articulation (BL4, BL5)

### CO4 Statement

> Solve optimization problems using dynamic programming and greedy strategies.

---

## Objective

The objective of this comparative analysis is to study and evaluate **Dynamic Programming (DP)** and **Greedy Algorithms** as techniques for solving optimization problems.

The analysis focuses on understanding how both approaches make decisions, how they achieve optimal solutions, their correctness, computational complexity, scalability, advantages, limitations, and suitability for real-world applications.

---

## Problem Description

Optimization problems require finding the best solution from a set of feasible solutions while satisfying given constraints.

Two important algorithmic strategies used for optimization problems are:

1. **Dynamic Programming**
2. **Greedy Algorithms**

Dynamic Programming solves problems by breaking them into smaller overlapping subproblems, storing their solutions, and combining them to obtain an optimal solution.

Greedy Algorithms make the best available local choice at each step with the expectation that these choices lead to a globally optimal solution.

However, these approaches behave differently depending on the structure of the optimization problem.

Therefore, a detailed comparison is required to determine:

- When Dynamic Programming is appropriate.
- When Greedy Algorithms are appropriate.
- Why Dynamic Programming can guarantee optimal solutions for suitable problems.
- Why Greedy Algorithms can fail for certain problems.
- How their time and space complexities differ.
- How their scalability changes with increasing input size.
- Which approach is more suitable for different real-world optimization problems.

---

## Problems Considered

The analysis considers representative optimization problems such as:

### Dynamic Programming

- 0/1 Knapsack Problem
- Longest Common Subsequence
- Matrix Chain Multiplication
- Coin Change Problem
- Rod Cutting Problem

### Greedy Algorithms

- Fractional Knapsack Problem
- Activity Selection Problem
- Huffman Coding
- Job Sequencing with Deadlines
- Prim's Algorithm
- Kruskal's Algorithm

---

## Key Comparison Parameters

The following parameters are used for comparative analysis:

| Parameter | Dynamic Programming | Greedy Algorithm |
|---|---|---|
| Basic Strategy | Solves overlapping subproblems | Makes locally optimal choices |
| Decision Making | Considers multiple possibilities | Selects the best current option |
| Optimal Substructure | Required | Required |
| Greedy-Choice Property | Not required | Required for guaranteed optimality |
| Subproblem Storage | Usually required | Usually not required |
| Memory Usage | Generally higher | Generally lower |
| Exact Solution | Yes, for suitable problems | Only when greedy strategy is provably optimal |
| Implementation | Relatively complex | Usually simpler |
| Scalability | Depends on state-space size | Usually efficient for suitable problems |
| Typical Complexity | Problem dependent | Often polynomial |
| Main Limitation | Time and memory requirements | May produce non-optimal solutions |

---

## Case Study: 0/1 Knapsack vs Fractional Knapsack

A major comparison is made using the Knapsack family of optimization problems.

### 0/1 Knapsack

Each item can either be completely selected or completely rejected.

Dynamic Programming can be used to find the optimal solution.

Typical complexity:

- **Time:** `O(nW)`
- **Space:** `O(nW)`

where:

- `n` = number of items
- `W` = capacity of the knapsack

### Fractional Knapsack

Items can be divided into fractions.

A Greedy Algorithm selects items according to their profit-to-weight ratio.

Typical complexity:

- **Time:** `O(n log n)`
- **Space:** `O(n)` depending on implementation

This comparison demonstrates an important distinction between the two strategies: a greedy approach that works optimally for Fractional Knapsack does not necessarily provide an optimal solution for 0/1 Knapsack.

---

## Activity Selection

The Activity Selection Problem is used to demonstrate the effectiveness of the Greedy strategy.

Given a collection of activities with starting and finishing times, the objective is to select the maximum number of non-overlapping activities.

The standard greedy strategy selects the activity with the earliest finishing time.

After sorting activities by finishing time, the typical complexity is:

```text
O(n log n)
