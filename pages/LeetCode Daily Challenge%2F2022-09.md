title:: LeetCode Daily Challenge/2022-09

- 4 easy, 17 medium, 2 hard
- 11 problems were solved for the first time
- [[2022-09-01 Thursday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Count Good Nodes in Binary Tree
  link:: https://leetcode.com/problems/count-good-nodes-in-binary-tree/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 6310a8b9-6a11-4e09-b2a0-10923ab59c61
	- use DFS and record the maximum value of the path along the way
- [[2022-09-02 Friday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Average of Levels in Binary Tree
  link:: https://leetcode.com/problems/average-of-levels-in-binary-tree/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 2
  id:: 6310a90a-2f42-4abb-b887-09c9acecf4ac
	- use BFS to calculate the sum of each level
- [[2022-09-03 Saturday]] #Backtracking #BFS 
  problem:: Numbers With Same Consecutive Differences
  link:: https://leetcode.com/problems/numbers-with-same-consecutive-differences/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63122521-2d5e-4bcd-b6f7-3d3b05958a25
	- use BFS
	- need to avoid duplicate when the difference is 0
- [[2022-09-04 Sunday]] #[[Hash Table]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Vertical Order Traversal of a Binary Tree
  link:: https://leetcode.com/problems/vertical-order-traversal-of-a-binary-tree/
  difficulty:: Hard
  duration:: 15 mins
  number_of_times:: 1
  id:: 6312b182-9dc6-4736-b607-5b3cd8f44a53
	- use BFS to traverse the node
	- store the row and the value of each node for each column
	- sort the column separately
	- because the column number may be negative, we need pre-allocate space and move index 0
- [[2022-09-05 Monday]] #Tree #BFS 
  problem:: N-ary Tree Level Order Traversal
  link:: https://leetcode.com/problems/n-ary-tree-level-order-traversal/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 2
  id:: 63140ad0-26ae-4899-a5a6-6c81731ba0d0
	- use DFS
	- need to consider empty tree case
- [[2022-09-06 Tuesday]] #Tree #DFS #[[Binary Tree]] 
  problem:: Binary Tree Pruning
  link:: https://leetcode.com/problems/binary-tree-pruning/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 631616d3-0ef5-4331-9d09-ce33811add31
	- use DFS
	- remove the subtrees first, then determine whether to remove the node
- [[2022-09-07 Wednesday]] #String #Tree #DFS #[[Binary Tree]] 
  problem:: Construct String from Binary Tree
  link:: https://leetcode.com/problems/construct-string-from-binary-tree/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 63172d03-7844-4317-9717-1bf6a830eddb
	- use DFS
	- need to insert a pair of empty parenthesis if there is a right subtree but no left subtree
- [[2022-09-08 Thursday]] #Stack #Tree #DFS #[[Binary Tree]] 
  problem:: Binary Tree Inorder Traversal
  link:: https://leetcode.com/problems/binary-tree-inorder-traversal/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 63188ab1-edae-492c-8ed3-abab74c7c919
	- use morris traversal
	- the key is to connect the last visited node in the left subtree to the current node, and be able to detect when we are back to current node
- [[2022-09-09 Friday]] #Array #Stack #Greedy #Sorting #[[Monotonic Stack]] 
  problem:: The Number of Weak Characters in the Game
  link:: https://leetcode.com/problems/the-number-of-weak-characters-in-the-game/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 1
  id:: 6319e31d-ab58-4cde-90dc-22b5fd1e0e6c
	- sort the array first
		- descending on attack, ascending on defense to avoid popping out element early
	- maintain a monotonic stack
		- for each level of attack, push at most one pair of property into the stack
	- check stack's top to see if it has the same level of attack
	- pop the stack until it's empty or the top has higher defense
- [[2022-09-12 Monday]] #Array #[[Two Pointers]] #Greedy #Sorting 
  problem:: Bag of Tokens
  link:: https://leetcode.com/problems/bag-of-tokens/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 631ba492-b016-48e4-a0d3-936213775c7c
	- sort the array then use two pointers
	- if playing a token facing down can let us play another token facing up, then we should play it
- [[2022-09-13 Tuesday]] #Array #[[Bit Manipulation]] 
  problem:: UTF-8 Validation
  link:: https://leetcode.com/problems/utf-8-validation/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 631f3b9a-0360-47bc-b3cc-42f671d87536
	- use bit masks to check each bytes
- [[2022-09-14 Wednesday]] #[[Bit Manipulation]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Pseudo-Palindromic Paths in a Binary Tree
  link:: https://leetcode.com/problems/pseudo-palindromic-paths-in-a-binary-tree/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63206d8a-d2d5-44c2-8a4e-b0c2172603d8
	- use DFS
	- pass the counting array to each child
- [[2022-09-15 Thursday]] #Array #[[Hash Table]] #Greedy #Sorting 
  problem:: Find Original Array From Doubled Array
  link:: https://leetcode.com/problems/find-original-array-from-doubled-array/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 6321c200-9d7e-4181-b8fd-d6417cec74fd
	- use sorting and a hash table
	- if we find a number that is half the value of the current number, then we can cancel each other out in the hash table
	- if we can't, then it's not a doubled array
	- be careful of the 0 case
- [[2022-09-18 Sunday]] #Array #[[Two Pointers]] #DP #Stack #[[Monotonic Stack]] 
  problem:: Trapping Rain Water
  link:: https://leetcode.com/problems/trapping-rain-water/
  difficulty:: Hard
  duration:: 30 mins
  number_of_times:: 1
  id:: 63233c7f-e22f-4993-ac93-b8b4baf05775
	- maintain a decreasing monotonic stack
	- every time we find a number that is greater than the number on top of the stack, we pop the number, and calculate how many water we can trap
- [[2022-09-19 Monday]] #Array #[[Hash Table]] #String 
  problem:: Find Duplicate File in System
  link:: https://leetcode.com/problems/find-duplicate-file-in-system/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 632684c3-d366-43d4-8d04-a2f659726020
	- use hash table
	- be careful of the `substr` method of strings
- [[2022-09-20 Tuesday]] #Array #[[Binary Search]] #DP #[[Sliding Window]] #[[Rolling Hash]] #[[Hash Function]] 
  problem:: Maximum Length of Repeated Subarray
  link:: https://leetcode.com/problems/maximum-length-of-repeated-subarray/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 2
  id:: 632891ce-e31c-465d-b035-34cf3da4b8e7
	- use DP
	- record the maximum length of repeated subarray ending at certain positions
- [[2022-09-21 Wednesday]] #Array #Simulation 
  problem:: Sum of Even Numbers After Queries
  link:: https://leetcode.com/problems/sum-of-even-numbers-after-queries/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63290dd5-f789-4a0d-a416-7a7e1fa2c2bd
	- maintain the sum of all even numbers in the array, and simulate the process
- [[2022-09-22 Thursday]] #[[Two Pointers]] #String 
  problem:: Reverse Words in a String III
  link:: https://leetcode.com/problems/reverse-words-in-a-string-iii/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 2
  id:: 632c5892-7b4f-471a-b061-ac476722cc26
	- use two pointers to modify the string in place
- [[2022-09-24 Saturday]] #Backtracking #Tree #DFS #[[Binary Tree]] 
  problem:: Path Sum II
  link:: https://leetcode.com/problems/path-sum-ii/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 632c8ce3-2cbe-45f1-9f8d-d4175659e83a
	- use DFS
	- need to handle leaf nodes carefully
- [[2022-09-25 Sunday]] #Array #[[Linked List]] #Design #Queue 
  problem:: Design Circular Queue
  link:: https://leetcode.com/problems/design-circular-queue/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 632e5522-9752-499b-9ee8-5b13447a850f
	- use two pointers
	- allocate one more space to separate empty and full case
- [[2022-09-26 Monday]] #Array #String #[[Union Find]] #Graph 
  problem:: Satisfiability of Equality Equations
  link:: https://leetcode.com/problems/satisfiability-of-equality-equations/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 632fa97a-7918-4e39-b17a-0f7aa1ad769f
	- use union find
	- merge all the nodes that should be equal, then check the nodes that should not be equal
- [[2022-09-28 Wednesday]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Remove Nth Node From End of List
  link:: https://leetcode.com/problems/remove-nth-node-from-end-of-list/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63319fa9-3266-453a-82e2-d7618f431a8f
	- use two pointers
	- move the fast pointer n steps forward first, then move two pointers until fast pointer reaches the end
- [[2022-09-29 Thursday]] #Array #[[Two Pointers]] #[[Binary Search]] #Sorting #Heap 
  problem:: Find K Closest Elements
  link:: https://leetcode.com/problems/find-k-closest-elements/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 633444dd-ebac-42e2-9f0d-a82e112e94c5
	- use a priority queue to store the absolute differences between the target and all the numbers
	- get the top k elements of the priority queue, and sort them base on their original values
-
- [Count Good Nodes in Binary Tree](((6310a8b9-6a11-4e09-b2a0-10923ab59c61))) is an easy DFS problem
- [Average of Levels in Binary Tree](((6310a90a-2f42-4abb-b887-09c9acecf4ac))) is an easy BFS/DFS problem
- [Numbers With Same Consecutive Differences](((63122521-2d5e-4bcd-b6f7-3d3b05958a25))) is an easy BFS problem
- [Vertical Order Traversal of a Binary Tree](((6312b182-9dc6-4736-b607-5b3cd8f44a53))) can be solved by using BFS, and remember to move index 0, because the column number may be negative
- [N-ary Tree Level Order Traversal](((63140ad0-26ae-4899-a5a6-6c81731ba0d0))) is an easy BFS/DFS problem
- [Binary Tree Pruning](((631616d3-0ef5-4331-9d09-ce33811add31))) is an easy DFS problem, remove the subtree first then remove the node
- [Construct String from Binary Tree](((63172d03-7844-4317-9717-1bf6a830eddb))) is an easy DFS problem
- [Binary Tree Inorder Traversal](((63188ab1-edae-492c-8ed3-abab74c7c919))) can be solved by using morris traversal, remember how to traverse from left subtree to current node, then to right subtree
- [The Number of Weak Characters in the Game](((6319e31d-ab58-4cde-90dc-22b5fd1e0e6c))) can be solved by using sorting and monotonic stack, remember not to push more than one pair of property with same level of attack into the stack
- [Bag of Tokens](((631ba492-b016-48e4-a0d3-936213775c7c))) can be solved by using sorting and two pointers
- [UTF-8 Validation](((631f3b9a-0360-47bc-b3cc-42f671d87536))) can be solved by using bit masks
- [Pseudo-Palindromic Paths in a Binary Tree](((63206d8a-d2d5-44c2-8a4e-b0c2172603d8))) can be solved by using DFS, and using bit manipulation can help saving space
- [Find Original Array From Doubled Array](((6321c200-9d7e-4181-b8fd-d6417cec74fd))) can be solved by sorting and hash table
- [Trapping Rain Water](((63233c7f-e22f-4993-ac93-b8b4baf05775))) can be solved by using monotonic stack, the key is to calculate the water we can trap using current number and the number on top of the stack
- [Find Duplicate File in System](((632684c3-d366-43d4-8d04-a2f659726020))) can be solved by using a hash table
- [Maximum Length of Repeated Subarray](((632891ce-e31c-465d-b035-34cf3da4b8e7))) can be solved by DP, which recode the maximum length of repeated subarray ending at certain positions
- [Sum of Even Numbers After Queries](((63290dd5-f789-4a0d-a416-7a7e1fa2c2bd))) is a simple simulation problem
- [Reverse Words in a String III](((632c5892-7b4f-471a-b061-ac476722cc26))) is an easy two pointers problem
- [Path Sum II](((632c8ce3-2cbe-45f1-9f8d-d4175659e83a))) can be solved by using DFS, but backtracking is more efficient
- [Design Circular Queue](((632e5522-9752-499b-9ee8-5b13447a850f))) can be solved by using two pointers
- [Satisfiability of Equality Equations](((632fa97a-7918-4e39-b17a-0f7aa1ad769f))) is an easy union find problem
- [Remove Nth Node From End of List](((63319fa9-3266-453a-82e2-d7618f431a8f))) can be solved in one pass using two pointers, the key is to maintain a gap of n steps between two pointers first, then move then until the fast pointer reaches the end
- [Find K Closest Elements](((633444dd-ebac-42e2-9f0d-a82e112e94c5))) can be solved by using priority queue