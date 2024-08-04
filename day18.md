### Day 18

- Question 1: Making a large island (https://leetcode.com/problems/making-a-large-island/description/)

key point: whenever we need to dynamically change the graph to solve the problem (such as here we can convert one 0 to 1), we use disjoint set data structure to solve the problem. Each cell in the matrix is represented by a row and column.but in disjoint sets, we represent each node with a single number and it is parent of itself initially.lets say there are 5 rows* 6 columns=30 cells. we will represent the cells from 0 to 29. row no*nofo columns+col no = node number.  step 1: perform union by rank on all islands        step 2: try converting 0 to 1 one by one, union them with 1s present in 4 directions and then choose the one with max size.
edge case: if a 0 is surrounded by 1s of same island from 2 or more directions, you will end up adding the same size for all 2 or more directions while we can only join the island and 0, which is wrong. SO instead of storing sizes, we take a set data structure and store the parent of neighbour 1.

- Question 2: Remove boxes (https://leetcode.com/problems/remove-boxes/description/)


