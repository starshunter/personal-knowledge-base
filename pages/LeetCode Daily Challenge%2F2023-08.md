- 1 easy, 14 medium, 0 hard
- 3 problems were solved for the first time
- [[2023-08-02 Wednesday]] #Array #Backtracking 
  problem:: Permutations
  link:: https://leetcode.com/problems/permutations/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 64c99f93-0d58-4ca5-a7ac-deaf388a7e8f
	- use backtracking
	- swap the numbers' places so we don't need to move the index around
- [[2023-08-03 Thursday]] #[[Hash Table]] #String #Backtracking 
  problem:: Letter Combinations of a Phone Number
  link:: https://leetcode.com/problems/letter-combinations-of-a-phone-number/
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 4
  id:: 64c9a0a3-3aed-4b84-af66-acc764356bf2
	- simple backtracking problem
	- build the digits to characters mapping at the beginning
- [[2023-08-04 Friday]] #Array #[[Hash Table]] #String #DP #Trie #Memoization 
  problem:: Word Break
  link:: https://leetcode.com/problems/word-break/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 64caf0a0-0509-4b6d-9640-35d5a1a30ae4
	- use DP to check if we can construct the substring end with each character
- [[2023-08-05 Saturday]] #DP #Backtracking #Tree #[[Binary Search Tree]] #[[Binary Tree]] 
  problem:: Unique Binary Search Trees II
  link:: https://leetcode.com/problems/unique-binary-search-trees-ii/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 3
  id:: 64cc44f6-f780-4b04-9efd-62ed168acf87
	- use DP to construct all possible subtrees of every interval
- [[2023-08-07 Monday]] #Array #[[Binary Search]] #Matrix 
  problem:: Search a 2D Matrix
  link:: https://leetcode.com/problems/search-a-2d-matrix/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 64cf99ae-a620-4dee-aa4b-18f167ecca58
	- use one binary search to search in the matrix
- [[2023-08-08 Tuesday]] #Array #[[Binary Search]] 
  problem:: Search in Rotated Sorted Array
  link:: https://leetcode.com/problems/search-in-rotated-sorted-array/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 3
  id:: 64d035e5-15fa-4718-832d-8503fc7a21dd
	- decide which half the target is in by finding the half that has continuous values
- [[2023-08-10 Thursday]] #Array #[[Binary Search]] 
  problem:: Search in Rotated Sorted Array II
  link:: https://leetcode.com/problems/search-in-rotated-sorted-array-ii/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 3
  id:: 64d18a10-9245-45c4-ba0b-43b5c52a63ee
	- consider the special case that left, right and middle numbers are all the same
	- we can shrink both left and right in this case
	- then do the same procedure to find out which half is continuous
- [[2023-08-11 Friday]] #Array #DP 
  problem:: Coin Change II
  link:: https://leetcode.com/problems/coin-change-ii/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 64d42e0b-5967-4dce-8769-7709c543f792
	- use DP
	- to avoid duplicate combination, iterate over the coins
- [[2023-08-12 Saturday]] #Array #DP #Matrix 
  problem:: Unique Paths II
  link:: https://leetcode.com/problems/unique-paths-ii/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 64d58017-e9ee-4720-ba38-6a887d8b7152
	- use one array to do DP
- [[2023-08-13 Sunday]] #Array #DP 
  problem:: Check if There is a Valid Partition For The Array
  link:: https://leetcode.com/problems/check-if-there-is-a-valid-partition-for-the-array/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 64d6d451-8538-46b6-918f-0a5d75c13128
	- easy DP problem
	- need to make sure we don't go out of bound
- [[2023-08-14 Monday]] #Array #[[Divide and Conquer]] #Sorting #Heap #[[Priority Queue]] #[[Quick Select]] 
  problem:: Kth Largest Element in an Array
  link:: https://leetcode.com/problems/kth-largest-element-in-an-array/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 4
  id:: 64d8271d-cf5a-421f-a300-944f61f59a26
	- use quick select
- [[2023-08-17 Thursday]] #Array #DP #BFS #Matrix 
  problem:: 01 Matrix
  link:: https://leetcode.com/problems/01-matrix/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 64d9716c-6382-4cbd-bf31-ac5860fd18e6
	- iterate the matrix two times to do the DP
	- first count from top left, then count from bottom right
- [[2023-08-18 Friday]] #Graph 
  id:: 64dd6593-5193-452a-9aed-daa3d73680c1
  problem:: Maximal Network Rank
  link:: https://leetcode.com/problems/maximal-network-rank/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
	- count the connected edges for each nodes
	- build a graph base on the edges
- [[2023-08-26 Saturday]] #Array #DP #Greedy #Sorting 
  problem:: Maximum Length of Pair Chain
  link:: https://leetcode.com/problems/maximum-length-of-pair-chain/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 64debaf8-4f95-41fd-85d8-046a5693c9bb
	- sort the array by the first number of each pair
	- use greedy to see if we can take the current pair as the end of the pair
- [[2023-08-28 Monday]] #Stack #Design #Queue 
  problem:: Implement Stack using Queues
  link:: https://leetcode.com/problems/implement-stack-using-queues/description/
  difficulty:: Easy
  duration:: 5 mins
  number-of-times:: 3
  id:: 64e9451e-9958-4b60-867a-087515d7987a
	- make sure the latest number stay at the front of the queue every time doing push operation
-
- [Permutations](((64c99f93-0d58-4ca5-a7ac-deaf388a7e8f))) can be solved by using backtracking and swapping target number to current position
- [Letter Combinations of a Phone Number](((64c9a0a3-3aed-4b84-af66-acc764356bf2))) can be solved by backtracking
- [Word Break](((64caf0a0-0509-4b6d-9640-35d5a1a30ae4))) can be solved by DP
- [Unique Binary Search Trees II](((64cc44f6-f780-4b04-9efd-62ed168acf87))) can be solved by using DP to find every subtree in every interval
- [Search a 2D Matrix](((64cf99ae-a620-4dee-aa4b-18f167ecca58))) can be solved by doing one binary search
- [Search in Rotated Sorted Array](((64d035e5-15fa-4718-832d-8503fc7a21dd))) can be solved by finding the continuous half before every binary search iteration
- [Search in Rotated Sorted Array II](((64d18a10-9245-45c4-ba0b-43b5c52a63ee))) can be solved by first handling the special case of all three pointers have the same number, then proceed to find which half is continuous
- [Coin Change II](((64d42e0b-5967-4dce-8769-7709c543f792))) can be solved by DP and iterate through different kinds of coins
- [Unique Paths II](((64d58017-e9ee-4720-ba38-6a887d8b7152))) is a simple DP problem
- [Check if There is a Valid Partition For The Array](((64d6d451-8538-46b6-918f-0a5d75c13128))) is an easy DP problem
- [Kth Largest Element in an Array](((64d8271d-cf5a-421f-a300-944f61f59a26))) is a classic quick select problem
- [01 Matrix](((64d9716c-6382-4cbd-bf31-ac5860fd18e6))) can be solved by using DP from two cornors
- [Maximal Network Rank](((64dd6593-5193-452a-9aed-daa3d73680c1))) is an easy graph problem
- [Maximum Length of Pair Chain](((64debaf8-4f95-41fd-85d8-046a5693c9bb))) can be solved by sorting the array first then use greedy
- [Implement Stack using Queues](((64e9451e-9958-4b60-867a-087515d7987a))) can be solved by maintaining stack property when doing push operation