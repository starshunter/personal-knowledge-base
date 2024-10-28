title:: LeetCode Daily Challenge/2022-07

- 5 easy, 18 medium, 1 hard
- 10 problems were solved for the first time
- [[2022-07-01 Friday]] #Array #Greedy #Sorting 
  problem:: Maximum Units on a Truck
  link:: https://leetcode.com/problems/maximum-units-on-a-truck/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 62be46e4-5e8c-4c31-abaf-2fa1307d91e6
	- sort the array base on number of units per box
	- take the boxes from the front until you can't
- [[2022-07-02 Saturday]] #Array #Greedy #Sorting 
  problem:: Maximum Area of a Piece of Cake After Horizontal and Vertical Cuts
  link:: https://leetcode.com/problems/maximum-area-of-a-piece-of-cake-after-horizontal-and-vertical-cuts/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 62be4751-a793-4e80-90dd-fadade4b8710
	- find the maximum intervals horizontally and vertically, then multiply them
	- be careful of integer overflow issue
- [[2022-07-03 Sunday]] #Array #DP #Greedy 
  problem:: Wiggle Subsequence
  link:: https://leetcode.com/problems/wiggle-subsequence/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
  id:: 62bfae80-c0d6-414c-8d3d-b2c1fe20b45a
	- use two arrays to store the states of the sequence
	- use two level iteration, for every number, consider all the numbers in front of it
- [[2022-07-04 Monday]] #Array #Greedy 
  id:: 62c1dec8-6fce-426c-9307-96efc0d84406
  problem:: Candy
  link:: https://leetcode.com/problems/candy/
  difficulty:: Hard
  duration:: 15 mins
  number_of_times:: 1
	- scan from the left first to ensure higher rating children get more candies, then scan from the right to make sure the same thing
- [[2022-07-05 Tuesday]] #Array #[[Hash Table]] #[[Union Find]] 
  id:: 62c2f703-50cb-4348-8b5f-545c3d2402be
  problem:: Longest Consecutive Sequence
  link:: https://leetcode.com/problems/longest-consecutive-sequence/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
	- use a hash table to store all the numbers
	- for each number, find its root and update its sequence length
- [[2022-07-06 Wednesday]] #Math #DP #Recursion #Memoization 
  id:: 62c46710-7622-4d4c-9be9-1993e263d60f
  problem:: Fibonacci Number
  link:: https://leetcode.com/problems/fibonacci-number/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 1
	- easy DP problem
- [[2022-07-09 Saturday]] #Array #DP #Queue #[[Sliding Window]] #Heap #[[Monotonic Queue]] 
  problem:: Jump Game VI
  link:: https://leetcode.com/problems/jump-game-vi/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 1
  id:: 62c898a6-4f94-422c-8c5a-79947dec5da8
	- starting from the back
	- use multiset to maintain the order of the next k elements
	- remove only one element from multiset at a time
- [[2022-07-10 Sunday]] #Array #DP 
  problem:: Min Cost Climbing Stairs
  link:: https://leetcode.com/problems/min-cost-climbing-stairs/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 62c8d5e6-287b-4ea8-95f5-3d09f1add0b0
	- easy DP problem
- [[2022-07-11 Monday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Binary Tree Right Side View
  link:: https://leetcode.com/problems/binary-tree-right-side-view/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 62ca62ba-6001-456a-9ce0-9c439fdc9266
	- use DFS
	- record each node's depth in the stack
- [[2022-07-13 Wednesday]] #Tree #BFS #[[Binary Tree]] 
  problem:: Binary Tree Level Order Traversal
  link:: https://leetcode.com/problems/binary-tree-level-order-traversal/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 62cb6fbc-61a7-41aa-a8c9-b62121880102
	- easy DFS problem
	- can also be solved with BFS
- [[2022-07-14 Thursday]] #Array #[[Hash Table]] #[[Divide and Conquer]] #Tree #[[Binary Tree]] 
  problem:: Construct Binary Tree from Preorder and Inorder Traversal
  link:: https://leetcode.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 62cf659f-eaf2-4b11-bffd-25678d6802a5
	- the first element in preorder array is the current root
	- find the current root in inorder array
	- split the arrays base on how many element in front of the current root in the inorder array
- [[2022-07-15 Friday]] #Array #DFS #BFS #[[Union Find]] #Matrix 
  problem:: Max Area of Island
  link:: https://leetcode.com/problems/max-area-of-island/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62cf6615-c4a8-4efa-b858-20b7d1ae4103
	- easy DFS problem
- [[2022-07-16 Saturday]] #DP 
  problem:: Out of Boundary Paths
  link:: https://leetcode.com/problems/out-of-boundary-paths/
  difficulty:: Medium
  duration:: 25 mins
  number_of_times:: 1
  id:: 62d0b849-eff2-4045-bee3-e8b05e3c0c06
	- use a hash table to store how many ways to get to a position for a specific step
	- update the hash table for each step, and add the ways to go out of the boundaries
	- we can use a two dimensional array instead
- [[2022-07-19 Tuesday]] #Array #DP 
  problem:: Pascal's Triangle
  link:: https://leetcode.com/problems/pascals-triangle/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 3
  id:: 62d69a28-7080-487f-8248-ead0afde8fe0
	- easy DP problem
- [[2022-07-20 Wednesday]] #[[Hash Table]] #String #Trie #Sorting 
  problem:: Number of Matching Subsequences
  link:: https://leetcode.com/problems/number-of-matching-subsequences/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 62d69a5b-3242-4298-9bde-6741c03418f3
	- use two pointers to check the matching subsequences
	- use a hash table to record the occurrences of a string
- [[2022-07-22 Friday]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Partition List
  link:: https://leetcode.com/problems/partition-list/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62d95fc5-2178-45c0-978a-9fc695a25d54
	- use two pointers to construct two lists
- [[2022-07-24 Sunday]] #Array #[[Binary Search]] #[[Divide and Conquer]] #Matrix 
  problem:: Search a 2D Matrix II
  link:: https://leetcode.com/problems/search-a-2d-matrix-ii/
  difficulty:: Medium
  duration:: 3 mins
  number_of_times:: 3
  id:: 62d9f149-cc7f-461f-bf1f-fd5713b4758c
	- set the initial number with the number at the top right corner of the matrix
	- move it by comparing it with the target number
- [[2022-07-25 Monday]] #Array #[[Binary Search]] 
  problem:: Find First and Last Position of Element in Sorted Array
  link:: https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 62dca697-0c69-4881-b412-56d6fd6fce4c
	- do binary search twice
	- first one is normal, second one change the middle element to the second half of the subarray
	- need to check if the target exists after the first binary search
- [[2022-07-26 Tuesday]] #Tree #DFS #[[Binary Tree]] 
  problem:: Lowest Common Ancestor of a Binary Tree
  link:: https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 3
  id:: 62dec920-436f-47c4-bc95-2e8408d5c4e4
	- use DFS
	- could try iterative DFS next time
- [[2022-07-27 Wednesday]] #[[Linked List]] #Stack #Tree #DFS #[[Binary Tree]] 
  problem:: Flatten Binary Tree to Linked List
  link:: https://leetcode.com/problems/flatten-binary-tree-to-linked-list/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62dff766-507e-4823-9d4a-480a995abd2c
	- use recursion
	- flatten the left subtree first, save the right subtree, move the flatten left subtree to the right, and concatenate the right subtree to the right most child
- [[2022-07-28 Thursday]] #[[Hash Table]] #String #Sorting 
  problem:: Valid Anagram
  link:: https://leetcode.com/problems/valid-anagram/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 3
  id:: 62e08a0a-c7f6-4b92-b51f-8323cbd4c481
	- use hash table to record the appearance time of each character
- [[2022-07-29 Friday]] #Array #[[Hash Table]] #String 
  problem:: Find and Replace Pattern
  link:: https://leetcode.com/problems/find-and-replace-pattern/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 62e2a98a-bdb6-4e16-ba7c-202faf4718de
	- use two hash tables for every string to record the two way mapping
	- we can normalize a word and compare it to normalized pattern
- [[2022-07-30 Saturday]] #Array #[[Hash Table]] #String 
  problem:: Word Subsets
  link:: https://leetcode.com/problems/word-subsets/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 62e32f3a-8e5c-49c0-98fb-6c3bda8914b0
	- failed using two level iteration to check each string
	- use a hash table to record the maximum appearance of a character in `words2`
	- use the hash table to check the string in `words1`
- [[2022-07-31 Sunday]] #Array #Design #[[Binary Indexed Tree]] #[[Segment Tree]] 
  problem:: Range Sum Query - Mutable
  link:: https://leetcode.com/problems/range-sum-query-mutable/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 2
  id:: 62e49103-9944-447d-9066-13b0988d861d
	- construct a segment tree
- [Maximum Units on a Truck](((62be46e4-5e8c-4c31-abaf-2fa1307d91e6))) is an easy problem
- [Maximum Area of a Piece of Cake After Horizontal and Vertical Cuts](((62be4751-a793-4e80-90dd-fadade4b8710))) is a simple sorting problem
- [Wiggle Subsequence](((62bfae80-c0d6-414c-8d3d-b2c1fe20b45a))) can be solved in `O(n)` time
- [Candy](((62c1dec8-6fce-426c-9307-96efc0d84406))) is a greedy problem
- [Longest Consecutive Sequence](((62c2f703-50cb-4348-8b5f-545c3d2402be))) can be solved using a hash table
- [Fibonacci Number](((62c46710-7622-4d4c-9be9-1993e263d60f))) is a very easy problem
- [Jump Game VI](((62c898a6-4f94-422c-8c5a-79947dec5da8))) can be solved using monotonic queue, remove all the element from the queue that is smaller than the current element, so we can guarantee no older element will exist behind current element
- [Min Cost Climbing Stairs](((62c8d5e6-287b-4ea8-95f5-3d09f1add0b0))) is an easy DP problem
- [Binary Tree Right Side View](((62ca62ba-6001-456a-9ce0-9c439fdc9266))) is a simple DFS problem
- [Binary Tree Level Order Traversal](((62cb6fbc-61a7-41aa-a8c9-b62121880102))) is a simple DFS problem
- [Construct Binary Tree from Preorder and Inorder Traversal](((62cf659f-eaf2-4b11-bffd-25678d6802a5))) can be solved by recursively finding the current root in the  preorder array
- [Max Area of Island](((62cf6615-c4a8-4efa-b858-20b7d1ae4103))) is a simple DFS problem
- [Out of Boundary Paths](((62d0b849-eff2-4045-bee3-e8b05e3c0c06))) can be solved by updating a two dimensional array for every step
- [Pascal's Triangle](((62d69a28-7080-487f-8248-ead0afde8fe0))) is an easy DP problem
- [Number of Matching Subsequences](((62d69a5b-3242-4298-9bde-6741c03418f3))) is an easy two pointers problem, but we can use binary search to increase the efficiency
- [Partition List](((62d95fc5-2178-45c0-978a-9fc695a25d54))) is a simple two pointers problem
- [Search a 2D Matrix II](((62d9f149-cc7f-461f-bf1f-fd5713b4758c))) is easy to solve by comparing and moving the number at the top right corner
- [Find First and Last Position of Element in Sorted Array](((62dca697-0c69-4881-b412-56d6fd6fce4c))) can be solved by doing binary search two times, the second time should move the middle element in each round to the second half of the subarray
- [Lowest Common Ancestor of a Binary Tree](((62dec920-436f-47c4-bc95-2e8408d5c4e4))) could be solved using DFS to check the position of the targets relative to current node
- [Flatten Binary Tree to Linked List](((62dff766-507e-4823-9d4a-480a995abd2c))) can be solved by doing recursion on the left subtree first
- [Valid Anagram](((62e08a0a-c7f6-4b92-b51f-8323cbd4c481))) can be solved using hash table
- [Find and Replace Pattern](((62e2a98a-bdb6-4e16-ba7c-202faf4718de))) can be solved using two hash tables, but we can solve it with only one
- [Word Subsets](((62e32f3a-8e5c-49c0-98fb-6c3bda8914b0))) can be solved by maintaining a hash table that records the maximum appearance of a character among strings
- [Range Sum Query - Mutable](((62e49103-9944-447d-9066-13b0988d861d))) can be solved by using segment tree