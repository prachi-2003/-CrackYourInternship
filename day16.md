### Day 16

- Question 1: Snakes and ladder (https://leetcode.com/problems/snakes-and-ladders/)

key point: whenever we are asked for shortest path, we apply bfs since this traversal gives us the shortest path.we do bfs traversal until the front becomes n*n. we keep counting the levels (or steps) of traversal which gives us the min no of steps required. if board[i][j]=-1, we push front+k (k is from 1 to 6) into queue, else we push board[i][j]
Major catch here is to find the coordinates of front+k in the board. Normally, if we have 1 2 3 4... in matrix from top to bottom in row filling and left to right column filling, we find row and column of  value by
rowNormal=(value-1)/no of rows 
colNormal=(val-1)%no of col 
But here, we have bottom to top filling of rows and right to left , then left to right alternate filling of columns, so we find the coordinates via
row=(n-1)-rowNormal
col=(n-1)- colNormal if right to left else colNormal.
the filling will be right to left if (row%2==0 && n%2==0) || (row%2==1 && n%2==1);


