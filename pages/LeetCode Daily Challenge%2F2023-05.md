- 5 easy, 12 medium, 0 hard
- 11 problems were solved for the first time
- [[2023-05-01 Monday]] #Array #Sorting 
  problem:: Average Salary Excluding the Minimum and Maximum Salary
  link:: https://leetcode.com/problems/average-salary-excluding-the-minimum-and-maximum-salary/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 644f0326-c998-4374-9652-d985722244f7
	- easy
- [[2023-05-02 Tuesday]] #Array #Math 
  problem:: Sign of the Product of an Array
  link:: https://leetcode.com/problems/sign-of-the-product-of-an-array/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 644f034b-4d51-45dd-bf8c-4b5c3b2a607a
	- easy
- [[2023-05-03 Wednesday]] #Array #[[Hash Table]] 
  problem:: Find the Difference of Two Arrays
  link:: https://leetcode.com/problems/find-the-difference-of-two-arrays/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 64505491-d4ad-4609-ac20-c7576ff1a3c1
	- use two hash tables to find the difference
- [[2023-05-04 Thursday]] #String #Greedy #Queue 
  problem:: Dota2 Senate
  link:: https://leetcode.com/problems/dota2-senate/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 6451ab19-f886-46c3-b8e1-7e59cb2c5132
	- use two queues with greedy
	- always choose to pop the other queue's front element
	- need to increase current element's index and push it to the back
- [[2023-05-05 Friday]] #String #[[Sliding Window]] 
  problem:: Maximum Number of Vowels in a Substring of Given Length
  link:: https://leetcode.com/problems/maximum-number-of-vowels-in-a-substring-of-given-length/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 6452fa04-c95d-44b3-9aa5-6608fed997f2
	- use sliding window
- [[2023-05-06 Saturday]] #Array #[[Two Pointers]] #[[Binary Search]] #Sorting 
  problem:: Number of Subsequences That Satisfy the Given Sum Condition
  link:: https://leetcode.com/problems/number-of-subsequences-that-satisfy-the-given-sum-condition/description/
  difficulty:: Medium
  duration:: 15 mins
  number-of-times:: 1
  id:: 64544bbd-0a32-4e2d-b663-edf1253afd29
	- it's asking for subsequence, so we can sort the array first
	- for each element, find the maximum element that satisfy the condition, and calculate the number of possible subsequences using the elements in between
- [[2023-05-08 Monday]] #Array #Matrix 
  problem:: Matrix Diagonal Sum
  link:: https://leetcode.com/problems/matrix-diagonal-sum/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 6455bd05-101c-4d5e-a95b-a72fe590ba6e
	- easy
- [[2023-05-10 Wednesday]] #Array #Matrix #Simulation 
  problem:: Spiral Matrix II
  link:: https://leetcode.com/problems/spiral-matrix-ii/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 4
  id:: 64583cc7-868c-45c0-aa63-1820e334a6ba
	- simulate the process
- [[2023-05-12 Friday]] #Array #DP 
  problem:: Solving Questions With Brainpower
  link:: https://leetcode.com/problems/solving-questions-with-brainpower/description/
  difficulty:: Medium
  duration:: 15 mins
  number-of-times:: 1
  id:: 645ae2cb-6f05-43ca-8844-b17c9e86ce82
	- use DP
	- find the maximum point we can get by solving the current question
	- update the base score of the next question we can solve
	- record the maximum score we  can get by skipping the current question
- [[2023-05-13 Saturday]] #DP 
  problem:: Count Ways To Build Good Strings
  link:: https://leetcode.com/problems/count-ways-to-build-good-strings/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 645d8ab0-1cfd-4752-8b37-05bfc3f90375
	- use DP
	- for every length calculate how many possible string end with certain number
- [[2023-05-15 Monday]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Swapping Nodes in a Linked List
  link:: https://leetcode.com/problems/swapping-nodes-in-a-linked-list/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 645f86d4-d622-4e74-9aa9-bc51818dab84
	- find the length of the list first
	- find the nodes we want to swap values
- [[2023-05-16 Tuesday]] #[[Linked List]] #Recursion 
  problem:: Swap Nodes in Pairs
  link:: https://leetcode.com/problems/swap-nodes-in-pairs/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 4
  id:: 646179c2-493b-40d0-a0fe-caa1175e0885
	- continue to swap pairs of nodes
	- need to have the nodes before and after the pair in advance
- [[2023-05-17 Wednesday]] #[[Linked List]] #[[Two Pointers]] #Stack 
  problem:: Maximum Twin Sum of a Linked List
  link:: https://leetcode.com/problems/maximum-twin-sum-of-a-linked-list/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 6462ca6b-1dc3-42d7-9e53-26c2ad33583f
	- find the length first
	- change the direction of the first half of the list
	- find the maximum pair in the second half
- [[2023-05-19 Friday]] #DFS #BFS #[[Union Find]] #Graph 
  problem:: Is Graph Bipartite?
  link:: https://leetcode.com/problems/is-graph-bipartite/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 64664f0d-d680-4d9f-838a-dfdd84243cae
	- use DFS
- [[2023-05-22 Monday]] #Array #[[Hash Table]] #[[Divide and Conquer]] #Sorting #Heap #[[Priority Queue]] #[[Bucket Sort]] #Counting #[[Quick Select]] 
  problem:: Top K Frequent Elements
  link:: https://leetcode.com/problems/top-k-frequent-elements/description/
  difficulty:: Medium
  duration:: 25 misn
  number-of-times:: 5
  id:: 6466c074-04fa-4155-8eb8-b99d8bb82b0c
	- use quick select
	- if we move the numbers that are smaller than the pivot to second half, then we need to shrink the range to exclude the pivot if the current number of top numbers is smaller than k
- [[2023-05-29 Monday]] #Design #Simulation #Counting 
  problem:: Design Parking System
  link:: https://leetcode.com/problems/design-parking-system/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 646ab9df-eeb9-46c1-9b63-0519f3ceb29f
	- very easy problem
- [[2023-05-31 Wednesday]] #[[Hash Table]] #String #Design 
  problem:: Design Underground System
  link:: https://leetcode.com/problems/design-underground-system/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 2
  id:: 6473edbc-7646-4566-a80a-069d0fb1d238
	- use two hash tables, one for passenger, another for station pair
-
- [Average Salary Excluding the Minimum and Maximum Salary](((644f0326-c998-4374-9652-d985722244f7))) is a very easy problem
- [Sign of the Product of an Array](((644f034b-4d51-45dd-bf8c-4b5c3b2a607a))) is a very easy problem
- [Find the Difference of Two Arrays](((64505491-d4ad-4609-ac20-c7576ff1a3c1))) can be solved using two hash tables
- [Dota2 Senate](((6451ab19-f886-46c3-b8e1-7e59cb2c5132))) can be solved by using two queues and always popping the other queue's front element
- [Maximum Number of Vowels in a Substring of Given Length](((6452fa04-c95d-44b3-9aa5-6608fed997f2))) is an easy sliding window problem
- [Number of Subsequences That Satisfy the Given Sum Condition](((64544bbd-0a32-4e2d-b663-edf1253afd29))) can be solved by using two pointers to find each pair of minimum and maximum elements
- [Matrix Diagonal Sum](((6455bd05-101c-4d5e-a95b-a72fe590ba6e))) is a very easy problem
- [Spiral Matrix II](((64583cc7-868c-45c0-aa63-1820e334a6ba))) can be solved by simulating the processing of filling numbers into the matrix
- [Solving Questions With Brainpower](((645ae2cb-6f05-43ca-8844-b17c9e86ce82))) can be solved by using DP to calculate the maximum score we can get by solving the current question
- [Count Ways To Build Good Strings](((645d8ab0-1cfd-4752-8b37-05bfc3f90375))) can be solved by using dynamic programming
- [Swapping Nodes in a Linked List](((645f86d4-d622-4e74-9aa9-bc51818dab84))) can be solved by using two pointers to do it in one pass
- [Swap Nodes in Pairs](((646179c2-493b-40d0-a0fe-caa1175e0885))) can be solved by swapping each pair of nodes in sequence
- [Maximum Twin Sum of a Linked List](((6462ca6b-1dc3-42d7-9e53-26c2ad33583f))) can be solved by using two pointers to find the half point, and change the direction of the list in the first half
- [Is Graph Bipartite?](((64664f0d-d680-4d9f-838a-dfdd84243cae))) is a simple DFS problem, but we can solve it by using union find, union the nodes adjacent to a given node
- [Top K Frequent Elements](((6466c074-04fa-4155-8eb8-b99d8bb82b0c))) can be solved by quick select, the way to shrink the range is a little complicated
  id:: 646ab9e2-4d2e-4a0e-9e44-2e9b01f939a2
- [Design Parking System](((646ab9df-eeb9-46c1-9b63-0519f3ceb29f))) is a very easy problem
- [Design Underground System](((6473edbc-7646-4566-a80a-069d0fb1d238))) can be solved by using two hash tables