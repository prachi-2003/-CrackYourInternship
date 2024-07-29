### Day 13

- Question 1: Graph Coloring (https://www.geeksforgeeks.org/problems/m-coloring-problem-1587115620/1)
key point: try all colors one by one for a node. try one color for a node and then perform recrusion to fid if coloring was possible. if not, try next color and so on.

- Question 2: Time needed to infor all employees (https://leetcode.com/problems/time-needed-to-inform-all-employees/description/)
key point: perform dfs and keep adding time required by current node to inform its subordinates. Backtrack on returning. the max time taken by path is ans.

- Question 3: Most stones removed with same row or column (https://leetcode.com/problems/most-stones-removed-with-same-row-or-column/description/)
key point: we perform union of row and column of all stones. No of nodes left after union which are parents of itself will give the no of components. Each component needs to have 1 element left as it will not have any row or column with stones after all the other stones from this component are removed. So, no of stones that can be removed will be stones.size()- no. Of components.

- Question 4: As far land as possible (https://leetcode.com/problems/as-far-from-land-as-possible/description/)
key point: start bfs simultaneously from all 1's (multi source bfs). Return the max number of level of traversal reached    

