- 6 easy, 21 medium, 1 hard
- 13 problems were solved for the first time
- [[2022-05-01 Sunday]] #[[Two Pointers]] #String #Stack #Simulation 
  id:: 53fa914e-9f58-47d5-9833-e48233aa6034
  problem:: Backspace String Compare
  link:: https://leetcode.com/problems/backspace-string-compare/
  difficulty:: Easy
  duration:: 20 mins
  number_of_times:: 1
  collapsed:: true
	- easy to solve using additional space
	- use input string to build the final string directly
	- we can use two pointers and iterate from the back to avoid modify strings
- [[2022-05-02 Monday]] #Array #[[Two Pointers]] #Sorting 
  id:: 626f49e4-bf2a-43d8-be4f-5bcae9dca3d6
  problem:: Sort Array By Parity
  link:: https://leetcode.com/problems/sort-array-by-parity/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 1
  collapsed:: true
	- basic two pointers problem
	- use left and right pointers and swap the correct elements onto each other
- [[2022-05-03 Tuesday]] #Array #[[Two Pointers]] #Stack #Greedy #Sorting #[[Monotonic Stack]] 
  id:: 626f4a46-c8bd-4730-8d13-60e1ce11a60e
  problem:: Shortest Unsorted Continuous Subarray
  link:: https://leetcode.com/problems/shortest-unsorted-continuous-subarray/
  difficulty:: Medium
  duration:: 50 mins
  number_of_times:: 1
  collapsed:: true
	- use two pointers to store unsorted subarray's left and right boundaries
	- use two variables to store minimum value in unsorted subarray, and current maximum value
	- if we encounter a number that is smaller than current maximum value, then it must be in the unsorted subarray
		- we must extend right boundary
		- we may need to extend left boundary, if current number is smaller than minimum value of current unsorted subarray
	- use four iterations to make the logic clearer
	- reference
		- [Java O(n) Time O(1) Space](https://leetcode.com/problems/shortest-unsorted-continuous-subarray/discuss/103057/Java-O(n)-Time-O(1)-Space) 
		  type:: article
		  tags:: LeetCode, [[Two Pointers]]
		  title:: Java O(n) Time O(1) Space
- [[2022-05-04 Wednesday]] #Array #[[Hash Table]] #[[Two Pointers]] #Sorting 
  problem:: Max Number of K-Sum Pairs
  link:: https://leetcode.com/problems/max-number-of-k-sum-pairs/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 6271ccb9-4e85-4395-87f9-52e5bff5c17d
  collapsed:: true
	- sort the array and add elements that are less or equal to the half of k into hash table
	- for every number that is greater than the half of k, we should check if there is a complemental number that will sum to k
	- we should handle numbers that are equal to the half of k as special case
	- we don't need sorting and hash table at the same time
	  collapsed:: true
		- hash table is enough
		- sorting and pair with two pointers
- [[2022-05-05 Thursday]] #Stack #Design #Queue
  problem:: Implement Stack using Queues
  link:: https://leetcode.com/problems/implement-stack-using-queues/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 62731d15-d128-4312-a7b2-9bd00879aec2
  collapsed:: true
	- implement stack using two queues
	- `push()` method requires $O(n)$ time
	- to using one queue, we can pop and push the numbers that are originally in the queue back to the newly added number
- [[2022-05-06 Friday]] #String #Stack
  problem:: Remove All Adjacent Duplicates in String II
  link:: https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string-ii/
  difficulty:: Medium
  duration:: 1 hr 30 mins
  number_of_times:: 1
  id:: 6273c8ab-d031-46c0-8dab-018d19a44649
  collapsed:: true
	- tried to delete adjacent duplicates iteration by iteration
		- TLE
	- use stack to remove duplicates in one iteration
	- because we can detect duplicates that are eligible to be deleted whenever we find one, so we don't have to be worry about ignoring duplicates
	- we can use two pointers and two arrays to solve this problem
		- one array to mimic stack's functionality, another for recording duplicates count
- [[2022-05-07 Saturday]] #Array #[[Binary Search]] #Stack #[[Monotonic Stack]] #[[Ordered Set]] 
  problem:: 132 Pattern
  link:: https://leetcode.com/problems/132-pattern/
  difficulty:: Medium
  duration:: 2 hrs
  number_of_times:: 2
  id:: 62750fa8-fdeb-45f2-b1a0-c228cf876c25
  collapsed:: true
	- the key is to start from the back and find valid `nums[j]` and `nums[k]`
	- keep a decreasing stack, and if we encounter a number that is larger than the number on top of the stack, we find a valid `nums[j]` and `nums[k]` pair
		- pop the stack until the condition break and record the greatest `nums[k]`
	- then if we encounter a number that is smaller than the greatest `nums[k]`, we find the answer
- [[2022-05-08 Sunday]] #Stack #Tree #DFS #Design #Queue #Iterator 
  id:: 6275fa3f-00fc-4f93-9cfd-8619848d055d
  problem:: Flatten Nested List Iterator
  link:: https://leetcode.com/problems/flatten-nested-list-iterator/
  difficulty:: Medium
  duration:: 2 hrs
  number_of_times:: 3
  collapsed:: true
	- use two stacks, one storing the current position of the current vector, another storing the ending position of the current vector
	- every time we call `next()`, we need to move our pointer to the next integer
		- if we reach the end of current vector, pop out both stacks
		- if we encounter a vector, then we need to determine if it is an empty vector
			- move to next position if it's an empty vector
			- push starting and ending position of that vector into stacks
		- the key of setting the loop condition is to use stack's emptiness as condition, and handle popping and pushing stacks in the same loop
	- we need to find the first integer's position in the constructor
	- took too much time, need to do better
- [[2022-05-09 Monday]] #[[Hash Table]] #String #Backtracking 
  problem:: Letter Combinations of a Phone Number
  link:: https://leetcode.com/problems/letter-combinations-of-a-phone-number/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 3
  id:: 62774118-84e3-47a7-a568-72bd110b2a65
  collapsed:: true
	- use backtracking
	- maintain a current string, and only push it into the answer array when it has the same length as the input
- [[2022-05-10 Tuesday]] #Array #Backtracking 
  collapsed:: true
  id:: 6279308f-d8c1-4199-b61a-6bcc25b5d7c6
  problem:: Combination Sum III
  link:: https://leetcode.com/problems/combination-sum-iii/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
	- classic backtracking problem
	- there are two conditions, target sum and how many number must use
- [[2022-05-11 Wednesday]] #DP 
  id:: 627a9dae-3abd-4420-8f10-8b53eb3f7878
  problem:: Count Sorted Vowel Strings
  link:: https://leetcode.com/problems/count-sorted-vowel-strings/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  collapsed:: true
	- this is a math problem, we don't need to actually construct the string
	- to append a new vowel, we can only append it to strings which were appended with a vowel smaller than the current one
	- so we keep track of how many number of strings we append for each vowel, for each iteration
	- we can update this information round by round, and return the answer by summing it up
	- there is a math solution for this
- [[May 12th, 2022]] #Array #Backtracking 
  problem:: Permutations II
  link:: https://leetcode.com/problems/permutations-ii
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 3
  id:: 627c52f5-8fbd-4eb2-a579-e8619f885873
  collapsed:: true
	- straightforward backtracking problem, but need to handle duplicate numbers carefully
	- we construct each permutation element by element
	- for current position's element, we have to exclude swapping same number multiple times, otherwise, once we move to next position, we will have duplicate case
		- consider `[1, 2, 2, 2, 3]`
		- we are at position 0, we swap it with its next element first, and if we proceed to swap it with next two element, then we will have two case with array `[2, 1, 2, 2, 3]` and `[2, 2, 1, 2, 3]`
		- we may create a duplicate if we swap position 1 and 2 in case one, and swap position 1 with itself in case two
	- we use a hash table in each backtrack stage, recording which number has been swapped to current position
- [[2022-05-13 Friday]] #[[Linked List]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Populating Next Right Pointers in Each Node II
  link:: https://leetcode.com/problems/populating-next-right-pointers-in-each-node-ii/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 627d27bd-1c12-4d55-a634-8807e73c3e77
  collapsed:: true
	- BFS but go backward in each level
	- keep a pointer points to previous node, and also push children in reverse order
- [[2022-05-14 Saturday]] #DFS #BFS #Graph #Heap #[[Shortest Path]] #[[Priority Queue]] #[[Dijkstra's Algorithm]]
  problem:: Network Delay Time
  link:: https://leetcode.com/problems/network-delay-time/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 627e79b1-caf4-4a67-a4ef-cd1d6629ee8b
  collapsed:: true
	- use BFS with a priority queue
	- keep a hash table to record which node is visited
	- this is actually Dijkstra's algorithm
	- we don't need record if node is visited or not, we can track the earliest visit time, so we won't push redundant node into the queue
- [[2022-05-15 Sunday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Deepest Leaves Sum
  link:: https://leetcode.com/problems/deepest-leaves-sum/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 627f1b1d-5f09-424f-9306-5ce88789c441
  collapsed:: true
	- easy BFS
	- record sum while iterating a level
	- if the queue becomes empty, then we return last level sum as answer
- [[2022-05-16 Monday]] #Array #BFS #Matrix 
  problem:: Shortest Path in Binary Matrix
  link:: https://leetcode.com/problems/shortest-path-in-binary-matrix/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 62806396-955b-49b6-85df-67b321977911
  collapsed:: true
	- straightforward BFS problem
	- to avoid push the same cell into queue in the same iteration, we need to make sure the steps required to reach cell is not smaller or equal to the steps required to reach current cell plus one
	- need to be careful of the edge case, where the matrix has only one cell
- [[2022-05-17 Tuesday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Find a Corresponding Node of a Binary Tree in a Clone of That Tree
  link:: https://leetcode.com/problems/find-a-corresponding-node-of-a-binary-tree-in-a-clone-of-that-tree/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 6282efa4-9e46-4e47-b229-d68f38f72178
  collapsed:: true
	- simple DFS problem
	- use two stacks to track each tree's traversal
	- use recursive DFS may save some space
- [[2022-05-20 Friday]] #Array #DP #Matrix 
  problem:: Unique Paths II
  link:: https://leetcode.com/problems/unique-paths-ii/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 628692c1-5a3b-4821-9291-cbb8ddbf837c
  collapsed:: true
	- simple DP problem
	- just remember to set the step starting position correctly
- [[2022-05-21 Saturday]] #Array #DP #BFS 
  problem:: Coin Change
  link:: https://leetcode.com/problems/coin-change/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 3
  id:: 6287afa9-df4f-4efe-9e08-10326f6f3edc
  collapsed:: true
	- this is a classic knapsack problem, but I solved it using BFS this time
	- use a hash table to record values
	- if the hash table already contains the value, it means we already get the value by using less or equal to the current numbers of coin
	- should practice DP next time
- [[2022-05-22 Sunday]] #String #DP 
  problem:: Palindromic Substrings
  link:: https://leetcode.com/problems/palindromic-substrings/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 628850df-caf5-4837-a60d-6f5dfcee91eb
  collapsed:: true
	- this is a DP problem, but I solved it by expanding substrings from the center as my note suggestetd
	- need to consider two kinds of center
		- a character
		- two characters
	- remember to check if two pointers reach the bounds
- [[2022-05-23 Monday]] #Array #String #DP 
  problem:: Ones and Zeroes
  link:: https://leetcode.com/problems/ones-and-zeroes/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
  id:: 62899e32-8b12-41dc-a1b0-d6ac8a28a4c9
  collapsed:: true
	- this is a 0-1 knapsack problem
	- we can use a two dimensional array to solve it
	- we also have to calculate each string's number of ones and zeros
	- remember to start the DP from bottom right, so we won't include the same string twice
- [[2022-05-24 Tuesday]] #String #DP #Stack 
  problem:: Longest Valid Parentheses
  link:: https://leetcode.com/problems/longest-valid-parentheses/
  difficulty:: Hard
  duration:: 10 mins
  number_of_times:: 1
  id:: 628bc42c-ddd7-4227-84bb-104e189288ee
  collapsed:: true
	- use DP
	- for every position, we iterate from the back and find the longest valid parantheses
	- we use an array to store the maximum length of valid substring in that range
	- this problem can be solved in $O(n)$
		- use stack
		- use DP, but use previous position's result to check if there is a left parenthesis
- [[2022-05-26 Thursday]] #[[Bit Manipulation]] 
  problem:: Number of 1 Bits
  link:: https://leetcode.com/problems/number-of-1-bits/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 2
  id:: 628e3a1f-672e-4c07-b56a-654546cb6abe
  collapsed:: true
	- solved it easily by iterating each bit from the back
	- we can use $n\&(n-1)$ to cancel out the lowest 1 bit
- [[2022-05-27 Friday]] #Math #[[Bit Manipulation]] 
  problem:: Number of Steps to Reduce a Number to Zero
  link:: https://leetcode.com/problems/number-of-steps-to-reduce-a-number-to-zero/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 1
  id:: 628f9930-66fd-4055-89b8-636656551559
  collapsed:: true
	- easy simulation
	- it actually asked us to count the number of ones and zeros in binary representation
- [[2022-05-28 Saturday]] #Array #[[Hash Table]] #Math #[[Bit Manipulation]] #Sorting 
  problem:: Missing Number
  link:: https://leetcode.com/problems/missing-number/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 3
  id:: 62911709-6dbb-4f44-a02d-b5cc21f8f970
	- easy to solve by using XOR
- [[2022-05-29 Sunday]] #Array #String #[[Bit Manipulation]] 
  problem:: Maximum Product of Word Lengths
  link:: https://leetcode.com/problems/maximum-product-of-word-lengths/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 2
  id:: 6291813d-9e03-422b-8a91-baff14bc60a2
  collapsed:: true
	- construct a bit string for each string to represent its character appearance
	- use `AND` on two bit strings to test if two strings share common characters
- [[2022-05-30 Monday]] #Math #[[Bit Manipulation]] 
  problem:: Divide Two Integers
  link:: https://leetcode.com/problems/divide-two-integers/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62940b4e-de0c-44c4-aac0-b62d7259c028
  collapsed:: true
	- use bit manipulation to construct quotient one bit by one bit
		- find the most significant bit, calculate the new dividend and do it again
	- many edge cases to consider
- [[2022-05-31 Tuesday]] #[[Hash Table]] #String #[[Bit Manipulation]] #[[Rolling Hash]] #[[Hash Function]] 
  problem:: Check If a String Contains All Binary Codes of Size K
  link:: https://leetcode.com/problems/check-if-a-string-contains-all-binary-codes-of-size-k/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 1
  id:: 6294e002-75c4-473e-a9f3-1e178642090e
  collapsed:: true
	- calculate the value of each bit substring
	- use a hash table to record each value's appearance
	- be careful of how to remove the most significant bit from the current substring
- [Backspace String Compare](((53fa914e-9f58-47d5-9833-e48233aa6034))) can be solved using two pointers and looping backwards
- [Sort Array By Parity](((626f49e4-bf2a-43d8-be4f-5bcae9dca3d6))) is a classic two pointers problem
- [Shortest Unsorted Continuous Subarray](((626f4a46-c8bd-4730-8d13-60e1ce11a60e))) can be solved using two pointers in one pass, but doing it in multiple iteration can make the logic clearer
- [Max Number of K-Sum Pairs](((6271ccb9-4e85-4395-87f9-52e5bff5c17d))) can be solved using only hash table
- [Implement Stack using Queues](((62731d15-d128-4312-a7b2-9bd00879aec2))) can be solved using only one queue, we can mimic another queue's functionality with push the front number to the newly added number repeatedly
- [Remove All Adjacent Duplicates in String II](((6273c8ab-d031-46c0-8dab-018d19a44649))) has to be solved using stack, if we check the condition again each time  after we remove the current duplicate, we will get a TLE
- [132 Pattern](((62750fa8-fdeb-45f2-b1a0-c228cf876c25))) is a problem I failed to solve two times, definitely need to understand the concept
- [Flatten Nested List Iterator](((6275fa3f-00fc-4f93-9cfd-8619848d055d))) is a problem I struggled on the corner case for too long, need to make sure I understand the loop condition
- [Flatten Nested List Iterator](((62774118-84e3-47a7-a568-72bd110b2a65))) can be solved using backtracking, but instead of adding a new character to strings in the array at once, maintain a string and add a new character at once
- [Combination Sum III](((6279308f-d8c1-4199-b61a-6bcc25b5d7c6))) is a classic backtracking problem with two ending conditions
- [Count Sorted Vowel Strings](((627a9dae-3abd-4420-8f10-8b53eb3f7878))) is a problem that can be solved using dynamic programming, but solving it using math is faster
  id:: 627b0729-43d7-438a-be77-ffd47c242892
- [Permutations II](((627c52f5-8fbd-4eb2-a579-e8619f885873))) is a classic backtracking problem but with a small tweak, realize that we are constructing the final permutations element by element is the key to this problem
- [Populating Next Right Pointers in Each Node II](((627d27bd-1c12-4d55-a634-8807e73c3e77))) is a simple BFS problem, just need to traverse from the back in each level, it can also be solved using less space by recording previous node and next level's head node
- [Network Delay Time](((627e79b1-caf4-4a67-a4ef-cd1d6629ee8b))) can be solved using Dijkstra's algorithm
- [Deepest Leaves Sum](((627f1b1d-5f09-424f-9306-5ce88789c441))) is a simple BFS problem
- [Shortest Path in Binary Matrix](((62806396-955b-49b6-85df-67b321977911))) is a simple BFS problem, but need to be careful of when should we push adjacent cell into queue
- [Find a Corresponding Node of a Binary Tree in a Clone of That Tree](((6282efa4-9e46-4e47-b229-d68f38f72178))) is a simple DFS problem, using recursive approach may save some space comparing to using iterative approach
- [Unique Paths II](((628692c1-5a3b-4821-9291-cbb8ddbf837c))) is a simple DP problem
- [Coin Change](((6287afa9-df4f-4efe-9e08-10326f6f3edc))) is a classic knapsack problem, but it can also be solved using BFS with hash table
- [Palindromic Substrings](((628850df-caf5-4837-a60d-6f5dfcee91eb))) can be solved by expanding substrings from center
- [Ones and Zeroes](((62899e32-8b12-41dc-a1b0-d6ac8a28a4c9))) is a 0-1 knapsack problem with two constraints
- [Longest Valid Parentheses](((628bc42c-ddd7-4227-84bb-104e189288ee))) is a DP problem, and it can be solved in $O(n)$ time using stack
- [Number of 1 Bits](((628e3a1f-672e-4c07-b56a-654546cb6abe))) is easy to solve by shifting the number, we can also use $n\&(n-1)$ to save some time
- [Number of Steps to Reduce a Number to Zero](((628f9930-66fd-4055-89b8-636656551559))) is easy to solve by simulating the process, but counting the number of ones and zeros in binary representation can make the solution faster
- [Missing Number](((62911709-6dbb-4f44-a02d-b5cc21f8f970))) is easy to solve by iterating over the array and using XOR
  id:: 6291813f-2fc1-4c17-a745-87084d0da9fa
- [Maximum Product of Word Lengths](((6291813d-9e03-422b-8a91-baff14bc60a2))) is an easy bit manipulation problem
- [Divide Two Integers](((62940b4e-de0c-44c4-aac0-b62d7259c028))) can be solved by using bit manipulation, but has many edge cases to consider
- [Check If a String Contains All Binary Codes of Size K](((6294e002-75c4-473e-a9f3-1e178642090e))) can be solve by treating each substring as the binary representation of a number, and use a hash table to track their appearance