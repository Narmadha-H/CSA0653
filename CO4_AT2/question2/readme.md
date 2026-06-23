# Manufacturing Resource Allocation Using Dynamic Programming

## Project Title
Manufacturing Resource Allocation System Using Dynamic Programming

## Objective
To determine the optimal combination of products that maximizes total profit without exceeding the available production budget.

## Problem Statement
A manufacturing company has a production budget of Rs.100,000 and several product options. Each product requires a specific investment and generates a certain profit. The objective is to select products that maximize profit while staying within the budget.

## Input Data

| Product | Investment (Rs.) | Profit (Rs.) |
|---------|------------------|--------------|
| A | 20,000 | 25,000 |
| B | 30,000 | 40,000 |
| C | 40,000 | 50,000 |
| D | 50,000 | 65,000 |

Total Budget = Rs.100,000

## Algorithm Used
Dynamic Programming (0/1 Knapsack Algorithm)

## Steps
1. Create a DP table.
2. Calculate maximum profit for each investment capacity.
3. Backtrack through the table to identify selected products.
4. Display the optimal product combination and maximum profit.

## Output

Selected Products: A, B, D

Total Investment: Rs.100,000

Maximum Profit: Rs.130,000

## Time Complexity
O(n × W)

where:
- n = Number of products
- W = Budget capacity

## Space Complexity
O(n × W)

## Advantages
- Produces an optimal solution.
- Avoids repeated calculations.
- Efficient for resource allocation problems.

## Applications
- Manufacturing planning
- Budget allocation
- Investment planning
- Resource optimization
- Production scheduling

## Conclusion
Using Dynamic Programming, the company should invest in Products A, B, and D to achieve the maximum profit of Rs.130,000 without exceeding the budget of Rs.100,000.