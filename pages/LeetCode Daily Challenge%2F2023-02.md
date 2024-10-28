- 11 easy, 11 medium, 0 hard
- 12 problems were solved for the first time
- [[2023-02-01 Wednesday]] #Math #String #[[Greatest Common Divisor]]
  id:: 63d9b11a-5288-465a-bb9f-52323304f68d
  problem:: Greatest Common Divisor of Strings
  link:: https://leetcode.com/problems/greatest-common-divisor-of-strings/description/
  difficulty:: Easy
  duration:: 10 mins
  number_of_times:: 1
	- keep calculating the residual of the longer string
	- stop when there's an empty string
	- return empty string if there's a no match while comparing characters
- [[2023-02-02 Thursday]] #Array #[[Hash Table]] #String 
  problem:: Verifying an Alien Dictionary
  link:: https://leetcode.com/problems/verifying-an-alien-dictionary/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 63d9b1e5-f572-4f7f-907b-e58d048f55fc
	- use the order string to convert the words
	- check if words are sorted
- [[2023-02-03 Friday]] #String 
  problem:: Zigzag Conversion
  link:: https://leetcode.com/problems/zigzag-conversion/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 63db0181-8c00-4542-bba2-82986b13a922
	- construct the answer row by row
	- remember to handle the first and last rows as special cases
- [[2023-02-04 Saturday]] #[[Hash Table]] #[[Two Pointers]] #String #[[Sliding Window]] 
  problem:: Permutation in String
  link:: https://leetcode.com/problems/permutation-in-string/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 63dc5229-a099-4f2e-9661-0f8a0a4247aa
	- use a hash table to do sliding window
	- can avoid checking the hash table every round
- [[2023-02-05 Sunday]] #[[Hash Table]] #String #[[Sliding Window]] 
  problem:: Find All Anagrams in a String
  link:: https://leetcode.com/problems/find-all-anagrams-in-a-string/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 63dda4cc-7112-4018-b8c6-563790ef51e5
	- use a hash table and sliding window
	- keep a variable about how many characters are unsatisfied in current window
- [[2023-02-06 Monday]] #Array #[[Bit Manipulation]] 
  id:: 63df42dc-64b0-4869-8b22-4a797d039d1d
  problem:: Shuffle the Array
  link:: https://leetcode.com/problems/shuffle-the-array/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 1
	- use another array and calculate the new indexes
- [[2023-02-07 Tuesday]] #Array #[[Hash Table]] #[[Sliding Window]] 
  problem:: Fruit Into Baskets
  link:: https://leetcode.com/problems/fruit-into-baskets/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63e04823-e8ed-45bb-9194-e52ebffafb24
	- use a hash table and sliding window
- [[2023-02-08 Wednesday]] #Array #DP #Greedy 
  problem:: Jump Game II
  link:: https://leetcode.com/problems/jump-game-ii/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63e19987-c214-4d86-ae21-8970abcf8bab
	- use DP
	- can be done in one loop, considering the farthest position we can jump using certain steps
- [[2023-02-11 Saturday]] #BFS #Graph 
  problem:: Shortest Path with Alternating Colors
  link:: https://leetcode.com/problems/shortest-path-with-alternating-colors/description/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 63e2ecee-8c0d-4970-b78a-fe11c2751d7d
	- use BFS
	- need to construct two graphs, and use two hash tables to record visited nodes
	- remember to put the color of the previous edge into the queue
- [[2023-02-12 Sunday]] #Tree #DFS #BFS #Graph 
  problem:: Minimum Fuel Cost to Report to the Capital
  link:: https://leetcode.com/problems/minimum-fuel-cost-to-report-to-the-capital/description/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 63e7bdad-e0ab-4138-94b5-c3d0b3b3cf9f
	- construct a graph and use DFS
	- need to pass the people in one node during DFS
- [[2023-02-13 Monday]] #Math 
  problem:: Count Odd Numbers in an Interval Range
  link:: https://leetcode.com/problems/count-odd-numbers-in-an-interval-range/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 1
  id:: 63e837fa-8395-4ccf-bc11-a72058fa5f35
	- easy math problem
	- consider odd interval and even interval cases
- [[2023-02-14 Tuesday]] #Math #String #[[Bit Manipulation]] #Simulation 
  problem:: Add Binary
  link:: https://leetcode.com/problems/add-binary/description/
  difficulty:: Easy
  duration:: 10 mins
  number_of_times:: 3
  id:: 63e98195-e6d1-48bb-92fb-93b7b26b9492
	- add the two strings
	- the size of the string can't be negative, need to be casted
- [[2023-02-15 Wednesday]] #Array #Math 
  problem:: Add to Array-Form of Integer
  link:: https://leetcode.com/problems/add-to-array-form-of-integer/description/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 1
  id:: 63ead324-7a27-4382-b361-5b67c883dbac
	- convert the number to strings then add two strings
- [[2023-02-16 Thursday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Maximum Depth of Binary Tree
  link:: https://leetcode.com/problems/maximum-depth-of-binary-tree/description/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 4
  id:: 63ec2435-81f0-4779-b8b6-5ba10a1d0b92
	- use recursive DFS
- [[2023-02-17 Friday]] #Tree #DFS #BFS #[[Binary Search Tree]] #[[Binary Tree]] 
  problem:: Minimum Distance Between BST Nodes
  link:: https://leetcode.com/problems/minimum-distance-between-bst-nodes/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 63ed7411-d539-4236-a6ea-06bad7adc445
	- use DFS and a set
	- can use [[In-order Traversal]] to solve this problem
- [[2023-02-18 Saturday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Invert Binary Tree
  link:: https://leetcode.com/problems/invert-binary-tree/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 63eec6fb-19f5-47bc-878d-18fd200715ac
	- use BFS
- [[2023-02-19 Sunday]] #Tree #BFS #[[Binary Tree]] 
  problem:: Binary Tree Zigzag Level Order Traversal
  link:: https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 63f01821-8b49-4097-a245-7b85b39efd01
	- use breadth first search
	- reverse the entire level when the level is odd
- [[2023-02-20 Monday]] #Array #[[Binary Search]] 
  problem:: Search Insert Position
  link:: https://leetcode.com/problems/search-insert-position/description/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 4
  id:: 63f1bac1-e7c2-493d-bf96-6e4760410b5f
	- use binary search
	- need to handle the case where the target is greater than the last number
- [[2023-02-22 Wednesday]] #Array #[[Binary Search]] 
  problem:: Capacity To Ship Packages Within D Days
  link:: https://leetcode.com/problems/capacity-to-ship-packages-within-d-days/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63f2ba79-36dd-4881-9467-42be16c50183
	- use binary search to search the answer space
	- remember to set the left boundary as the maximum weight
- [[2023-02-25 Saturday]] #Array #DP 
  problem:: Best Time to Buy and Sell Stock
  link:: https://leetcode.com/problems/best-time-to-buy-and-sell-stock/description/
  difficulty:: Easy
  duration:: 1
  number_of_times:: 5
  id:: 63f56034-3248-4b9d-af5d-b39fe5b28898
	- easy DP problem
- [[2023-02-27 Monday]] #Array #[[Divide and Conquer]] #Tree #Matrix 
  problem:: Construct Quad Tree
  link:: https://leetcode.com/problems/construct-quad-tree/description/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 2
  id:: 63f95413-0af6-44af-9759-3eefcd39dca7
	- use recursion to construct the tree
	- check all the numbers in range each round
- [[2023-02-28 Tuesday]] #[[Hash Table]] #Tree #DFS #[[Binary Tree]] 
  problem:: Find Duplicate Subtrees
  link:: https://leetcode.com/problems/find-duplicate-subtrees/description/
  difficulty:: Medium
  duration:: 25 mins
  number_of_times:: 1
  id:: 63fbfe24-def9-4d90-ac6d-cb79d498a13c
	- serialize all subtrees to strings
	- use a hash table to store the root of each subtree
-
- [Greatest Common Divisor of Strings](((63d9b11a-5288-465a-bb9f-52323304f68d))) can be solved by simply calculating the GCD of the strings' length
- [Verifying an Alien Dictionary](((63d9b1e5-f572-4f7f-907b-e58d048f55fc))) can be solved by simply constructing a map than convert the input strings
- [Zigzag Conversion](((63db0181-8c00-4542-bba2-82986b13a922))) can be solved by observing the pattern, and construct the answer row by row
- [Permutation in String](((63dc5229-a099-4f2e-9661-0f8a0a4247aa))) can be solved by using a hash table and sliding window
- [Find All Anagrams in a String](((63dda4cc-7112-4018-b8c6-563790ef51e5))) can be solved by using a hash table and sliding window
- [Shuffle the Array](((63df42dc-64b0-4869-8b22-4a797d039d1d))) can be solved in place using bit manipulation
- [Fruit Into Baskets](((63e04823-e8ed-45bb-9194-e52ebffafb24))) is an easy sliding window problem
- [Jump Game II](((63e19987-c214-4d86-ae21-8970abcf8bab))) can be solved with DP, using only one loop
- [Shortest Path with Alternating Colors](((63e2ecee-8c0d-4970-b78a-fe11c2751d7d))) can be solved by BFS, but need to create two graphs
- [Minimum Fuel Cost to Report to the Capital](((63e7bdad-e0ab-4138-94b5-c3d0b3b3cf9f))) can be solved by using DFS, but we need to know how many people reach each node
- [Count Odd Numbers in an Interval Range](((63e837fa-8395-4ccf-bc11-a72058fa5f35))) is an easy math problem
- [Add Binary](((63e98195-e6d1-48bb-92fb-93b7b26b9492))) is an easy string problem, but need to be careful, the size of string can't be negative
- [Add to Array-Form of Integer](((63ead324-7a27-4382-b361-5b67c883dbac))) can be solved without converting the number to string
- [Maximum Depth of Binary Tree](((63ec2435-81f0-4779-b8b6-5ba10a1d0b92))) is an easy DFS problem
- [Minimum Distance Between BST Nodes](((63ed7411-d539-4236-a6ea-06bad7adc445))) can be solved by [[In-order Traversal]] traversal
- [Invert Binary Tree](((63eec6fb-19f5-47bc-878d-18fd200715ac))) can be solved by recursion, or iterative BFS and DFS
- [Binary Tree Zigzag Level Order Traversal](((63f01821-8b49-4097-a245-7b85b39efd01))) is an easy BFS problem
- [Search Insert Position](((63f1bac1-e7c2-493d-bf96-6e4760410b5f))) is a basic binary search problem
- [Capacity To Ship Packages Within D Days](((63f2ba79-36dd-4881-9467-42be16c50183))) cab be solved by using binary search in the answer space
- [Best Time to Buy and Sell Stock](((63f56034-3248-4b9d-af5d-b39fe5b28898))) is a basic DP problem
- [Construct Quad Tree](((63f95413-0af6-44af-9759-3eefcd39dca7))) can be solved by constructing all the subtrees first, than use the value of the subtrees to determine the value of current tree
- [Find Duplicate Subtrees](((63fbfe24-def9-4d90-ac6d-cb79d498a13c))) can be solved by using DFS to serialize the tree first, than use a hash table to find the duplicate subtrees