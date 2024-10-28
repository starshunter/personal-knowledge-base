- 5 easy, 8 medium, 0 hard
- 5 problems were solved for the first time
- [[2024-02-01 Thursday]] #Array #Greedy #Sorting 
  problem:: Divide Array Into Arrays With Max Difference
  link:: https://leetcode.com/problems/divide-array-into-arrays-with-max-difference/description/?envType=daily-question&envId=2024-02-01
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 1
  id:: 65bae51b-4833-46f0-af08-afb3d84c85df
	- easy greedy problem
- [[2024-02-05 Monday]] #[[Hash Table]] #String #Queue #Counting 
  problem:: First Unique Character in a String
  link:: https://leetcode.com/problems/first-unique-character-in-a-string/description/?envType=daily-question&envId=2024-02-05
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 3
  id:: 65bae557-fd92-4623-a850-5a9ba497acfb
	- easy hash table problem
- [[2024-02-06 Tuesday]] #Array #[[Hash Table]] #String #Sorting 
  problem:: Group Anagrams
  link:: https://leetcode.com/problems/group-anagrams/description/?envType=daily-question&envId=2024-02-06
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 4
  id:: 65c02749-8532-48fc-b455-218c09319664
	- use the sorted string as hash table key, store all anagrams under that key
- [[2024-02-14 Wednesday]] #Array #[[Two Pointers]] #Simulation 
  problem:: Rearrange Array Elements by Sign
  link:: https://leetcode.com/problems/rearrange-array-elements-by-sign/description/?envType=daily-question&envId=2024-02-14
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 1
  id:: 65c277cb-44e0-4366-9852-bca258268da2
	- use two arrays to sort the positives and negatives
- [[2024-02-16 Friday]] #Array #[[Hash Table]] #Greedy #Sorting #Counting 
  problem:: Least Number of Unique Integers after K Removals
  link:: https://leetcode.com/problems/least-number-of-unique-integers-after-k-removals/description/?envType=daily-question&envId=2024-02-16
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 65cd3652-adae-4a72-b807-0dbd3ac71479
	- use a hash table to count the occurrence
	- put numbers into buckets using their occurrences
- [[2024-02-17 Saturday]] #Array #Greedy #Heap 
  problem:: Furthest Building You Can Reach
  link:: https://leetcode.com/problems/furthest-building-you-can-reach/description/?envType=daily-question&envId=2024-02-17
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 2
  id:: 65ceac0b-e642-49de-bcf9-7a55e42450e8
	- store the differences in a heap and only use the bricks when the size exceeds the number of ladders
- [[2024-02-19 Monday]] #Math #[[Bit Manipulation]] #Recursion 
  problem:: Power of Two
  link:: https://leetcode.com/problems/power-of-two/description/?envType=daily-question&envId=2024-02-19
  difficulty:: Easy
  duration:: 2 mins
  number-of-times:: 2
  id:: 65cffdf0-5092-4087-bbc4-f2f3b9f9db83
	- use bit manipulation to check if the number only contains one 1 in binary
- [[2024-02-20 Tuesday]] #Array #[[Hash Table]] #Math #[[Binary Search]] #[[Bit Manipulation]] #Sorting 
  problem:: Missing Number
  link:: https://leetcode.com/problems/missing-number/description/?envType=daily-question&envId=2024-02-20
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 4
  id:: 65d29da1-9adc-4686-a725-7668b7735a36
	- use XOR to find the missing number
- [[2024-02-21 Wednesday]] #[[Bit Manipulation]] 
  problem:: Bitwise AND of Numbers Range
  link:: https://leetcode.com/problems/bitwise-and-of-numbers-range/description/?envType=daily-question&envId=2024-02-21
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 3
  id:: 65d3f04c-acaa-4bf4-912d-e7530ef24ebc
	- find the common prefix in binary representation
- [[2024-02-23 Friday]] #DP #DFS #BFS #Graph #Heap #[[Shortest Path]] 
  problem:: Cheapest Flights Within K Stops
  link:: https://leetcode.com/problems/cheapest-flights-within-k-stops/description/?envType=daily-question&envId=2024-02-23
  difficulty:: Medium
  duration:: 15 mins
  number-of-times:: 3
  id:: 65d54027-8fc3-4156-8e0d-9ac7d9535aa4
	- construct the graph first then use BFS
	- update the distance in each iteration
	- remember to use a new list to record new distance to avoid using the new distance in current iteration
- [[2024-02-26 Monday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Same Tree
  link:: https://leetcode.com/problems/same-tree/description/?envType=daily-question&envId=2024-02-26
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 4
  id:: 65d7e637-6f64-48d0-aa89-d62dfc5e47b2
	- use recursion to compare each subtree
	- need to check null nodes first
- [[2024-02-27 Tuesday]] #Tree #DFS #[[Binary Tree]] 
  problem:: Diameter of Binary Tree
  link:: https://leetcode.com/problems/diameter-of-binary-tree/description/?envType=daily-question&envId=2024-02-27
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 3
  id:: 65dbd7b0-dabd-48ed-8e11-0434df0131f4
	- use recursion to find each subtree's depth
- [[2024-02-28 Wednesday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Find Bottom Left Tree Value
  link:: https://leetcode.com/problems/find-bottom-left-tree-value/description/?envType=daily-question&envId=2024-02-28
  difficulty:: Medium
  duration:: 2 mins
  number-of-times:: 1
  id:: 65dd2b57-23c9-4f4f-b548-78e22f996807
	- use BFS to find the last node in the tree
	- push right child into the queue first
- [[2024-02-29 Thursday]] #Tree #BFS #[[Binary Tree]] 
  problem:: Even Odd Tree
  link:: https://leetcode.com/problems/even-odd-tree/description/?envType=daily-question&envId=2024-02-29
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 65de7fee-088e-4342-b433-e3bb0895b7c4
	- use BFS
-
- [Divide Array Into Arrays With Max Difference](((65bae51b-4833-46f0-af08-afb3d84c85df))) can be solved by sorting the array then check the condition greedily
- [First Unique Character in a String](((65bae557-fd92-4623-a850-5a9ba497acfb))) can be solved by using a hash table
- [Group Anagrams](((65c02749-8532-48fc-b455-218c09319664))) can be solved by using a hash table
- [Rearrange Array Elements by Sign](((65c277cb-44e0-4366-9852-bca258268da2))) can be solved by using additional arrays
- [Least Number of Unique Integers after K Removals](((65cd3652-adae-4a72-b807-0dbd3ac71479))) can be solved by counting the occurrences first then sort the occurrences
- [Furthest Building You Can Reach](((65ceac0b-e642-49de-bcf9-7a55e42450e8))) can be solved by using a priority queue
- [Power of Two](((65cffdf0-5092-4087-bbc4-f2f3b9f9db83))) is an easy bit manipulation problem
- [Missing Number](((65d29da1-9adc-4686-a725-7668b7735a36))) is an easy bit manipulation problem
- [Bitwise AND of Numbers Range](((65d3f04c-acaa-4bf4-912d-e7530ef24ebc))) can be solved by finding the common prefix of the boundaries in binary representation
- [Cheapest Flights Within K Stops](((65d54027-8fc3-4156-8e0d-9ac7d9535aa4))) can be solved by using BFS, and use a temporary list to record the updated distances
- [Same Tree](((65d7e637-6f64-48d0-aa89-d62dfc5e47b2))) is an easy recursion problem
- [Diameter of Binary Tree](((65dbd7b0-dabd-48ed-8e11-0434df0131f4))) is an easy recursion problem
- [Find Bottom Left Tree Value](((65dd2b57-23c9-4f4f-b548-78e22f996807))) is an easy BFS problem
- [Even Odd Tree](((65de7fee-088e-4342-b433-e3bb0895b7c4))) is an easy BFS problem