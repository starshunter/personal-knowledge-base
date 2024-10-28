title:: LeetCode Daily Challenge/2022-10

- 8 easy, 14 medium, 0 hard
- 10 problems were solved for the first time
- [[2022-10-01 Saturday]] #String #DP 
  problem:: Decode Ways
  link:: https://leetcode.com/problems/decode-ways/description/
  difficulty:: Medium
  duration:: 3
  number_of_times:: 10 mins
  id:: 63378b90-611c-4511-a6aa-8f4ad4584997
	- use DP
	- if there's 0 decode way with current position as the end, we should return 0
- [[2022-10-02 Sunday]] #DP 
  problem:: Number of Dice Rolls With Target Sum
  link:: https://leetcode.com/problems/number-of-dice-rolls-with-target-sum/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 1
  id:: 63378bed-2c1b-4813-b45c-2bca1069fb63
	- use DP
	- store how many ways to get the given value with the given coins
- [[2022-10-03 Monday]] #Array #String #DP #Greedy 
  problem:: Minimum Time to Make Rope Colorful
  link:: https://leetcode.com/problems/minimum-time-to-make-rope-colorful/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 6338e971-1973-40fe-bfb2-8f404a873959
	- use greedy
	- for every group of consecutive balloons with the same colors, we only left the balloons with the longest removal time and remove others
- [[2022-10-04 Tuesday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Path Sum
  link:: https://leetcode.com/problems/path-sum/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 633aca97-1817-4cce-9a59-0b6e1f43702c
	- use BFS
- [[2022-10-05 Wednesday]] #Tree #DFS #BFS #[[Binary Tree]] 
  problem:: Add One Row to Tree
  link:: https://leetcode.com/problems/add-one-row-to-tree/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 633c2bb4-2e4e-4881-b56d-94cffc3285e0
	- use BFS
- [[2022-10-08 Saturday]] #Array #[[Two Pointers]] #Sorting 
  problem:: 3Sum Closest
  link:: https://leetcode.com/problems/3sum-closest/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 633d85e2-ad46-4700-80e2-ae357bb11672
	- sort the array, then use two pointers and binary search
	- because we are calculating the absolute difference, we need to consider the previous element of the number we find using binary search
	- it can be solved using two pointers only
- [[2022-10-09 Sunday]] #[[Hash Table]] #[[Two Pointers]] #Tree #DFS #BFS #[[Binary Search Tree]] #[[Binary Tree]] 
  problem:: Two Sum IV - Input is a BST
  link:: https://leetcode.com/problems/two-sum-iv-input-is-a-bst/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 2
  id:: 6340d338-93f0-48f6-a412-1dbcd5837d8f
	- use a hash table and DFS
	- basically the same as the original two sum problem, but instead we need to use DFS in this one
- [[2022-10-10 Monday]] #String #Greedy 
  problem:: Break a Palindrome
  link:: https://leetcode.com/problems/break-a-palindrome/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 2
  id:: 63422056-6c44-4788-b788-b1e861f9f68b
	- change the first non a character to a, but remember to skip the middle character
	- change the last character to b if the string only has a
- [[2022-10-11 Tuesday]] #Array #Greedy 
  problem:: Increasing Triplet Subsequence
  link:: https://leetcode.com/problems/increasing-triplet-subsequence/description/
  difficulty:: Medium
  duration:: 3 mins
  number_of_times:: 3
  id:: 63436abf-e2b3-439c-9992-f1024cf842db
	- use two variables to store the minimum value of the smallest ending number of increasing sequence
- [[2022-10-12 Wednesday]] #Array #Math #Greedy #Sorting 
  problem:: Largest Perimeter Triangle
  link:: https://leetcode.com/problems/largest-perimeter-triangle/description/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 1
  id:: 634552e7-e8a0-4730-8f17-bcc862e2d0b4
	- sort the array to be decreasing
	- then start from the biggest number, and check whether it can form a triangle with the next two numbers
- [[2022-10-13 Thursday]] #[[Linked List]] 
  problem:: Delete Node in a Linked List
  link:: https://leetcode.com/problems/delete-node-in-a-linked-list/description/
  difficulty:: Medium
  duration:: 1 min
  number_of_times:: 2
  id:: 6346b979-f8f0-4b22-8aba-b6a3d1bd7a6c
	- just replace current node's value with next node's value
	- skip the next node
- [[2022-10-14 Friday]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Delete the Middle Node of a Linked List
  link:: https://leetcode.com/problems/delete-the-middle-node-of-a-linked-list/description/
  difficulty:: Medium
  duration:: 3 mins
  number_of_times:: 1
  id:: 63480064-a3f0-4a3d-b336-fdb620648cd8
	- use two pointers
- [[2022-10-17-monday]] #[[Hash-table]] #String 
  problem:: Check if the Sentence Is Pangram
  link:: https://leetcode.com/problems/check-if-the-sentence-is-pangram/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 634ca665-c417-4897-bd2a-381680f32cb8
	- use hash table
	- use a number to replace hash table to save space
- [[2022-10-18 Tuesday]] #String 
  problem:: Count and Say
  link:: https://leetcode.com/problems/count-and-say/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 634ca6bf-a707-480b-b640-1fc232e249a6
	- use iterative approach to construct the string one by one
	- it's impossible to have 0 in the string
- [[2022-10-19 Wednesday]] #[[Hash Table]] #String #Trie #Sorting #Heap #[[Bucket Sort]] #Counting #[[Priority Queue]] 
  problem:: Top K Frequent Words
  link:: https://leetcode.com/problems/top-k-frequent-words/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 634df7b5-7cb0-42c1-902c-9f300a0e56ea
	- use hash table and min heap
- [[2022-10-20 Thursday]] #[[Hash Table]] #Math #String 
  problem:: Integer to Roman
  link:: https://leetcode.com/problems/integer-to-roman/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 63516902-b132-42a6-9b2a-dcf6414fd0e1
	- construct a hash table in descending order
	- divided the target number using the element in the hash table, and see how many times the target number need to use the element
	- because the hash table is in descending order, we can easily handle 4 and 9 cases
		- numbers over 4 are also the same
- [[2022-10-21 Friday]] #Array #[[Hash Table]] #[[Sliding Window]] 
  problem:: Contains Duplicate II
  link:: https://leetcode.com/problems/contains-duplicate-ii/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 63516a10-4ac0-451c-9f1e-3ff69b0a528b
	- use a hash table and sliding window
	- remember to remove the number first than check for duplicate
- [[2022-10-23 Sunday]] #Array #[[Hash Table]] #[[Bit Manipulation]] #Sorting 
  problem:: Set Mismatch
  link:: https://leetcode.com/problems/set-mismatch/description/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 1
  id:: 6352db94-732b-4be0-8206-6d85b46a96c9
	- use negative numbers to indicate the index has been seen
	- need another iteration to check for positive number
- [[2022-10-24 Monday]] #Array #String #Backtracking #[[Bit Manipulation]] 
  problem:: Maximum Length of a Concatenated String with Unique Characters
  link:: https://leetcode.com/problems/maximum-length-of-a-concatenated-string-with-unique-characters/description/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 1
  id:: 6354d7fe-ce8c-4abf-9121-3bee6a4da946
	- use binary bits to represent the existence of a character in a string
	- remove strings with duplicate characters
	- use backtracking to find the answer
- [[2022-10-25 Tuesday]] #Array #String 
  problem:: Check If Two String Arrays are Equivalent
  link:: https://leetcode.com/problems/check-if-two-string-arrays-are-equivalent/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 6356772c-40c0-47be-bcde-16a757800d2b
	- use four pointers
	- be careful of the edge cases
- [[2022-10-28 Friday]] #Array #[[Hash Table]] #String #Sorting 
  problem:: Group Anagrams
  link:: https://leetcode.com/problems/group-anagrams/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 635a7a28-157c-441a-adf2-b0464da8a2b3
	- use counting sort to sort each string, and use a hash table to record anagrams
- [[2022-10-31 Monday]] #Array #Matrix 
  problem:: Toeplitz Matrix
  link:: https://leetcode.com/problems/toeplitz-matrix/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 635b26bb-7d4c-4f1d-bc92-213d88cc1bf4
	- start from every number in the first row and the first column, check all diagonals
- [Decode Ways](((63378b90-611c-4511-a6aa-8f4ad4584997))) is an easy DP problem
- [Number of Dice Rolls With Target Sum](((63378bed-2c1b-4813-b45c-2bca1069fb63))) can be solved by using DP, and we can further reduce the space to only one array
- [Minimum Time to Make Rope Colorful](((6338e971-1973-40fe-bfb2-8f404a873959))) can be solved by greedy method, remove consecutive balloons with the same color but leave one of it
- [Path Sum](((633aca97-1817-4cce-9a59-0b6e1f43702c))) is an easy BFS problem
- [Add One Row to Tree](((633c2bb4-2e4e-4881-b56d-94cffc3285e0))) can be solved by both BFS and DFS
- [3Sum Closest](((633d85e2-ad46-4700-80e2-ae357bb11672))) can be solved by using two pointers and binary search
- [Two Sum IV - Input is a BST](((6340d338-93f0-48f6-a412-1dbcd5837d8f))) is a simple DFS problem
- [Break a Palindrome](((63422056-6c44-4788-b788-b1e861f9f68b))) can be solved once realize how to break a palindrome
- [Increasing Triplet Subsequence](((63436abf-e2b3-439c-9992-f1024cf842db))) is an easy greedy problem
- [Largest Perimeter Triangle](((634552e7-e8a0-4730-8f17-bcc862e2d0b4))) is an easy sorting problem
- [Delete Node in a Linked List](((6346b979-f8f0-4b22-8aba-b6a3d1bd7a6c))) is a very easy problem
- [Delete the Middle Node of a Linked List](((63480064-a3f0-4a3d-b336-fdb620648cd8))) is an easy two pointers problem
- [Check if the Sentence Is Pangram](((634ca665-c417-4897-bd2a-381680f32cb8))) is an easy hash table problem
- [Count and Say](((634ca6bf-a707-480b-b640-1fc232e249a6))) can be solved by constructing the string one by one
- [Top K Frequent Words](((634df7b5-7cb0-42c1-902c-9f300a0e56ea))) can be solved by using hash table and min heap
- [Integer to Roman](((63516902-b132-42a6-9b2a-dcf6414fd0e1))) can be solved by constructing a descending hash table, than construct the target number one by one
- [Contains Duplicate II](((63516a10-4ac0-451c-9f1e-3ff69b0a528b))) can be solved by using a hash table and sliding window
- [Set Mismatch](((6352db94-732b-4be0-8206-6d85b46a96c9))) can solved by using two iterations
- [Maximum Length of a Concatenated String with Unique Characters](((6354d7fe-ce8c-4abf-9121-3bee6a4da946))) can be solved by using backtracking and bit manipulation
- [Check If Two String Arrays are Equivalent](((6356772c-40c0-47be-bcde-16a757800d2b))) is an easy problem
- [Group Anagrams](((635a7a28-157c-441a-adf2-b0464da8a2b3))) can be solved by doing counting sort on each string
- [Toeplitz Matrix](((635b26bb-7d4c-4f1d-bc92-213d88cc1bf4))) can be solved by checking every number's equality with its bottom left number