- 0 easy, 4 medium, 0 hard
- 2 problems were solved for the first time
- [[2023-03-02 Thursday]] #[[Two Pointers]] #String 
  problem:: String Compression
  link:: https://leetcode.com/problems/string-compression/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 63ffec81-385f-4123-9b75-d7a4eef85258
	- store current character and current length of the sequence
	- insert empty character at the end
	- reverse sequence length once we finish a sequence
- [[2023-03-21 Tuesday]] #Array #Math 
  problem:: Number of Zero-Filled Subarrays
  link:: https://leetcode.com/problems/number-of-zero-filled-subarrays/description/
  difficulty:: Medium
  duration:: 3 mins
  number_of_times:: 1
  id:: 6418f5e5-6365-4888-abdc-dc5d058d73a3
	- easy math problem, count the length of consecutive 0s
- [[2023-03-25 Saturday]] #DFS #BFS #[[Union Find]] #Graph 
  problem:: Count Unreachable Pairs of Nodes in an Undirected Graph
  link:: https://leetcode.com/problems/count-unreachable-pairs-of-nodes-in-an-undirected-graph/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 6418f60e-6169-4166-8578-848dc4c97496
	- construct the graph first
	- find all components' size using BFS
	- multiply component size with each other
		- to avoid TLE, add the size of previous components together
- [[2023-03-27 Monday]] #Array #DP #Matrix 
  problem:: Minimum Path Sum
  link:: https://leetcode.com/problems/minimum-path-sum/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 641e3f6a-08f8-4611-865b-4d8548e6695d
	- use DP to calculate the minimum paths of each row
-
- [String Compression](((63ffec81-385f-4123-9b75-d7a4eef85258))) can be solved by using two pointers, and reverse the sequence length at the end
- [Number of Zero-Filled Subarrays](((6418f5e5-6365-4888-abdc-dc5d058d73a3))) is an easy math problem
- [Count Unreachable Pairs of Nodes in an Undirected Graph](((6418f60e-6169-4166-8578-848dc4c97496))) can be solved by find the size of all components, and multiply the size with each other
- [Minimum Path Sum](((641e3f6a-08f8-4611-865b-4d8548e6695d))) can be solved by using DP on each row