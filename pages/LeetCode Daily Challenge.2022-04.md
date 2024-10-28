- 10 easy, 20 medium, 0 hard
- 17 problems were solved for the first time
-
- [[2022-04-01 Friday]] #[[Two Pointers]] #String #Recursion
  id:: baf21642-c5c9-497e-a1f2-74c4b336b3b4
  collapsed:: true
	- problem:: Reverse String
	  link:: https://leetcode.com/problems/reverse-string/
	  difficulty:: Easy
	  duration:: 1 min
	- third time solving this problem
	- easy, not much to say
- [[2022-04-02 Saturday]] #[[Two Pointers]] #String #Greedy
  id:: de429926-6076-4b1c-ba9b-050b51a6e9a5
  collapsed:: true
	- problem:: Valid Palindrome II
	  link:: https://leetcode.com/problems/valid-palindrome-ii/
	  difficulty:: Easy 
	  duration:: 10 mins
	- first time solving this problem
	- tried to solve it with simple conditions but failed
	- use recursion instead
	- when we encounter two different characters, try both way of deleting one character
- [[2022-04-03 Sunday]] #Array
  id:: d4167fbd-dbda-4a1f-8c08-1c30b1f12ddd
  collapsed:: true
	- problem:: Next Permutation
	  link:: https://leetcode.com/problems/next-permutation/
	  difficulty:: Medium
	  duration:: 5 mins
	- third time solving this problem
	- first find the first number that is smaller than its next number
		- if such number doesn't exist, that reverse the whole array and return
	- then starting from that number's next position, find the smallest number that is greater than it
	- swap these two numbers, than reverse the subarray
- [[2022-04-04 Monday]] #[[Linked List]] #[[Two Pointers]]
  id:: 0decdd00-37a1-4552-964a-fcbdac7e70c9
  collapsed:: true
	- problem:: Swapping Nodes in a Linked List
	  link:: https://leetcode.com/problems/swapping-nodes-in-a-linked-list/
	  difficulty:: Medium
	  duration:: 10 mins
	- first time solving this problem
	- use two iteration to find the length of the list and the nodes we need to swap
	- swap these two nodes base on their relationship
	- can solve this in one iteration, reset the pointer to head once we reach the kth node from the head, then we can find the kth node from the end
- [[2022-04-05 Tuesday]] #Array #[[Two Pointers]] #Greedy
  id:: b9b14335-d2a1-4bdc-a7dc-d8b62f3dbf9b
  collapsed:: true
	- problem:: Container With Most Water
	  link:: https://leetcode.com/problems/container-with-most-water/
	  difficulty:: Medium
	  duration:: 3 mins
	- third time solving this problem
	- use two pointers
	- move the pointer that points to the shorter line
- [[2022-04-06 Wednesday]] #Array #[[Hash Table]] #[[Two Pointers]] #Sorting #Counting
  id:: 1b9f1071-2142-4764-8eaf-ba78d2ecf8ee
  collapsed:: true
	- problem:: 3Sum With Multiplicity
	  link:: https://leetcode.com/problems/3sum-with-multiplicity/
	  difficulty:: Medium
	  duration:: 15 mins
	- first time solving this problem
	- use two hash tables
		- one for individual number appearance, another for two number sum frequency
	- update answer using second hash table
	- update second hash table before first hash table
	- should use three pointers approach, and handle duplication cases differently
- [[2022-04-07 Thursday]] #Array #Heap
  collapsed:: true
  id:: 62517216-9cd9-406d-9d8d-fe7456ea915d
	- problem:: Last Stone Weight
	  link:: https://leetcode.com/problems/last-stone-weight/
	  difficulty:: Easy
	  duration:: 5 mins
	  id:: 76417886-6cfc-4d16-8edf-160caef7491d
	- first time solving this problem
	- first sort the array
	- then continually pop out the last two element, insert new element back into the array if it's needed
	- can also solve it using max heap
- [[2022-04-08 Friday]] #Tree #Design #[[Binary Search Tree]] #Heap #[[Binary Tree]] #[[Data Stream]]
  id:: e8c9a105-d13f-428e-bbc8-5b4b6b8bf3bc
  collapsed:: true
	- problem:: Kth Largest Element in a Stream
	  link:: https://leetcode.com/problems/kth-largest-element-in-a-stream/
	  difficulty:: Easy
	  duration:: 10 mins
	- first time solving this problem
	- maintain a priority queue of size k
	- remember to check the queue size before popping out a number to avoid empty queue
- [[2022-04-09 Saturday]] #Array #[[Hash Table]] #[[Divide and Conquer]] #Sorting #Heap #[[Bucket Sort]] #Counting #[[Quick Select]]
  id:: 453ae967-db42-483d-b556-101eb1d2efe3
  collapsed:: true
	- problem:: Top K Frequent Elements
	  link:: https://leetcode.com/problems/top-k-frequent-elements/
	  difficulty:: Medium
	  duration:: 40 mins
	- forth time solving this problem
	- use quick select
	- stuck at how the recursion boundary should work
	- move the numbers that are smaller or equal to the pivot to the second half of the array, so we can guarantee the array shrink after each iteration
	- use bucket sort can solve this problem in $O(n)$
- [[2022-04-10 Sunday]] #Array #Stack #Simulation
  id:: 16000428-f119-4380-a176-a1da3b92c3f8
  collapsed:: true
	- problem:: Baseball Game
	  link:: https://leetcode.com/problems/baseball-game/
	  difficulty:: Easy
	  duration:: 10 mins
	- first time solving this problem
	- easy to solve using stack to simulate the whole process
- [[2022-04-11 Monday]] #Array #Matrix #Simulation
  collapsed:: true
  id:: 62545723-bf91-4cbe-8fdb-2e44f66c3fa4
	- problem:: Shift 2D Grid
	  link:: https://leetcode.com/problems/shift-2d-grid/
	  difficulty:: Easy
	  duration:: 10 mins
	- first time solving this problem
	- treat the matrix as a 1D array, then shift each element by k
	- swap each number onto its correct position continuously
	- need to prove that we won’t swap same number multiple times
	- he argument if we can traverse to the second position position starting from the first position, than we can as well traverse to the third position starting from the first position, and so on. Basically we can traverse the whole array starting from the first position. But since the counter hasn’t reach the target, we know the above scenario doesn’t exist, thus prove by contradiction
	- this concept was derived from [rotate array](((3aaf91a5-581f-423f-b3da-286b974d4885)))
- [[2022-04-12 Tuesday]] #Array #Matrix #SImulation
  collapsed:: true
  id:: b8d6fae5-f0f3-4644-bdcf-1ca63679e48d
	- problem:: Game of Life
	  link:: https://leetcode.com/problems/game-of-life/
	  difficulty:: Medium
	  duration:: 10 mins
	- third time solving this problem
	- because the board only contains 0 or 1, so we can use second bit to record new state, and shift right one bit after handling all state transition
	- be careful of how to get old state
- [[2022-04-13 Wednesday]] #Array #Matrix #Simulation 
  id:: aef4f9c8-a775-4316-b324-9bb68b5ad984
  collapsed:: true
  problem:: Spiral Matrix II
  link:: https://leetcode.com/problems/spiral-matrix-ii/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 3
	- simulate the filling process
	- remember to reset starting position after finishing a layer of the matrix
	- need to fill the cell in the middle if the length of the matrix is odd
	- we can change direction if we detect we are on non-zero cell, so that we can avoid multiple for loops
- [[2022-04-14 Thursday]] #Tree #[[Binary Search Tree]] #[[Binary Tree]] 
  id:: 38fd6307-10dc-40ed-b075-6bc31f0811cd
  collapsed:: true
  problem:: Search in a Binary Search Tree
  link:: https://leetcode.com/problems/search-in-a-binary-search-tree/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 1
	- very easy
	- just traverse the binary tree until you can't
- [[2022-04-15 Friday]] #Tree #DFS #BFS #[[Binary Tree]] 
  id:: 449de5c7-310d-4c1f-be4e-4ce08c16ddb9
  collapsed:: true
  problem:: Trim a Binary Search Tree
  link:: https://leetcode.com/problems/trim-a-binary-search-tree/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
	- use recursion
	- need to trim the correct subtree if we find out current root is not in the range
	- write iterative solution next time
		- first find the right root
		- then starting from the new root, trim inappropriate nodes from the tree using stack
- [[2022-04-16 Saturday]] #Tree #DFS #BFS #[[Binary Tree]] 
  id:: d657fdda-881d-427b-9417-a53393f8bf76
  collapsed:: true
  problem:: Convert BST to Greater Tree
  link:: https://leetcode.com/problems/convert-bst-to-greater-tree/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
	- implement in-order traversal using stack
		- took some time to remember how to do it, still need to be more familiar with this [topic](((61f542da-f33e-489a-a87d-c80dc7f3de06)))
	- should try morris traversal next time #[[Morris Traversal]]
		- the idea is to get back to current node when we finish traversing its left subtree, we can achieve this by linking its successor back to it
		- to unlink, use the same function that find the successor, if we find there's a link that can traverse back to current node, we know we finish traversing current subtree
- [[2022-04-17 Sunday]] #Stack #Tree #DFS #BFS #[[Binary Tree]] 
  id:: 57cf07f4-7de1-44fa-b3ab-42c65359cfe2
  collapsed:: true
  problem:: Increasing Order Search Tree
  link:: https://leetcode.com/problems/increasing-order-search-tree/
  difficulty:: Easy
  duration:: Easy
  number_of_times:: 1
	- use iterative in-order traversal
	- remember to unlink every node's left pointer so that we won't create a cycle
	- should write recursive solution next time
- [[2022-04-18 Monday]] #Tree #DFS #BFS #[[Binary Tree]] #[[Binary Search Tree]] 
  id:: 53d1a843-7fec-4a88-84a3-951a44ccbc1a
  collapsed:: true
  problem:: Kth Smallest Element in a BST
  link:: https://leetcode.com/problems/kth-smallest-element-in-a-bst/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 3
	- implement iterative in-order traversal
	- tried to use morris traversal, but the judge didn't allow non-tree structure
- [[2022-04-19 Tuesday]] #Tree #DFS #BFS #[[Binary Tree]] #[[Morris Traversal]] 
  id:: 22b46aaa-d60b-464c-8afe-13906e5da894
  collapsed:: true
  problem:: Recover Binary Search Tree
  link:: https://leetcode.com/problems/recover-binary-search-tree/
  difficulty:: Medium
  duration:: 1 hr
  number_of_times:: 1
	- tried to use various methods to do in-order traversal, but failed to find out the misplaced nodes
	- think about what happen if we swap a pair of numbers in a list of sorted numbers
		- for the first misplaced number, it will still be bigger than its previous number, but also will be bigger than its next number
		- for the second misplaced number, it will be smaller than its previous number
	- use morris traversal and constant space next time
- [[2022-04-20 Wednesday]] #Stack #Tree #Design #[[Binary Search Tree]] #[[Binary Tree]] #Iterator 
  problem:: Binary Search Tree Iterator
  link:: https://leetcode.com/problems/binary-search-tree-iterator/
  difficulty:: Medium
  duration:: 25 mins
  number_of_times:: 3
	- implement morris traversal
	- because we have to stop in the iterator, so the implementation is a little different than normal morris traversal
	- we can use current pointer to indicate whether we have finished the traversal or not
	- this solution doesn't satisfy the question's requirements
- [[2022-04-21 Thursday]] #Array #[[Hash Table]] #[[Linked List]] #Design #[[Hash Function]] 
  id:: 1c8463e5-2116-41b3-9054-ff87cec58685
  problem:: Design HashSet
  link:: https://leetcode.com/problems/design-hashset/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
	- use a dynamically allocated array and a size variable to implement it
	- should use an actual hash function next time
- [[2022-04-22 Friday]] #Array #[[Hash Table]] #[[Linked List]] #Design #[[Hash Function]] 
  id:: 3e14050c-a540-40df-91b3-37a3e6ee976a
  collapsed:: true
  problem:: Design HashMap
  link:: https://leetcode.com/problems/design-hashmap/
  difficulty:: Easy
  duration:: 10 mins
  number_of_times:: 1
	- use an array to implement it
	- should write my own node class to mimic the real structure behind hash map
- [[2022-04-23 Saturday]] #[[Hash Table]] #String #Design #[[Hash Function]] 
  id:: b1923d01-f3ac-457a-a1f0-770b0dcfa68d
  collapsed:: true
  problem:: Encode and Decode TinyURL
  link:: https://leetcode.com/problems/encode-and-decode-tinyurl/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
	- use two hash tables to store two way mapping
	- generate 6 characters long string as short url
	- remember to check if there is collision in new generated url
- [[2022-04-24 Sunday]] #[[Hash Table]] #String #Design 
  id:: aa3ca182-b410-41d0-ae7c-bf30ed411801
  collapsed:: true
  problem:: Design Underground System
  link:: https://leetcode.com/problems/design-underground-system/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
	- use two hash table
		- one for customer's starting station and time
		- another for total travel time and number of records of each stations pair
- [[2022-04-25 Monday]] #Array #Design #Iterator 
  id:: d1fd9fd6-2029-4412-bff0-548a069831c1
  collapsed:: true
  problem:: Peeking Iterator
  link:: https://leetcode.com/problems/peeking-iterator/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 3
	- use two additional variables to store iterator's state
	- remember to check if there is element left before moving the iterator
- [[2022-04-26 Tuesday]] #Array #[[Union Find]] #[[Minimum Spanning Tree]] #Graph 
  id:: b83add23-920b-4808-bcf6-056f5df94850
  collapsed:: true
  problem:: Min Cost to Connect All Points
  link:: https://leetcode.com/problems/min-cost-to-connect-all-points/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 1
	- maintain a set of points that are connected
	- in each iteration, select a node in the set that hasn't been selected, which has the shortest distance to the connected nodes
	- this is a classic minimum spanning tree problem, and I actually implemented the Prim's algorithm
	- Prim's algorithm can be implemented with min-heap
	- or maybe implement Kruskal's algorithm next time
- [[2022-04-27 Wednesday]] #[[Hash Table]] #String #DFS #BFS #[[Union Find]] 
  id:: 70517444-767d-482c-90a0-0436f828810e
  problem:: Smallest String With Swaps
  link:: https://leetcode.com/problems/smallest-string-with-swaps/
  difficulty:: Medium
  duration:: 50 mins
  number_of_times:: 1
  collapsed:: true
	- positions that are connected through pairs can be sorted
	- we use DFS to find those connected position
	- we replace characters on those position in the original string with our sorted character strings
	- implement union find next time
- [[2022-04-28 Thursday]] #Array #[[Binary Search]] #DFS #BFS #[[Union Find]] #Heap #Matrix 
  id:: 54e99a69-4bf4-448e-9df5-622c5a89ae80
  collapsed:: true
  problem:: Path With Minimum Effort
  link:: https://leetcode.com/problems/path-with-minimum-effort/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
	- tried to use DP but failed
		- we can go up and left in this question
	- use BFS, but allow to revisit a position
		- use another matrix to record the effort walking to a position, if we can revisit a position with lower effort, then we allow it
	- this is actually a variation of Dijkstra's algorithm
	- use binary search plus DFS next time
- [[2022-04-29 Friday]] #DFS #BFS #[[Union Find]] #Graph 
  id:: e2e2cdd8-574b-4d02-b712-630549f3481e
  collapsed:: true
  problem:: Is Graph Bipartite?
  link:: https://leetcode.com/problems/is-graph-bipartite/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
	- use two hash tables to store two sets of nodes
	- use BFS to separate nodes
	- terminate the program if current node and its neighbor are in the same set during BFS
	- if BFS is finished and there still have nodes that haven't been added to the sets, then choose one node, add it to one of the set, and start another BFS
		- this means the graph contains separated components
	- I should try DFS next time, and hash tables are not required
- [[2022-04-30 Saturday]] #Array #DFS #BFS #[[Union Find]] #Graph #[[Shortest Path]] 
  id:: 626c9652-7efa-46ce-b48e-cddf6ab32493
  problem:: Evaluate Division
  link:: https://leetcode.com/problems/evaluate-division/
  difficulty:: Medium
  duration:: 35 mins
  number_of_times:: 3
	- use a variation of union find
		- record relative multiple with parent
		- when finding a point's root, calculate the multiple as well, so that we can do path compression correctly
	- draw a simple graph to help us understand how to union two components correctly
		- [[draws/2022-04-30-11-10-55.excalidraw]]
	- create the nodes before if they don't exist
	- evaluation is easy if we implement the find function of union find correctly
	- there may be non-exist nodes in the queries, make sure the program can detect it
- [Reverse String](((baf21642-c5c9-497e-a1f2-74c4b336b3b4))) is very easy
- [Valid Palindrome II](((de429926-6076-4b1c-ba9b-050b51a6e9a5))) is not that intuitive, we cannot solve it with simple condition to decide which character to delete, we need to walk through the entire process of two ways of deleting character
- [Next Permutation](((d4167fbd-dbda-4a1f-8c08-1c30b1f12ddd))) is easy to solve once you find the regularity
- [Swapping Nodes in a Linked List](((0decdd00-37a1-4552-964a-fcbdac7e70c9))) can be solved using two pointers to optimize efficiency
- [Container With Most Water](((b9b14335-d2a1-4bdc-a7dc-d8b62f3dbf9b))) can be solved using greedy, and the proof is intuitive once the graph is drawn
- [3Sum With Multiplicity](((1b9f1071-2142-4764-8eaf-ba78d2ecf8ee))) is a mutation of 3sum problem, should have use three pointers approach to increase memory efficiency
- [Last Stone Weight](((62517216-9cd9-406d-9d8d-fe7456ea915d))) is easy to solve once you figure out how to insert new element while maintaining the sorted property, or just use heap to help you achieve this
- [Kth Largest Element in a Stream](((e8c9a105-d13f-428e-bbc8-5b4b6b8bf3bc))) is easy to solving using priority queue, but need to be avoid empty queue situation
- [Top K Frequent Elements](((453ae967-db42-483d-b556-101eb1d2efe3))) can be solved using quick select, but I still can't implement quick select smoothly
- [Baseball Game](((16000428-f119-4380-a176-a1da3b92c3f8))) is easy to solve using stack
- [Shift 2D Grid](((62545723-bf91-4cbe-8fdb-2e44f66c3fa4))) can be solved easily if we treat the matrix as a 1D array
- [Game of Life](((b8d6fae5-f0f3-4644-bdcf-1ca63679e48d))) can be solved in place, just use additional bit to store new state
- [Spiral Matrix II](((aef4f9c8-a775-4316-b324-9bb68b5ad984))) can be solved by filling matrix layer by layer, and by detecting non-zero cell, we can change direction automatically
- [Search in a Binary Search Tree](((38fd6307-10dc-40ed-b075-6bc31f0811cd))) is a basic binary search tree traversal problem
- [Trim a Binary Search Tree](((449de5c7-310d-4c1f-be4e-4ce08c16ddb9))) is easy to solve using recursion, but iterative solution needs two steps
- [Convert BST to Greater Tree](((d657fdda-881d-427b-9417-a53393f8bf76))) is easy to solved using in-order traversal, but morris traversal has better performance
- [Increasing Order Search Tree](((57cf07f4-7de1-44fa-b3ab-42c65359cfe2))) is easy to solve using iterative in-order traversal and a new dummy node, should try recursive solution next time
- [Kth Smallest Element in a BST](((53d1a843-7fec-4a88-84a3-951a44ccbc1a))) is a normal question with in-order traversal on a binary search tree
- [Recover Binary Search Tree](((22b46aaa-d60b-464c-8afe-13906e5da894))) is a problem not only about the traversal of a binary search tree, but it is also about how to find a pair of misplaced number in a sorted array
- [Binary Search Tree Iterator](((7830f59c-a2c2-4472-bfc3-f71ceade3fc0))) can be solved using modified morris traversal, although it doesn't satisfy the question's requirements
- [Design HashSet](((1c8463e5-2116-41b3-9054-ff87cec58685))) can be solved just using an array because the test set is simple, but I should use an actual hash function next time
- [Design HashMap](((3e14050c-a540-40df-91b3-37a3e6ee976a))) can be solved just using an array, but I should try implementing custom node class next time
- [Encode and Decode TinyURL](((b1923d01-f3ac-457a-a1f0-770b0dcfa68d))) can be solved using two hash tables, we don't need a hash function, we just need to generate a 6 characters string and make sure there is no collision for every url
- [Design Underground System](((aa3ca182-b410-41d0-ae7c-bf30ed411801))) need two hash tables
- [Peeking Iterator](((d1fd9fd6-2029-4412-bff0-548a069831c1))) is easy to solve using two additional variable
- [Min Cost to Connect All Points](((b83add23-920b-4808-bcf6-056f5df94850))) is a classic minimal spanning tree problem, and I should implement Kruskal's algorithm next time
- [Smallest String With Swaps](((70517444-767d-482c-90a0-0436f828810e))) can be solved using DFS, and I should try union find next time
- [Path With Minimum Effort](((54e99a69-4bf4-448e-9df5-622c5a89ae80))) is a variation of BFS
- [Is Graph Bipartite?](((e2e2cdd8-574b-4d02-b712-630549f3481e))) is a basic question about testing if a graph is bipartite or not, it can be solved using BFS and DFS
- [Evaluate Division](((626c9652-7efa-46ce-b48e-cddf6ab32493))) is a variation of union find, it took some time to implement it correctly