- 6 easy, 12 medium, 0 hard
- 8 problems were solved for the first time
- [[2023-04-01 Saturday]] #Array #[[Binary Search]] 
  problem:: Binary Search
  link:: https://leetcode.com/problems/binary-search/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 2
  id:: 64277f7b-2a3d-4517-b63a-a73798c27bd7
	- basic binary search
- [[2023-04-02 Sunday]] #Array #[[Two Pointers]] #[[Binary Search]] #Sorting 
  problem:: Successful Pairs of Spells and Potions
  link:: https://leetcode.com/problems/successful-pairs-of-spells-and-potions/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 64277f9d-c221-4ebe-803d-7b8d49c7d47a
	- sort the array first
	- find the target to do binary search
	- be careful of integer overflow
	- need to consider the case where the target is greater than the maximum item in the array
- [[2023-04-03 Monday]] #Array #[[Two Pointers]] #Greedy #Sorting 
  problem:: Boats to Save People
  link:: https://leetcode.com/problems/boats-to-save-people/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 2
  id:: 642970ac-22fc-4843-a207-05ee3fce67c6
	- sort the array first
	- use two pointers
- [[2023-04-04 Tuesday]] #[[Hash Table]] #String #Greedy 
  problem:: Optimal Partition of String
  link:: https://leetcode.com/problems/optimal-partition-of-string/description/
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 1
  id:: 642a867b-3fcf-4adc-890a-ac4cd7e039d2
	- use an integer as a hash table
- [[2023-04-05 Wednesday]] #Array #[[Binary Search]] #DP #Greedy #[[Prefix Sum]] 
  problem:: Minimize Maximum of Array
  link:: https://leetcode.com/problems/minimize-maximum-of-array/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 642b6d38-9b31-474a-bc73-8875180e1e99
	- the maximum is the ceiling of the average of the subarray
	- we don't need to do anything if we encounter a number smaller than the current maximum
	- the new average may be smaller than the current maximum, so take the maximum of the two
- [[2023-04-06 Thursday]] #Array #DFS #BFS #[[Union Find]] #Matrix 
  problem:: Number of Closed Islands
  link:: https://leetcode.com/problems/number-of-closed-islands/description/
  difficulty:: Medium
  duration:: 15 mins
  number-of-times:: 1
  id:: 642cc1ce-0bf8-4028-ae32-350ebb6dabb4
	- use DFS to find all the islands
	- check if the island touch the boundaries
- [[2023-04-08 Saturday]] #[[Hash Table]] #DFS #BFS #Graph 
  problem:: Clone Graph
  link:: https://leetcode.com/problems/clone-graph/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 4
  id:: 642eb903-0312-4359-9a0b-9b3bf8190f87
	- use DFS to clone the graph
	- need a hash table to record the mapping between old nodes and cloned nodes
- [[2023-04-10 Monday]] #String #Stack 
  problem:: Valid Parentheses
  link:: https://leetcode.com/problems/valid-parentheses/description/
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 4
  id:: 6430b6a8-b1f4-4aca-9ab1-d9205148cd79
	- use a stack to store open parentheses
- [[2023-04-12 Wednesday]] #String #Stack 
  problem:: Simplify Path
  link:: https://leetcode.com/problems/simplify-path/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 4
  id:: 6433532f-3920-47d1-a47d-615816b26d2b
	- iterate through the input path, and maintain a simplified path
	- remember to append a slash at the end of the input path
- [[2023-04-13 Thursday]] #Array #Stack #Simulation #[[Two Pointers]] 
  id:: 6435f8d2-accb-4b93-abbb-0fca3354671b
  problem:: Validate Stack Sequences
  link:: https://leetcode.com/problems/validate-stack-sequences/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
	- use a stack to simulate the process
	- can save the space by modifying the input array
- [[2023-04-14 Friday]] #String #DP 
  problem:: Longest Palindromic Subsequence
  link:: https://leetcode.com/problems/longest-palindromic-subsequence/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 64374b34-53e5-4e52-b32a-0acc62dea77d
	- use two dimensional DP
	- increase value if the letters on two ends match
	- choose the maximum of the sub interval if there's no match
- [[2023-04-17 Monday]] #Array 
  problem:: Kids With the Greatest Number of Candies
  link:: https://leetcode.com/problems/kids-with-the-greatest-number-of-candies/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 64389c0d-3092-48ff-984a-e9258549ec69
	- find the maximum first then check each number
- [[2023-04-18 Tuesday]] #[[Two Pointers]] #String 
  problem:: Merge Strings Alternately
  link:: https://leetcode.com/problems/merge-strings-alternately/description/
  difficulty:: Easy
  duration:: 2 mins
  number-of-times:: 1
  id:: 643c8e8c-dfc8-4ca9-a12d-c4ce011dea7a
	- easy two pointers problem
- [[2023-04-19 Wednesday]] #DP #Tree #DFS #[[Binary Tree]] 
  problem:: Longest ZigZag Path in a Binary Tree
  link:: https://leetcode.com/problems/longest-zigzag-path-in-a-binary-tree/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 643de0e6-fee1-435a-9743-ac7db609682f
	- use DFS
	- for every node, find the maximum zigzag length in different directions
	- the answer doesn't need to start at the root
- [[2023-04-24 Monday]] #Array #Heap 
  problem:: Last Stone Weight
  link:: https://leetcode.com/problems/last-stone-weight/description/
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 2
  id:: 643f344c-9880-4ad7-9ab5-3c4b54a6dad7
	- use priority queue
- [[2023-04-25 Tuesday]] #[[Hash Table]] #Design #Heap 
  problem:: Smallest Number in Infinite Set
  link:: https://leetcode.com/problems/smallest-number-in-infinite-set/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 64466886-3a7b-450c-9ad1-c09b9af3bd07
	- use a set to record the numbers that have been popped from the set
	- iterate through the set to find the smallest number that has been popped out
- [[2023-04-26 Wednesday]] #Math #Simulation #[[Number Theory]] 
  problem:: Add Digits
  link:: https://leetcode.com/problems/add-digits/description/
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 4
  id:: 64471e80-1e2f-400d-a768-70bc2aed5287
	- find the pattern
- [[2023-04-27 Thursday]] #Math #Brainteaser 
  problem:: Bulb Switcher
  link:: https://leetcode.com/problems/bulb-switcher/description/
  difficulty:: Medium
  duration:: 1 min
  number-of-times:: 3
  id:: 64486c7e-b6b1-4406-80a6-e505a6d9ff1f
	- easy math problem
	- count the numbers that have a integer square root
-
- [Binary Search](((64277f7b-2a3d-4517-b63a-a73798c27bd7))) is a basic binary search problem
- [Successful Pairs of Spells and Potions](((64277f9d-c221-4ebe-803d-7b8d49c7d47a))) can be solved by binary search, and need to consider maximum number corner case
- [Boats to Save People](((642970ac-22fc-4843-a207-05ee3fce67c6))) is an easy two pointers problem
- [Optimal Partition of String](((642a867b-3fcf-4adc-890a-ac4cd7e039d2))) is an easy hash table problem
- [Minimize Maximum of Array](((642b6d38-9b31-474a-bc73-8875180e1e99))) can be solved by using DP and prefix sum, remember to take the maximum of the new average and current maximum
- [Number of Closed Islands](((642cc1ce-0bf8-4028-ae32-350ebb6dabb4))) can be solved by using DFS to find all the islands
- [Clone Graph](((642eb903-0312-4359-9a0b-9b3bf8190f87))) can be solved by using DFS with a hash table
- [Valid Parentheses](((6430b6a8-b1f4-4aca-9ab1-d9205148cd79))) is an easy stack problem
- [Simplify Path](((6433532f-3920-47d1-a47d-615816b26d2b))) can be solved by iterating through the string
- [Validate Stack Sequences](((6435f8d2-accb-4b93-abbb-0fca3354671b))) can be solved by using two pointers and without extra space
- [Longest Palindromic Subsequence](((64374b34-53e5-4e52-b32a-0acc62dea77d))) can be solved by using two dimensional DP
- [Kids With the Greatest Number of Candies](((64389c0d-3092-48ff-984a-e9258549ec69))) is an easy problem
- [Merge Strings Alternately](((643c8e8c-dfc8-4ca9-a12d-c4ce011dea7a))) is an easy two pointers problem
- [Longest ZigZag Path in a Binary Tree](((643de0e6-fee1-435a-9743-ac7db609682f))) can be solved by using DFS to return the maximum zigzag length in each direction
- [Last Stone Weight](((643f344c-9880-4ad7-9ab5-3c4b54a6dad7))) is an easy priority queue problem
- [Smallest Number in Infinite Set](((64466886-3a7b-450c-9ad1-c09b9af3bd07))) can be solved by using a set to keep all the numbers that have been popped out
- [Add Digits](((64471e80-1e2f-400d-a768-70bc2aed5287))) is an easy math problem
- [Bulb Switcher](((64486c7e-b6b1-4406-80a6-e505a6d9ff1f))) is an easy math problem