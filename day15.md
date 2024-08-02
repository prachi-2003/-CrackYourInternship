### Day 15

- Question 1: Floyd warshall (https://www.gdayeeksforgeeks.org/problems/implementing-floyd-warshall2042/1)
key point: for each element in matrix[i][j], set it as min of matrix[i][j] and matrix[i][k]+matrix[k][j], where k goes from node 0 to node n-1;

- Question 2:Find the city with smallest number of neighbours at a threshold distance (https://leetcode.com/problems/find-the-city-with-the-smallest-number-of-neighbors-at-a-threshold-distance/description/)
key point: create a distance 2d vector and using floyd warshall, store the min distance of each node from each node. Now, loop through each row (or city), and count the no of elements (or adjacent cities) with distance smaller or equal to threshold distance. It this count is less than previously stores cnt, update it along with city no.

- Question 3: Pre requisite Tasks (https://www.geeksforgeeks.org/problems/prerequisite-tasks/1)
key point: detect cycle in directed graph formed, if cycle present return false. If we are asked to find the ordering as well, use bfs to detect cycle in directed graph and then return the topo sort. Or you can find topo sort and check its size.Check cycle through dfsvis also.

- Question 4: Minimum Spanning Tree (https://www.geeksforgeeks.org/problems/minimum-spanning-tree/1)
key point: use prims algorith. The vector key stores weights involved in MST, so sum its element other than INT_MAX to find the sum of all weights in MST. If edges are asked, the parent[i] to i will be the edge and key[i] will be the weight of that edge (i is iterated from 0 to V).

- Question 5: Evaluate division (https://leetcode.com/problems/evaluate-division/description/)
key point: create a graph with edge from Ai to Bi (from equations) with weight values[i]. Also create an edge from Bi to Ai with weight 1/values[i]. now travel from src ( queries[0]) to dest (queries[1]) and keep multiplying the weights you encounter in path, traverse via dfs (or bfs) and when src=dest, return the product.


