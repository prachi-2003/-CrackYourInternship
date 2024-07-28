### Day 12

- Question 1: decode string (https://leetcode.com/problems/decode-string/)
key point: create two stacks, one for digit and one for char. perform string addition. Traverse the string once and do different operation for [ ,char,int and ]. 

- Question 2: Shortest bridge (https://leetcode.com/problems/shortest-bridge/description/)
key point: perform dfs/bfs on one island and then do multisource bfs from that island just like in steps by knight, as soon as you encounter a 1 which is not visited, return the no of steps counted by then.

- Question 3: Number of operations to make network connected (https://leetcode.com/problems/number-of-operations-to-make-network-connected/description/)
key point: count the no of components (cnt). cnt-1 will give the no of required edges to connect all computers. connections.size()-((n-1)-reqEdges) will give the no of extra edges.

- Question 4: Find eventual Safe states (https://leetcode.com/problems/find-eventual-safe-states/description/)
key point: every node which is part of a cycle or directed to a cycle will never be a safe node.use dfs 

- Question 5: Strongly connected components  (https://www.geeksforgeeks.org/problems/strongly-connected-components-kosarajus-algo/1)
key point:find topo sort, reverse the direction of each edge and perform dfs on topo sort.
