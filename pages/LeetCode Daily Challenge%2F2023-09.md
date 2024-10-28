- 6 easy, 10 medium, 0 hard
- 2 problems were solved for the first time
- [[2023-09-01 Friday]] #DP #[[Bit Manipulation]] 
  problem:: Counting Bits
  link:: https://leetcode.com/problems/counting-bits/description/
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 4
  id:: 64f12bd4-61f5-4c10-8761-ca8be2841693
	- find the first unset bit for current number, every bit before it will be unset in the next number
- [[2023-09-03 Sunday]] #Math #DP #Combinatorics 
  problem:: Unique Paths
  link:: https://leetcode.com/problems/unique-paths/
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 5
  id:: 64f12cc5-a05f-420a-85a3-9da1604f5bd3
	- use math
	- avoid integer overflow
- [[2023-09-04 Monday]] #[[Hash Table]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Linked List Cycle
  link:: https://leetcode.com/problems/linked-list-cycle/description/?envType=daily-question&envId=2023-09-04
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 3
  id:: 64f4af0a-f9f5-4803-84e9-a442e9816291
	- use two pointers
	- check if both pointers are valid
- [[2023-09-05 Tuesday]] #[[Hash Table]] #[[Linked List]] 
  problem:: Copy List with Random Pointer
  link:: https://leetcode.com/problems/copy-list-with-random-pointer/description/?envType=daily-question&envId=2023-09-05
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 3
  id:: 64f5208c-fd08-4682-9e23-b9b0a8888a6d
	- use 3 iterations to achieve the deep copy
	- first iteration to create new nodes, and point original nodes' next pointer to them
	- second iteration to link copied nodes' random pointer
	- third iteration to link copied nodes' next pointer
	- remember to reverse the changes on original nodes
- [[2023-09-07 Thursday]] #[[Linked List]] 
  problem:: Reverse Linked List II
  link:: https://leetcode.com/problems/reverse-linked-list-ii/description/?envType=daily-question&envId=2023-09-07
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 3
  id:: 64f674c9-6cd0-488f-954f-71f2c87dda03
	- record the start of the interval, and move other nodes to its front
- [[2023-09-08 Friday]] #Array #DP 
  problem:: Pascal's Triangle
  link:: https://leetcode.com/problems/pascals-triangle/description/?envType=daily-question&envId=2023-09-08
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 4
  id:: 64f917f1-0171-471b-807d-efd8bd704453
	- easy DP problem
- [[2023-09-09 Saturday]] #Array #DP 
  problem:: Combination Sum IV
  link:: https://leetcode.com/problems/combination-sum-iv/description/?envType=daily-question&envId=2023-09-09
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 64fa6599-fb0e-408b-a089-5381faeca4f0
	- simple DP problem
	- use `unsigned int` because its overflow behavior is defined
- [[2023-09-11 Monday]] #Array #[[Hash Table]] 
  problem:: Group the People Given the Group Size They Belong To
  link:: https://leetcode.com/problems/group-the-people-given-the-group-size-they-belong-to/description/?envType=daily-question&envId=2023-09-11
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 64fbbaca-eca4-40b6-9322-d3826e95400b
	- use a hash table to keep track of groups with each size
- [[2023-09-15 Friday]] #Array #[[Union Find]] #Graph #[[Minimum Spanning Tree]] 
  problem:: Min Cost to Connect All Points
  link:: https://leetcode.com/problems/min-cost-to-connect-all-points/description/?envType=daily-question&envId=2023-09-15
  difficulty:: Medium
  duration:: 15 mins
  number-of-times:: 2
  id:: 64fe5c86-b45f-43ca-9c62-de049cf23b80
	- implement [[Kruskal's Algorithm]]
		- add minimum edges to the set if the nodes are not connected
	- use [[Union Find]] to decide if two nodes are connected
- [[2023-09-18 Monday]] #Array #[[Binary Search]] #Sorting #Heap #[[Priority Queue]] #Matrix 
  problem:: The K Weakest Rows in a Matrix
  link:: https://leetcode.com/problems/the-k-weakest-rows-in-a-matrix/description/
  difficulty:: Medium
  duration:: 15 mins
  number-of-times:: 2
  id:: 6503a652-17da-475d-afe2-67c58b19a24c
	- use binary search to find the strength of each row
	- use max heap to store the weakest rows
	- reverse the output
- [[2023-09-19 Tuesday]] #Array #[[Two Pointers]] #[[Binary Search]] #[[Bit Manipulation]] 
  problem:: Find the Duplicate Number
  link:: https://leetcode.com/problems/find-the-duplicate-number/description/?envType=daily-question&envId=2023-09-19
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 4
  id:: 6507991d-577e-4c02-a0cd-f323c8ebfb3f
	- use the number as the next index to move, and do cycle detection
	- a duplicate number guarantee we will enter a cycle
	- after two pointers meet, reset the fast pointer to the beginning and move them in the same speed
- [[2023-09-20 Wednesday]] #Array #[[Hash Table]] #[[Binary Search]] #[[Sliding Window]] #[[Prefix Sum]] 
  problem:: Minimum Operations to Reduce X to Zero
  link:: https://leetcode.com/problems/minimum-operations-to-reduce-x-to-zero/description/?envType=daily-question&envId=2023-09-20
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 6508e91c-8801-400b-ab7e-7e4014a3a77b
	- find the target that needs to remain after the operations first
	- use a hash table to store the prefix sum and its index
	- for each index, find if there's a prefix sum in the hash table that could get us to the target
- [[2023-09-23 Saturday]] #Array #[[Hash Table]] #[[Two Pointers]] #String #DP 
  problem:: Longest String Chain
  link:: https://leetcode.com/problems/longest-string-chain/description/?envType=daily-question&envId=2023-09-23
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 650a3b5a-4af8-44dd-a5af-0fe89a137f76
	- sort the array by string length first
	- for each string, find its possible predecessor
	- use a hash table to record the length of all possible chains, with the last word as key
- [[2023-09-24 Sunday]] #DP 
  problem:: Champagne Tower
  link:: https://leetcode.com/problems/champagne-tower/description/?envType=daily-question&envId=2023-09-24
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 650e31ad-81ca-4f4b-b80c-3a568fa9b79f
	- simple DP problem
	- for each row, count how many water will pour down from each glass
- [[2023-09-25 Monday]] #[[Hash Table]] #String #[[Bit Manipulation]] #Sorting 
  problem:: Find the Difference
  link:: https://leetcode.com/problems/find-the-difference/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 4
  id:: 650f83f7-5d8f-41a0-9ee8-b26edcb34a25
	- use XOR operation
- [[2023-09-29 Friday]] #Array 
  problem:: Monotonic Array
  link:: https://leetcode.com/problems/monotonic-array/description/?envType=daily-question&envId=2023-09-29
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 1
  id:: 6510cf39-c076-4263-8d84-150fdbc6c820
	- easy
	- consecutive same number won't affect monotonic property
-
- [Counting Bits](((64f12bd4-61f5-4c10-8761-ca8be2841693))) can be solved by finding the first unset bit for a number
- [Unique Paths](((64f12cc5-a05f-420a-85a3-9da1604f5bd3))) is a simple math problem
- [Linked List Cycle](((64f4af0a-f9f5-4803-84e9-a442e9816291))) is an easy two pointers problem
- [Copy List with Random Pointer](((64f5208c-fd08-4682-9e23-b9b0a8888a6d))) can be solved by constructing the deep copy list in three iterations
- [Reverse Linked List II](((64f674c9-6cd0-488f-954f-71f2c87dda03))) can be solved by moving the nodes to the beginning of the reverse range
- [Pascal's Triangle](((64f917f1-0171-471b-807d-efd8bd704453))) is a very easy DP problem
- [Combination Sum IV](((64fa6599-fb0e-408b-a089-5381faeca4f0))) is a simple DP problem
- [Group the People Given the Group Size They Belong To](((64fbbaca-eca4-40b6-9322-d3826e95400b))) is an easy hash table problem
- [Min Cost to Connect All Points](((64fe5c86-b45f-43ca-9c62-de049cf23b80))) can be solved by using [[Kruskal's Algorithm]] to get the [[Minimum Spanning Tree]]
- [The K Weakest Rows in a Matrix](((6503a652-17da-475d-afe2-67c58b19a24c))) can be solved by using max heap and binary search
- [Find the Duplicate Number](((6507991d-577e-4c02-a0cd-f323c8ebfb3f))) can be solved by using cycle detection
- [Minimum Operations to Reduce X to Zero](((6508e91c-8801-400b-ab7e-7e4014a3a77b))) can be solved by using prefix sum and hash table, use hash table to store  prefix sum and its index
- [Longest String Chain](((650a3b5a-4af8-44dd-a5af-0fe89a137f76))) can be solved by sorting the array with string length first, and use hash table to store the length of all possible chains
- [Champagne Tower](((650e31ad-81ca-4f4b-b80c-3a568fa9b79f))) is a simple DP problem
- [Find the Difference](((650f83f7-5d8f-41a0-9ee8-b26edcb34a25))) is a simple bit manipulation problem
- [Monotonic Array](((6510cf39-c076-4263-8d84-150fdbc6c820))) is a very easy problem