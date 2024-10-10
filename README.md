# Supply-Chain-Problem-CSP

This repository contains a [CSP](https://en.wikipedia.org/wiki/Constraint_satisfaction_problem) model written in [essence prime](https://www.csplib.org/Languages/EssencePrime/), which has been evaluated using [Savile Row](https://www-users.york.ac.uk/peter.nightingale/savilerow/). 

## Scenario
The Supply Chain Problem (SCP) involves supplying a set of shops with a product from various suppliers. Each shop has a specific demand for the product, and suppliers offer packages of different sizes and prices. For instance, one supplier might provide boxes of 10 units for £10, while another offers pallets of 100 units for £80. 

The goal is to ensure every shop receives enough units to meet its demand while minimising the total delivery cost. Over-supply is permitted, allowing excess product to be stored for future use. An optimal solution must determine how many packages to order from each supplier for each shop, satisfying demand and minimising costs.

## Evaluation of Solution
| Test Case                               | Minion Solver Nodes | Minion Solver Time (s) |
|-----------------------------------------|---------------------|-------------------------|
| Case 1 (Simple)                        | 12                  | 0                       |
| Case 2 (Low excess stock limit)        | 28,772              | 0.03125                 |
| Case 3 (High Excess stock limit)       | 2,093,734           | 2.90625                 |
| Case 4 (Large difference in shop demands) | 7,101,243           | 10.7188                 |
| Case 5 (Most Challenging)              | 350,766,457         | 268.859                 |
| Test Instance (from paper)             | 10,323,476          | 10.1719                 |

_All code submitted as part of a master module at the University of York - Constraint Programming_
