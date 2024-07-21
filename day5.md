### Day 5
- Question 1: sudoko solver (https://leetcode.com/problems/sudoku-solver/description/)
 key point: complete 1 cell by trying all values in it and recursion will complete the rest.write isSafe function and perform backtrack. 

- Question 2: subsets (https://leetcode.com/problems/subsets/description/) 
key point : include and exclude each element (perform for one and call recursion for rest).create a vector, include an element by pushing it into vector and then calling index+1, exclude an element by directly calling index+1 . (index: 0-> nums.size()...reaches base case at nums.size() (push output into ans on reaching base case)).

- Question 3: Subsets - II (https://leetcode.com/problems/subsets-ii/description/)
 key point : run a for loop from index to n, if i>index && nums[i]==nums[i-1], we continue. Otherwise, we push nums[i] into output, do recursion for index+1 and backtrack. index goes from 0 to n through recursive calls.1st line is to push output into ans.

 
