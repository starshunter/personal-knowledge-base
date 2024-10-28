- 4 easy, 11 medium, 0 hard
- 11 problems were solved for the first time
- [[2023-06-02 Friday]] #Array #Math #DFS #BFS #Graph #Geometry 
  problem:: Detonate the Maximum Bombs
  link:: https://leetcode.com/problems/detonate-the-maximum-bombs/description/
  difficulty:: medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 6479375b-db1f-4fdf-9697-f79d8d2a222b
	- it's a graph problem, so construct the graph first
	- use DFS to find the maximum number of node we can get to starting from one node
- [[2023-06-03 Saturday]] #Tree #DFS #BFS 
  problem:: Time Needed to Inform All Employees
  link:: https://leetcode.com/problems/time-needed-to-inform-all-employees/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 647937c3-aa60-4488-b6df-0d50a782736c
	- use BFS
	- need to know the time each employee learn the news
- [[2023-06-04 Sunday]] #DFS #BFS #[[Union Find]] #Graph 
  problem:: Number of Provinces
  link:: https://leetcode.com/problems/number-of-provinces/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 3
  id:: 647a8b73-a1a1-4bcf-85b9-6ef4bbce6899
	- use union find
- [[2023-06-05 Monday]] #Array #Math #Geometry 
  problem:: Check If It Is a Straight Line
  link:: https://leetcode.com/problems/check-if-it-is-a-straight-line/description/
  difficulty:: Easy
  duration:: 10 mins
  number-of-times:: 1
  id:: 647bd73c-870f-4117-89e2-f78a9395fd9a
	- find the slope of the line
	- need to avoid divide by zero
	- make vertical line a special case
- [[2023-06-08 Thursday]] #Array #[[Binary Search]] #Matrix 
  problem:: Count Negative Numbers in a Sorted Matrix
  link:: https://leetcode.com/problems/count-negative-numbers-in-a-sorted-matrix/description/
  difficulty:: Easy
  duration:: 2 mins
  number-of-times:: 1
  id:: 647d2a80-0268-459e-b452-f693263de46f
	- easy counting problem
- [[2023-06-09 Friday]] #Array #[[Binary Search]] 
  problem:: Find Smallest Letter Greater Than Target
  link:: https://leetcode.com/problems/find-smallest-letter-greater-than-target/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 64811e8f-2ef5-4c6a-8026-e6cd2ec2a5a9
	- easy binary search problem
- [[2023-06-11 Sunday]] #Array #[[Hash Table]] #[[Binary Search]] #Design 
  problem:: Snapshot Array
  link:: https://leetcode.com/problems/snapshot-array/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 64826f4f-84bb-4630-b776-75fffae463a5
	- only store a position's value when it changes
	- use binary search to find the answer
- [[2023-06-12 Monday]] #Array 
  problem:: Summary Ranges
  link:: https://leetcode.com/problems/summary-ranges/description/
  difficulty:: Easy
  duration:: 10 mins
  number-of-times:: 3
  id:: 64851a4e-eed6-4eb7-a6f8-76c3d3b0a5c9
	- append the last number to avoid repeated code
	- be careful of integer overflow
- [[2023-06-13 Tuesday]] #Array #[[Hash Table]] #Matrix #Simulation #Trie 
  problem:: Equal Row and Column Pairs
  link:: https://leetcode.com/problems/equal-row-and-column-pairs/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 6486634c-4f95-4455-a770-4b6ebb1d477a
	- use tree map
	- can be solved by trie
- [[2023-06-14 Wednesday]] #Tree #DFS #BFS #[[Binary Search Tree]] #[[Binary Tree]] #[[In-order Traversal]] 
  id:: 6487b788-c12b-4ba8-af2f-54b619f32777
  problem:: Minimum Absolute Difference in BST
  link:: https://leetcode.com/problems/minimum-absolute-difference-in-bst/description/
  difficulty:: Easy
  duration:: 5 mins
  number-of-times:: 2
	- use in-order traversal
- [[2023-06-20 Tuesday]] #Array #[[Sliding Window]] 
  problem:: K Radius Subarray Averages
  link:: https://leetcode.com/problems/k-radius-subarray-averages/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 64890671-3761-4912-8c69-544939173363
	- easy sliding window problem
- [[2023-06-22 Thursday]] #Array #DP #Greedy 
  problem:: Best Time to Buy and Sell Stock with Transaction Fee
  link:: https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 2
  id:: 6490efda-b0ba-4f0e-ae35-77da562bfebf
	- maintain buy state and sell state
- [[2023-06-23 Friday]] #Array #[[Hash Table]] #[[Binary Search]] #DP 
  problem:: Longest Arithmetic Subsequence
  link:: https://leetcode.com/problems/longest-arithmetic-subsequence/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 6493961d-b528-43ee-bb50-380a2e8c0b8e
	- use DP with hash table
- [[2023-06-26 Monday]] #Array #[[Two Pointers]] #Heap #[[Priority Queue]] #Simulation 
  problem:: Total Cost to Hire K Workers
  link:: https://leetcode.com/problems/total-cost-to-hire-k-workers/description/
  difficulty:: Medium
  duration:: 15 mins
  number-of-times:: 1
  id:: 6495965a-1568-4b4d-83c5-b61f6c833484
	- use two priority queues
	- use two pointers to check if we need to push new numbers into queues
	- be careful of putting the same numbers into different queues
- [[2023-06-27 Tuesday]] #Array #Heap #[[Priority Queue]] 
  problem:: Find K Pairs with Smallest Sums
  link:: https://leetcode.com/problems/find-k-pairs-with-smallest-sums/description/
  difficulty:: Medium
  duration:: 30 mins
  number-of-times:: 2
  id:: 6498db89-3d74-4363-b0cc-b787cd18e11d
	- use a min queue, and push every pair with a number from the first array and the first number in the second array into it
	- every time we get a pair from the queue, push the next pair with the same number from first array into the queue
	- we can reduce the memory usage by only pushing the minimum pair at the beginning
-
- [Detonate the Maximum Bombs](((6479375b-db1f-4fdf-9697-f79d8d2a222b))) can be solved by constructing graph and use DFS
- [Time Needed to Inform All Employees](((647937c3-aa60-4488-b6df-0d50a782736c))) can be solved by using BFS
- [Number of Provinces](((647a8b73-a1a1-4bcf-85b9-6ef4bbce6899))) is an easy union find problem
- [Check If It Is a Straight Line](((647bd73c-870f-4117-89e2-f78a9395fd9a))) can be solved by finding the slope of the line first
- [Count Negative Numbers in a Sorted Matrix](((647d2a80-0268-459e-b452-f693263de46f))) is an very easy problem
- [Find Smallest Letter Greater Than Target](((64811e8f-2ef5-4c6a-8026-e6cd2ec2a5a9))) is an easy binary search problem
- [Snapshot Array](((64826f4f-84bb-4630-b776-75fffae463a5))) can be solved by using hash table and binary search
- [Summary Ranges](((64851a4e-eed6-4eb7-a6f8-76c3d3b0a5c9))) is an easy problem
- [Equal Row and Column Pairs](((6486634c-4f95-4455-a770-4b6ebb1d477a))) can be solved by tree map or trie
- [Minimum Absolute Difference in BST](((6487b788-c12b-4ba8-af2f-54b619f32777))) is an easy in-order traversal problem
- [K Radius Subarray Averages](((64890671-3761-4912-8c69-544939173363))) is an easy sliding window problem
- [Best Time to Buy and Sell Stock with Transaction Fee](((6490efda-b0ba-4f0e-ae35-77da562bfebf))) can be solved by using DP and maintain two states
- [Longest Arithmetic Subsequence](((6493961d-b528-43ee-bb50-380a2e8c0b8e))) can be solved by using DP and hash table
- [Total Cost to Hire K Workers](((6495965a-1568-4b4d-83c5-b61f6c833484))) can be solved by using two priority queues and two pointers, but need to remember not to put the same numbers into different queues
- [Find K Pairs with Smallest Sums](((6498db89-3d74-4363-b0cc-b787cd18e11d))) can be solved by using priority queue to store the pairs with a number from first array and first number from second array