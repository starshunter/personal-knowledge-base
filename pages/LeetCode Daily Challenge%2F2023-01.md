- 7 easy, 15 medium, 0 hard
- 8 problems were solved for the first time
- [[2023-01-01 Sunday]] #[[Hash Table]] #String 
  problem:: Word Pattern
  link:: https://leetcode.com/problems/word-pattern/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 4
  id:: 63b18658-c0c3-4bb4-8dd8-4f3d075e679d
	- use two hash table
	- need to check character to string mapping, and vice versa
- [[2023-01-02 Monday]] #String 
  problem:: Detect Capital
  link:: https://leetcode.com/problems/detect-capital/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 2
  id:: 63b243f1-cf3b-4c13-a1d7-437bb0ea71a6
	- use a variable to represent whether last character is capital
	- only need to change it when the second character change from capital to not capital
- [[2023-01-03 Tuesday]] #Array #String 
  problem:: Delete Columns to Make Sorted
  link:: https://leetcode.com/problems/delete-columns-to-make-sorted/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 63b24430-aada-4085-a9f6-ba67c4241077
	- just check if each column is sorted lexicographically
- [[2023-01-04 Wednesday]] #Array #[[Hash Table]] #Greedy #Counting 
  problem:: Minimum Rounds to Complete All Tasks
  link:: https://leetcode.com/problems/minimum-rounds-to-complete-all-tasks/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63b37beb-7459-4904-94d8-c4fc09da525b
	- sort the input first
	- count the length of the sequences
	- need to take the last sequence into account
- [[2023-01-05 Thursday]] #Array #Greedy #Sorting 
  problem:: Minimum Number of Arrows to Burst Balloons
  link:: https://leetcode.com/problems/minimum-number-of-arrows-to-burst-balloons/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 3
  id:: 63b4d15f-76d8-401d-8e48-bf1180c38e6f
	- sort the array by each point's ending position
	- compare one point's ending position to other points' starting position
	- even we cannot burst the next balloon but can burst the next next balloon, it's guarantee that the next next balloon can be burst by the next balloon
	- we just need to increase the count when we find a balloon's starting position is bigger than current ending position
- [[2023-01-06 Friday]] #Array #Greedy #Sorting 
  problem:: Maximum Ice Cream Bars
  link:: https://leetcode.com/problems/maximum-ice-cream-bars/description/
  difficulty:: Medium
  duration:: 1 min
  number_of_times:: 1
  id:: 63b6bf32-59ad-4dd6-b15e-d89a34fcfc94
	- just sort the input array
- [[2023-01-07 Saturday]] #Array #Greedy 
  problem:: Gas Station
  link:: https://leetcode.com/problems/gas-station/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 3
  id:: 63b76fd2-ce09-4f70-afcc-76929afb0292
	- start from a gas station, then proceed until we have negative sum
	- start from the next gas station which we got negative sum, it's guarantee the gas stations between these two aren't the answer
	- tried to reduce the runtime through hash table but failed
- [[2023-01-09 Monday]] #Stack #Tree #DFS #[[Binary Tree]] #[[Morris Traversal]] 
  problem:: Binary Tree Preorder Traversal
  link:: https://leetcode.com/problems/binary-tree-preorder-traversal/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 63b8c640-f5df-4c04-9217-943e08cfd42f
	- use morris traversal
	- find the last node in the left subtree and connect it to current node
		- if it's already connected to current node, break the link and go to right subtree
- [[2023-01-10 Tuesday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Same Tree
  link:: https://leetcode.com/problems/same-tree/description/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 3
  id:: 63bb66dd-1911-4930-b555-50b170e073aa
	- use recursive DFS to check both trees
- [[2023-01-12 Thursday]] #[[Hash Table]] #Tree #DFS #BFS #Counting 
  problem:: Number of Nodes in the Sub-Tree With the Same Label
  link:: https://leetcode.com/problems/number-of-nodes-in-the-sub-tree-with-the-same-label/description/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 63bcb789-785a-4ade-b077-2497cb7473ec
	- use DFS
	- return a hash table from each subtree
	- remember to pass string as reference
- [[2023-01-14 Saturday]] #String #[[Union Find]] 
  problem:: Lexicographically Smallest Equivalent String
  link:: https://leetcode.com/problems/lexicographically-smallest-equivalent-string/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63bffe5e-564a-43fa-831f-6158b7baf10e
	- easy union find problem
- [[2023-01-16 Monday]] #Array 
  problem:: Insert Interval
  link:: https://leetcode.com/problems/insert-interval/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 63c216a8-95dc-42d0-ac04-9c1f95e7bfe6
	- insert the new interval into the array and maintain the ascending order
	- merge the intervals by pushing to another array
- [[2023-01-17 Tuesday]] #String #DP 
  problem:: Flip String to Monotone Increasing
  link:: https://leetcode.com/problems/flip-string-to-monotone-increasing/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63c4a18f-0ea5-4dea-b1b1-f5cffc7f5097
	- count for every position, how many steps it takes to make the string monotone
	- find the minimum position
- [[2023-01-20 Friday]] #Array #[[Hash Table]] #Backtracking #[[Bit Manipulation]] 
  problem:: Non-decreasing Subsequences
  link:: https://leetcode.com/problems/non-decreasing-subsequences/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
  id:: 63cab7bf-6d5e-49a8-a72a-6165bc17bb42
	- use backtracking
	- need to avoid picking duplicated sequences, so need to use a hash table to pick the same number only once in each iteration
- [[2023-01-21 Saturday]] #String #Backtracking 
  problem:: Restore IP Addresses
  link:: https://leetcode.com/problems/restore-ip-addresses/description/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 3
  id:: 63cab835-b936-4c15-b613-f8dec27ac379
	- use backtracking
	- need to avoid leading zero number
- [[2023-01-22 Sunday]] #String #DP #Backtracking 
  problem:: Palindrome Partitioning
  link:: https://leetcode.com/problems/palindrome-partitioning/description/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 3
  id:: 63cbfd53-854f-4421-89b8-46339bd19e27
	- use DP to construct a table to lookup palindrome first
	- then use backtracking to find all the partitions
- [[2023-01-23 Monday]] #Array #[[Hash Table]] #Graph 
  problem:: Find the Town Judge
  link:: https://leetcode.com/problems/find-the-town-judge/description/
  difficulty:: Easy
  duration:: 10 mins
  number_of_times:: 1
  id:: 63cd5120-0788-4c48-b19e-f38685afdaea
	- use hash table
	- it's possible that there's no judge, but impossible to have multiple judges
- [[2023-01-24 Tuesday]] #Array #BFS #Matrix 
  problem:: Snakes and Ladders
  link:: https://leetcode.com/problems/snakes-and-ladders/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63ce4853-459c-4dc6-9901-926b020b1dd7
	- use BFS and a hash table
	- need to map the labels to cells in the matrix
- [[2023-01-25 Wednesday]] #DFS #Graph 
  problem:: Find Closest Node to Given Two Nodes
  link:: https://leetcode.com/problems/find-closest-node-to-given-two-nodes/description/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 1
  id:: 63cfa062-b598-459f-ac5b-3ea7684e6b2c
	- use two hash tables
	- may have multiple nodes satisfy the condition
- [[2023-01-26 Thursday]] #DP #DFS #BFS #Graph #Heap #[[Shortest Path]] #[[Bellman-Ford]] 
  problem:: Cheapest Flights Within K Stops
  link:: https://leetcode.com/problems/cheapest-flights-within-k-stops/description/
  difficulty:: Medium
  duration:: 1 hr
  number_of_times:: 2
  id:: 63d24b76-2a2e-4063-9b88-bde6e9d939ca
	- use bellman ford to find the shortest path to destination
	- the times of relaxation cannot exceed `k + 1`
	- need to use another array round to avoid using updated distance
- [[2023-01-30 Monday]] #Math #DP #Memoization 
  problem:: N-th Tribonacci Number
  link:: https://leetcode.com/problems/n-th-tribonacci-number/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 2
  id:: 63d299a6-c798-45d8-ace7-f63cdcfb78ca
	- use an array to store current three numbers
	- move the last two numbers to the front, and add them to the last number
- [[2023-01-31 Tuesday]] #Array #DP #Sorting 
  problem:: Best Team With No Conflicts
  link:: https://leetcode.com/problems/best-team-with-no-conflicts/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63d70a98-ad41-49b0-abf0-61864b1253a7
	- sort each player's by their score
	- use dynamic programming to find the maximum score, when choosing the current player as the last player in the team
-
- [Word Pattern](((63b18658-c0c3-4bb4-8dd8-4f3d075e679d))) can be solved by using two hash table, recording the two way mappings
- [Detect Capital](((63b243f1-cf3b-4c13-a1d7-437bb0ea71a6))) is an easy problem, just need to consider all the cases
- [Delete Columns to Make Sorted](((63b24430-aada-4085-a9f6-ba67c4241077))) is an easy problem
- [Minimum Rounds to Complete All Tasks](((63b37beb-7459-4904-94d8-c4fc09da525b))) can be solved by sorting the array, then count each element
- [Minimum Number of Arrows to Burst Balloons](((63b4d15f-76d8-401d-8e48-bf1180c38e6f))) can be solved by sorting the array by each balloon's ending position first, then count how far we can get by bursting the first balloon on its ending position
- [Maximum Ice Cream Bars](((63b6bf32-59ad-4dd6-b15e-d89a34fcfc94))) is an easy problem
- [Gas Station](((63b76fd2-ce09-4f70-afcc-76929afb0292))) can be solved by greedy in $O(n^2)$, but it's possible to solve it using two pointers in $O(n)$
- [Binary Tree Preorder Traversal](((63b8c640-f5df-4c04-9217-943e08cfd42f))) can be solved by using morris traversal
- [Same Tree](((63bb66dd-1911-4930-b555-50b170e073aa))) is an easy DFS problem
- [Number of Nodes in the Sub-Tree With the Same Label](((63bcb789-785a-4ade-b077-2497cb7473ec))) can be solved by recursive DFS
- [Lexicographically Smallest Equivalent String](((63bffe5e-564a-43fa-831f-6158b7baf10e))) is an easy union find problem
- [Insert Interval](((63c216a8-95dc-42d0-ac04-9c1f95e7bfe6))) can be solved by first pushing the new interval to the right position
- [Flip String to Monotone Increasing](((63c4a18f-0ea5-4dea-b1b1-f5cffc7f5097))) can be solved by finding the flip count for every position first
- [Non-decreasing Subsequences](((63cab7bf-6d5e-49a8-a72a-6165bc17bb42))) can be solved by backtracking, but need to also use a hash table to avoid duplicated sequences
- [Restore IP Addresses](((63cab835-b936-4c15-b613-f8dec27ac379))) can be solved by using backtracking
- [Palindrome Partitioning](((63cbfd53-854f-4421-89b8-46339bd19e27))) can be solved by using DP and backtracking
- [Find the Town Judge](((63cd5120-0788-4c48-b19e-f38685afdaea))) is an easy hash table problem
- [Snakes and Ladders](((63ce4853-459c-4dc6-9901-926b020b1dd7))) can be solved by using BFS, but need to remember to map the label to the cell in the matrix
- [Find Closest Node to Given Two Nodes](((63cfa062-b598-459f-ac5b-3ea7684e6b2c))) can be solved by using two hash tables
- [Cheapest Flights Within K Stops](((63d24b76-2a2e-4063-9b88-bde6e9d939ca))) can be solved by different shortest path algorithm, but need to remember the limitation of k
- [N-th Tribonacci Number](((63d299a6-c798-45d8-ace7-f63cdcfb78ca))) is an easy DP problem
- [Best Team With No Conflicts](((63d70a98-ad41-49b0-abf0-61864b1253a7))) can be solved by sorting the players' score first, then use DP to find the maximum score for each team composition