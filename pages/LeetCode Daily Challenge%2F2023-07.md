- 0 easy, 7 medium, 0 hard
- 3 problems were solved for the first time
- [[2023-07-14 Friday]] #Array #[[Hash Table]] #DP 
  problem:: Longest Arithmetic Subsequence of Given Difference
  link:: https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 64b094f0-ee66-4702-8ab7-ba602117f51c
	- use DP with a hash table
- [[2023-07-17 Monday]]
  problem:: Add Two Numbers II
  link:: https://leetcode.com/problems/add-two-numbers-ii/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 2
  id:: 64b488c9-ebce-400b-bb5e-121bbf9c2296
	- reverse the input lists then add them up
	- need to handle the carry at the end
- [[2023-07-22 Saturday]] #DP 
  problem:: Knight Probability in Chessboard
  link:: https://leetcode.com/problems/knight-probability-in-chessboard/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 64b488fa-5b39-40db-a028-546a9e862d15
	- use DP to find the probability of each position after each move
- [[2023-07-24 Monday]] #Math #Recursion 
  problem:: Pow(x, n)
  link:: https://leetcode.com/problems/powx-n/description/
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 3
  id:: 64bb2710-eeb6-4e63-bafb-923c82c606d3
	- use recursion to do divide and conquer
	- avoid integer overflow when n equals to integer minimum
- [[2023-07-25 Tuesday]] #Array #[[Binary Search]] 
  problem:: Peak Index in a Mountain Array
  link:: https://leetcode.com/problems/peak-index-in-a-mountain-array/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 64bdc397-ae79-4a98-be7f-e1fc0fda99fe
	- use binary search
- [[2023-07-26 Wednesday]] #Array #[[Binary Search]] 
  problem:: Minimum Speed to Arrive on Time
  link:: https://leetcode.com/problems/minimum-speed-to-arrive-on-time/description/
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 64bf1599-0440-4b2c-a77d-63950b655fb9
	- use binary search to search in the answer space
	- check the answer is valid
- [[2023-07-28 Friday]] #Array #Math #DP #Recursion #[[Game Theory]] 
  problem:: Predict the Winner
  link:: https://leetcode.com/problems/predict-the-winner/description/
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 2
  id:: 64c06830-a4f8-42ad-8dc0-60ce74c0bcf3
	- use DP, and reduce it to one dimensional
-
- [Longest Arithmetic Subsequence of Given Difference](((64b094f0-ee66-4702-8ab7-ba602117f51c))) can be solved by DP with a hash table
- [Add Two Numbers II](((64b488c9-ebce-400b-bb5e-121bbf9c2296))) can be solved by reversing the lists, or use stacks to store the digits
- [Knight Probability in Chessboard](((64b488fa-5b39-40db-a028-546a9e862d15))) can be solved by DP
- [Pow(x, n)](((64bb2710-eeb6-4e63-bafb-923c82c606d3))) can be solved by recursion
- [Peak Index in a Mountain Array](((64bdc397-ae79-4a98-be7f-e1fc0fda99fe))) is a simple binary search problem
- [Minimum Speed to Arrive on Time](((64bf1599-0440-4b2c-a77d-63950b655fb9))) can be solved by using binary search on the answer space
- [Predict the Winner](((64c06830-a4f8-42ad-8dc0-60ce74c0bcf3))) can be solved by one dimensional DP, can start with two dimensional DP to help to understand the concept