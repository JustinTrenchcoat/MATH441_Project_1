# MATH441_Project_1

## Problem Statement
### In real-time strategy (RTS) games, players must manage resources to strength their military power to defeat other players. 
The player has to make sure that the military power requirement is met before declaring war on other players. 
Based on the resources available to the player, how should the player build the army to meet the requirements while minimizing the cost? 

#### Define Variables
| Description | Symbol | 
|-------------|--------|
|Cost of unit $j$ | $c_j$ | 
|Decision variabe, the amount of military unit $j$ we make| $x_j$ |
|How much militray power $i$ is in the unit $j$| $a_j$| 
|Military power requirement |$b_i$ |
|Housing constraint|$h$ |

#### Build Solutions

The total cost

$$
\mathbf{c}^T \mathbf{x} = \sum_j c_j x_j
$$

The military requirement constraints are

$$
\sum_j a_{ij} x_j \geq b_i, i = 1,\dots,m
$$

$$
x_j \geq 0, j = 1,\dots,n
$$

The housing constraint is:
$$
\sum_j x_j \leq h
$$