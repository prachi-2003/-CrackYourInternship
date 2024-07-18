### Day 2
- Question 1: Move zeroes (https://leetcode.com/problems/move-zeroes/description/) key point : use one pointer to find non zero element and another pointer to find the index where next non zero element should be placed and swap them.

- Question 2: Majority Element (https://leetcode.com/problems/majority-element/description/) 
key point : sorting

- Question 3: BFS traversal of graph (https://www.geeksforgeeks.org/problems/bfs-traversal-of-graph/1)
 key point : use queue

- Question 4: dFS traversal of graph (https://www.geeksforgeeks.org/problems/depth-first-traversal-for-a-graph/1) key point : use recursion

- Question 5: Rat in a maze (https://www.geeksforgeeks.org/problems/rat-in-a-maze-problem/1) 
key point : create a function to check if moving to a coordinate is possible according to conditions of question and another function that moves down,left,right and up recursively by checking through first function.

- Question 6: cycle detection in undirected graph (https://www.geeksforgeeks.org/problems/detect-cycle-in-an-undirected-graph/1) 
key point : while traversing, if you find a neighbour of any node which is already visited but is not the parent of node, then cycle is present.

- Question 7: cycle detection in directed graph (https://www.geeksforgeeks.org/problems/detect-cycle-in-a-directed-graph/1) 
key point : by dfs- create a dfsvisited vector/map which is true for a node if it's call has been made and mark it false on returning from function call of that node.Also create a visited vector to track if a node is visited. if you encounter a node with both dfsvisited and visited marked true, a cycle is present.

