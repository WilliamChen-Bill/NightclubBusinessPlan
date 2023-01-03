# Nightclub Business Plan
## Project Main Idea/Goal:

* we want to find out the **minimum cost** to fulfilling the demand of the nightclub and also try to figure out how we are going to run this nightclub business for **maximum profit**.

## Project Goal for part (a) and part (b):

* **Part (a)** goal of this project is utilizing **Multiperiod Planning Programming** to calculate the minimum cost to produce the different drinks for nightclubs.
  * Most multi-period planning problems have a "planning horizon".  $T = \left\\{1,2,\dots,T^{\text{max}}\right\\}$
  * Idea of balance for each month which is T
  
* **Part (b)** goal of this project is utilizing **Integer Programming** to make a decision about which month we should open our nightclub, change to open as a bar, or not open both in different months based on the random dataset for the demand of the nightclub customers.
1. add indicator variable 

```math
 z_i = \left\{\begin{array}{l}\text{1 if we make product i}\\\\\text{0 otherwise}\end{array}\right.\\
```
2. Logical constraint
```math
(x_i > 0 \Rightarrow z_i = 1)\equiv(z_i = 0 \Rightarrow x_i = 0)
```
3. add y algebraic constriants to model the logic

```math
\sum_{i=1}^{n}z_i \leq y
```
```math
x_i \leq M_iz_i \;\;\; \forall i = 1,\dots,n
```

## Project Skills:

* Julia, JuMP
* Optimzer choice: Gurobi
* Integer Programming, Linear Programming (Multiperiod Planning Programming)
