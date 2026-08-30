# Problem Statement

## Dominating Set Problem (NP-Complete Problem)

### Course Details

- **Course Code:** CSA06
- **Course Title:** Design and Analysis of Algorithms
- **Course Outcome:** CO4 – Articulation (BL4, BL5)
- **Topic:** Dominating Set Problem (NP-Complete Problem)

---

## 1. Overview

The **Dominating Set Problem** is a fundamental graph-theoretic optimization problem and an important example of an **NP-Complete decision problem**.

Given an undirected graph:

\[
G = (V,E)
\]

the objective is to find a minimum subset of vertices:

\[
D \subseteq V
\]

such that every vertex in the graph is either:

1. Present in the dominating set \(D\), or
2. Adjacent to at least one vertex in \(D\).

The minimum possible size of such a set is called the **Minimum Dominating Set**.

---

## 2. Problem Definition

Given a graph:

\[
G = (V,E)
\]

find a subset:

\[
D \subseteq V
\]

such that:

\[
\forall v \in V,\quad v \in D \ \text{or}\ \exists u \in D \text{ such that } (u,v)\in E
\]

and minimize:

\[
|D|
\]

In simple terms:

> Select the smallest possible number of vertices so that every vertex in the graph is either selected or connected to a selected vertex.

---

## 3. Example

Consider the following graph:

```text
        2
       / \
      /   \
     1 --- 3
     |     |
     |     |
     4 --- 5
           |
           6
