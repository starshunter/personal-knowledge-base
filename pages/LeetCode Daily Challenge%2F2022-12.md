- 7 easy, 18 medium, 0 hard
- 12 problems were solved for the first time
- [[2022-12-01 Thursday]] #String #Counting 
  problem:: Determine if String Halves Are Alike
  link:: https://leetcode.com/problems/determine-if-string-halves-are-alike/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 1
  id:: 6387f805-f172-4c4b-bcd7-4e8dd796e927
	- count the number of vowels
	- make the count to be negative once we enter second half of the string, and check if the count equals to 0 at the end
- [[2022-12-02 Friday]] #[[Hash Table]] #String #Sorting 
  problem:: Determine if Two Strings Are Close
  link:: https://leetcode.com/problems/determine-if-two-strings-are-close/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 6387f84a-45d9-4e69-8583-d64bec1b38cd
	- need to check two things
		- the occurrence of unique characters of two strings are the same
		- the existing unique characters of two strings are the same
- [[2022-12-03 Saturday]] #[[Hash Table]] #String #Sorting #Heap #[[Priority Queue]] #[[Bucket Sort]] #Counting 
  problem:: Sort Characters By Frequency
  link:: https://leetcode.com/problems/sort-characters-by-frequency/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 63894dd9-f9f4-4ab9-bde6-945d1687029e
	- use two hash tables
	- count the occurrence of each character first
	- then store the occurrence and its character in descending order
	- can be solved by counting sort
- [[2022-12-04 Sunday]] #Array #[[Prefix Sum]] 
  id:: 638b427f-3631-4a20-a663-fc5ca8c2f40e
  problem:: Minimum Average Difference
  link:: https://leetcode.com/problems/minimum-average-difference/description/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
	- use prefix sum
	- need to remember divide by zero, round to floor and integer overflow problem
- [[2022-12-05 Monday]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Middle of the Linked List
  link:: https://leetcode.com/problems/middle-of-the-linked-list/description/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 1
  id:: 638bf655-4af3-4479-857c-818419aaef06
	- use two pointers
- [[2022-12-06 Tuesday]] #[[Linked List]] 
  problem:: Odd Even Linked List
  link:: https://leetcode.com/problems/odd-even-linked-list/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 638d3dc5-afe2-46da-909c-2a5f580f0cd8
	- iterate through the list and move even nodes to another list
	- concatenate the new list to the end of the old list
- [[2022-12-07 Wednesday]] #Tree #DFS #[[Binary Search Tree]] #[[Binary Tree]] 
  problem:: Range Sum of BST
  link:: https://leetcode.com/problems/range-sum-of-bst/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 2
  id:: 638e8fc5-211d-48f7-8540-821f8a2f59e0
	- easy to solve using recursive method
- [[2022-12-08 Thursday]] #Tree #DFS #[[Binary Tree]] 
  problem:: Leaf-Similar Trees
  link:: https://leetcode.com/problems/leaf-similar-trees/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 638fe28f-7e8a-4830-9859-7164cfa26b6c
	- use DFS to traverse two trees
	- when we reach a leaf, pause and wait for another tree
	- compare two leaves' value
	- the stacks used by DFS should be empty at the same time
- [[2022-12-09 Friday]] #Tree #DFS #[[Binary Tree]] 
  problem:: Maximum Difference Between Node and Ancestor
  link:: https://leetcode.com/problems/maximum-difference-between-node-and-ancestor/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 2
  id:: 63913733-8510-496e-804d-d3955462c666
	- use recursive DFS
	- update the maximum and minimum value along the way to the leaf
	- return the difference at the leaves
- [[2022-12-10 Saturday]] #Tree #DFS #[[Binary Tree]] 
  problem:: Maximum Product of Splitted Binary Tree
  link:: https://leetcode.com/problems/maximum-product-of-splitted-binary-tree/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 7652434a-6f6c-43bf-b7ca-b595bde894f0
	- do two DFS
	- first calculate the sum of each subtree
	- second find the maximum product of two subtrees
- [[2022-12-12 Monday]] #Math #DP #Memoization 
  problem:: Climbing Stairs
  link:: https://leetcode.com/problems/climbing-stairs/description/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 4
  id:: 6393f2c9-cf67-4465-984c-fbfef8990003
	- easy DP problem
- [[2022-12-13 Tuesday]] #Array #DP #Matrix 
  problem:: Minimum Falling Path Sum
  link:: https://leetcode.com/problems/minimum-falling-path-sum/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63974cc0-0e2b-4475-a61c-e594140ba654
	- easy DP problem
	- need to consider the case where the size of the matrix is 1
- [[2022-12-14 Wednesday]] #Array #DP 
  problem:: House Robber
  link:: https://leetcode.com/problems/house-robber/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 6397cec7-1555-42d2-bd48-827431cb9182
	- use DP
	- for each position, calculate the maximum sum for the cases of rubbing it and not rubbing it
- [[2022-12-15 Thursday]] #String #DP 
  problem:: Longest Common Subsequence
  link:: https://leetcode.com/problems/longest-common-subsequence/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
  id:: 6399bb66-1d9a-41ad-ae75-ca115562c565
	- use DP
	- optimize two dimensions matrix to one array
	- be careful of the first column of the array
	- need to store the value of the previous position to calculate current position
- [[2022-12-16 Friday]] #Stack #Design #Queue 
  problem:: Implement Queue using Stacks
  link:: https://leetcode.com/problems/implement-queue-using-stacks/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 639a73c8-a74c-45f0-9e37-7871f627807b
	- use two stacks
	- push elements into one stack
	- when need to pop or peek, first check if another stack is empty, if it is, then move the elements in the first stack into another
- [[2022-12-17 Saturday]] #Array #Math #Stack 
  problem:: Evaluate Reverse Polish Notation
  link:: https://leetcode.com/problems/evaluate-reverse-polish-notation/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 639cc216-9048-4281-80c7-d8cfec05f5fa
	- use a stack to store the numbers
	- pop the last two numbers when we encounter a operators
	- be careful of the integer overflow problem
- [[2022-12-18 Sunday]] #Array #Stack #[[Monotonic Stack]] 
  problem:: Daily Temperatures
  link:: https://leetcode.com/problems/daily-temperatures/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 2
  id:: 639d0f30-b4b5-403e-8f85-956f4bf7cf1d
	- use a monotonic stack to store the indexes of increasing temperatures
- [[2022-12-19 Monday]] #DFS #BFS #[[Union Find]] #Graph 
  problem:: Find if Path Exists in Graph
  link:: https://leetcode.com/problems/find-if-path-exists-in-graph/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 639ee9bb-6d49-49c5-87d9-21094f034201
	- construct a graph
	- use BFS
- [[2022-12-20 Tuesday]] #DFS #BFS #Graph 
  problem:: Keys and Rooms
  link:: https://leetcode.com/problems/keys-and-rooms/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 639fb748-f5f2-494f-9b3f-ef76c09207a8
	- use BFS
- [[2022-12-21 Wednesday]] #DFS #BFS #[[Union Find]] #Graph 
  problem:: Possible Bipartition
  link:: https://leetcode.com/problems/possible-bipartition/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63a1061d-ba7d-442e-86cc-e852ac61c2c1
	- construct a graph
	- do BFS from each node in the graph to label them
	- use a hash table to store and check each node's label
- [[2022-12-23 Friday]] #Array #DP 
  problem:: Best Time to Buy and Sell Stock with Cooldown
  link:: https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 63a25cfc-f03a-4e73-82ff-58a33fa34111
	- use DP
	- record three states for each price: buy, sell and cool
	- the state means what action was taken until current price
- [[2022-12-26 Monday]] #Array #DP #Greedy 
  problem:: Jump Game
  link:: https://leetcode.com/problems/jump-game/description/
  difficulty:: Medium
  duration:: 1 min
  number_of_times:: 3
  id:: 63a4fc30-0cc6-4c61-9e43-023b9bccbff8
	- use greedy, for every position, find the farthest position we can jump to after visiting that position
- [[2022-12-27 Tuesday]] #Array #Greedy #Sorting 
  problem:: Maximum Bags With Full Capacity of Rocks
  link:: https://leetcode.com/problems/maximum-bags-with-full-capacity-of-rocks/description/
  difficulty:: Medium
  duration:: 3 mins
  number_of_times:: 1
  id:: 63a8f0c3-2f30-4de5-9ae1-eb0d5345f495
	- calculate the remaining capacity for every bag
	- use greedy and fill the bag until we run out of rocks
- [[2022-12-28 Wednesday]] #Array #Heap #[[Priority Queue]] 
  problem:: Remove Stones to Minimize the Total
  link:: https://leetcode.com/problems/remove-stones-to-minimize-the-total/description/
  difficulty:: Medium
  duration:: 3 mins
  number_of_times:: 1
  id:: 63aa4583-8678-4af0-bb1f-aedaa98cf062
	- put the input inside a priority queue
	- use greedy to continue to cut the biggest element in half
- [[2022-12-30 Friday]] #Backtracking #DFS #BFS #Graph #DAG 
  problem:: All Paths From Source to Target
  link:: https://leetcode.com/problems/all-paths-from-source-to-target/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 63ab9676-7812-4d35-b8cf-82d19b4d6d31
	- use BFS
	- because the input is a DAG, we don't need to record the nodes we already visited
-
- [Determine if String Halves Are Alike](((6387f805-f172-4c4b-bcd7-4e8dd796e927))) is an easy counting problem
- [Determine if Two Strings Are Close](((6387f84a-45d9-4e69-8583-d64bec1b38cd))) can be solved by checking the occurrence of unique characters, and the existing unique characters
- [Sort Characters By Frequency](((63894dd9-f9f4-4ab9-bde6-945d1687029e))) can be solved by hash tables and counting sort
- [Minimum Average Difference](((638b427f-3631-4a20-a663-fc5ca8c2f40e))) can be solved by using prefix sum, but need to remember some integer and floating point details
- [Middle of the Linked List](((638bf655-4af3-4479-857c-818419aaef06))) is an easy two pointers problem
- [Odd Even Linked List](((638d3dc5-afe2-46da-909c-2a5f580f0cd8))) can be solved by using another list to store all the even nodes
- [Range Sum of BST](((638e8fc5-211d-48f7-8540-821f8a2f59e0))) can be solved by both recursive and iterative method
- [Leaf-Similar Trees](((638fe28f-7e8a-4830-9859-7164cfa26b6c))) can be solved by doing DFS on both trees
- [Maximum Difference Between Node and Ancestor](((63913733-8510-496e-804d-d3955462c666))) can be solved by using DFS, and record maximum and minimum value along the way to leaf
- [Maximum Product of Splitted Binary Tree](((7652434a-6f6c-43bf-b7ca-b595bde894f0))) can be solved by doing two DFS
- [Climbing Stairs](((6393f2c9-cf67-4465-984c-fbfef8990003))) is a very basic DP problem
- [Minimum Falling Path Sum](((63974cc0-0e2b-4475-a61c-e594140ba654))) can be solved by using DP
- [House Robber](((6397cec7-1555-42d2-bd48-827431cb9182))) is a classic DP problem, every iteration update the status of robbing that position and not rubbing that position
- [Longest Common Subsequence](((6399bb66-1d9a-41ad-ae75-ca115562c565))) is a classic DP problem, and can be optimized to only using one array
- [Implement Queue using Stacks](((639a73c8-a74c-45f0-9e37-7871f627807b))) can be solved by using two stacks, move elements into another stack to perform peek and pop
- [Evaluate Reverse Polish Notation](((639cc216-9048-4281-80c7-d8cfec05f5fa))) can be solved by using a stack
- [Daily Temperatures](((639d0f30-b4b5-403e-8f85-956f4bf7cf1d))) is an easy monotonic stack problem, but remember to store the index into it
- [Find if Path Exists in Graph](((639ee9bb-6d49-49c5-87d9-21094f034201))) can be solved by using BFS or DFS
- [Keys and Rooms](((639fb748-f5f2-494f-9b3f-ef76c09207a8))) can be solved by using BFS or DFS
- [Possible Bipartition](((63a1061d-ba7d-442e-86cc-e852ac61c2c1))) can be solved by using BFS or DFS to label each node, or use union find
- [Best Time to Buy and Sell Stock with Cooldown](((63a25cfc-f03a-4e73-82ff-58a33fa34111))) can be solved by using DP with three states for each price
- [Jump Game](((63a4fc30-0cc6-4c61-9e43-023b9bccbff8))) can be solved by using greedy from the start or the end
- [Maximum Bags With Full Capacity of Rocks](((63a8f0c3-2f30-4de5-9ae1-eb0d5345f495))) is a simple greedy problem
- [Remove Stones to Minimize the Total](((63aa4583-8678-4af0-bb1f-aedaa98cf062))) can be solved by using greedy with priority queue
- [All Paths From Source to Target](((63ab9676-7812-4d35-b8cf-82d19b4d6d31))) is an easy BFS problem