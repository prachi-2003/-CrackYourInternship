### Day 17

- Question 1: Cheapest flights with K stops (https://leetcode.com/problems/cheapest-flights-within-k-stops/description/)
key point: here the meaning of steps is no of nodes, and in dijkstra, it will take more no of nodes if its shorter. but we have to find in atmost k steps(or nodes). So, dijkstra or common shortest distance algo cannot be applied.
we need to consider min stops instead of min costs.
instead of priroity queue or set, we can simply take a queue because the stop will increase by one as we move ahead and the topmost element will always be the node with min stops.( since the increase is constant)
Tc- O(no of edges(flights.size)).


- Question 2:bipartite graph(https://www.geeksforgeeks.org/problems/bipartite-graph/1)
key point:bipartite graph is a graph which can be colored with 2 colors such that no two adjacent nodes have same color.Linear graphs with no cycles and graphs with even cycle length are always bipartite. hence, odd length cycle graph is not bipartite. we fill up colors via bfs and if we encounter any two adjacent nodes with same color,we return false.

- Question 3: Longest increasing path in a matrix (https://leetcode.com/problems/longest-increasing-path-in-a-matrix/description/)
key point: since we dont know from which node to start from, we will check for each cell and create a helper vector where helper[i][j] is the max length of path if matrix[i][j] was a starting node.we can directly use this value if we encounter [i][j] in a path from a different starting cell.(memoization)  

