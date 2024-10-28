title:: LeetCode Daily Challenge/2022-06

- 5 easy, 17 medium, 3 hard
- 15 problems were solved for the first time
- [[2022-06-01 Wednesday]] #Array #[[Prefix Sum]] 
  id:: 6296b079-b2d2-4b64-a16d-450c13eccbb4
  problem:: Running Sum of 1d Array
  link:: https://leetcode.com/problems/running-sum-of-1d-array/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 1
  collapsed:: true
	- easy
	- we can solve it without using extra space
- [[2022-06-02 Thursday]] #Array #Matrix #Simulation
  id:: 6297b175-3783-4644-a017-00121dbe5a25
  problem:: Transpose Matrix
  link:: https://leetcode.com/problems/transpose-matrix/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 1
  collapsed:: true
	- easy, just use additional space
- [[2022-06-03 Friday]] #Array #Design #Matrix #[[Prefix Sum]] 
  problem:: Range Sum Query 2D - Immutable
  link:: https://leetcode.com/problems/range-sum-query-2d-immutable/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
  id:: 629969bd-4439-4d52-909e-c3287f70bc2f
  collapsed:: true
	- an easy 2D prefix sum problem
- [[2022-06-04 Saturday]] #Array #Backtracking 
  problem:: N-Queens
  link:: https://leetcode.com/problems/n-queens/
  difficulty:: Hard
  duration:: 25 mins
  number_of_times:: 1
  id:: 629abba3-1adf-4d07-98c9-501cf93d5c47
  collapsed:: true
	- simple backtracking problem
	- need to check the same column, and both diagonals
- [[2022-06-05 Sunday]] #Backtracking 
  id:: 629abc22-e9dc-4b31-b1f9-e09d9df651a3
  problem:: N-Queens II
  link:: https://leetcode.com/problems/n-queens-ii/
  difficulty:: Hard
  duration:: 15 mins
  number_of_times:: 1
  collapsed:: true
	- simple backtracking problem
	- we don't need to actual simulate the board, we just need to record the previous queens' position
	- check current position with previous queens' position to see if they are on the same column or diagonal
- [[2022-06-06 Monday]] #[[Hash Table]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Intersection of Two Linked Lists
  link:: https://leetcode.com/problems/intersection-of-two-linked-lists/
  difficulty:: Easy
  duration:: 10 mins
  number_of_times:: 3
  id:: 629c0d4d-7860-43fe-b0b8-6a3e57b26b8e
  collapsed:: true
	- use two pointers
	- reset the current pointer to another head when it reaches the end
- [[2022-06-07 Tuesday]] #Array #[[Two Pointers]] #Sorting 
  problem:: Merge Sorted Array
  link:: https://leetcode.com/problems/merge-sorted-array/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 629d4a69-6f3b-43bd-b84f-8c27eaafa88f
  collapsed:: true
	- use two pointers
	- construct the answer from the back
- [[2022-06-08 Wednesday]] #Array #String 
  problem:: Remove Palindromic Subsequences
  link:: https://leetcode.com/problems/remove-palindromic-subsequences/
  difficulty:: Easy
  duration:: 10 mins
  number_of_times:: 1
  id:: 629f73bf-f1bd-4e13-b7d6-3a3ff48d0062
	- for any given string, we only need a maximum of two operations to remove it all
	- if the string is not a palindrome, we can just remove all instances of one of the character, then the remaining string will contain only another character
- [[2022-06-09 Thursday]] #Array #[[Two Pointers]] #[[Binary Search]] 
  problem:: Two Sum II - Input Array Is Sorted
  link:: https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/
  difficulty:: Medium
  duration:: 2 mins
  number_of_times:: 3
  id:: 62a0ce40-4df8-4c52-8286-19cf7e0f5f13
	- easy two pointers problem
- [[2022-06-10 Friday]] #[[Hash Table]] #String #[[Sliding Window]] 
  problem:: Longest Substring Without Repeating Characters
  link:: https://leetcode.com/problems/longest-substring-without-repeating-characters/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62a209c0-6ac9-4099-a09f-c30ccf4fcdbe
	- use a bit set as hash table, then use sliding windows to find the longest substring
	- remember to reset the characters before left pointer
- [[2022-06-11 Saturday]] #Array #[[Hash Table]] #[[Binary Search]] #[[Sliding Window]] #[[Prefix Sum]] 
  problem:: Minimum Operations to Reduce X to Zero
  link:: https://leetcode.com/problems/minimum-operations-to-reduce-x-to-zero/
  difficulty:: Medium
  duration:: 1 hr
  number_of_times:: 1
  id:: 62a3ff30-2aad-44ac-aece-d43ed2954b0f
	- tried to use 2D DP but got TLE
	- see discussion
	- use prefix sum and hash table
	- store prefix sum into hash table, then find if there's a prefix sum in the hash table that can help us reach the target
- [[2022-06-12 Sunday]] #Array #[[Hash Table]] #[[Sliding Window]] 
  problem:: Maximum Erasure Value
  link:: https://leetcode.com/problems/maximum-erasure-value/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 62a4000f-15b3-43de-a935-3a57fcc33b8d
	- easy two pointers problem
	- need to use a hash table to tract subarray's number appearance
- [[2022-06-13 Monday]] #Array #DP 
  id:: 62a54874-f2af-4564-95d7-eb5c6ba2b863
  problem:: Triangle
  link:: https://leetcode.com/problems/triangle/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 3
	- bottom-up DP
	- no need to use extra space
- [[2022-06-14 Tuesday]] #String #DP 
  problem:: Delete Operation for Two Strings
  link:: https://leetcode.com/problems/delete-operation-for-two-strings/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
  id:: 62a7d80b-a589-4822-ac36-efb4ad21e6b5
	- a DP problem
	- use two one-dimensional array
	- calculate how many steps it takes from one state to another state
	- the base case is when one of the string is empty
- [[2022-06-15 Wednesday]] #Array #[[Hash Table]] #[[Two Pointers]] #String #DP 
  problem:: Longest String Chain
  link:: https://leetcode.com/problems/longest-string-chain/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 62a8a544-5cf9-43b9-9a49-ff1c2b45dc91
	- we can find all the predecessor of a string by removing one of its character
	- we can use a hash table to store the maximum length of a word chain, with the ending word as the key
	- we can use the predecessor we have constructed and the hash table to quickly find out the maximum length of the word chain ending with current word
- [[2022-06-16 Thursday]] #String #DP 
  problem:: Longest Palindromic Substring
  link:: https://leetcode.com/problems/longest-palindromic-substring/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62aa0ee4-563b-41d1-886f-08983d8500f1
	- use two pointers to expand from substrings' center
- [[2022-06-19 Sunday]] #Array #String #Trie 
  problem:: Search Suggestions System
  link:: https://leetcode.com/problems/search-suggestions-system/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 1
  id:: 62acada9-7f1a-4892-8492-3c7821343653
  collapsed:: true
	- use trie
	- store suggestions in each trie node
- [[2022-06-21 Tuesday]] #Array #Greedy #Heap 
  problem:: Furthest Building You Can Reach
  link:: https://leetcode.com/problems/furthest-building-you-can-reach/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 62ae87e4-333a-4e01-816f-47db5132e38f
	- this is a greedy problem
	- we use the ladders between buildings with the most significant height difference
	- maintain a priority queue with length of number of ladders
	- we have to use bricks on the remaining difference, once the bricks are not enough, we have found the answer
- [[2022-06-22 Wednesday]] #Array #[[Divide and Conquer]] #Sorting #Heap #[[Quick Select]] 
  problem:: Kth Largest Element in an Array
  link:: https://leetcode.com/problems/kth-largest-element-in-an-array/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 62b11611-f766-40ad-9322-f2688548b68c
	- maintain a min-heap of size k
	  id:: 446fbbd0-058f-4d5f-a04a-99e6cb3ccf14
- [[2022-06-23 Thursday]]
  problem:: Course Schedule III
  link:: https://leetcode.com/problems/course-schedule-iii/
  difficulty:: Hard
  duration:: 40 mins
  number_of_times:: 1
  id:: 62b26771-5b93-4358-97ae-3cabefad4b86
	- a greedy problem
	- we need to sort the courses with their ending date first
	- then maintain a priority queue of the courses' duration
	- iterate through the courses and keep updating current date, if we find a course that is too late to take, but there is a course we have taken that is longer than it, we can drop that course and take this course
		- because by doing this, we will have a smaller current ending date
- [[2022-06-25 Saturday]] #Array 
  problem:: Non-decreasing Array
  link:: https://leetcode.com/problems/non-decreasing-array/
  difficulty:: Medium
  duration:: 25 mins
  number_of_times:: 1
  id:: 62b3bb73-dd66-4d11-b31f-099910c1ff58
	- calculate if it is a non-decreasing array from the front and from the back for every position
	- iterate through the array and try to connect two non-decreasing arrays
- [[2022-06-26 Sunday]] #Array #[[Sliding Window]] #[[Prefix Sum]] 
  problem:: Maximum Points You Can Obtain from Cards
  link:: https://leetcode.com/problems/maximum-points-you-can-obtain-from-cards/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 62b7bcd5-c2a9-4d97-bddb-3b6f46be47be
	- calculate the sum of the array first
	- maintain an interval and its sum
	- move that interval and find the maximum answer
	  id:: 62b7c414-41f1-405c-9fd5-b5e17618f681
- [[2022-06-27 Monday]] #String #Greedy 
  problem:: Partitioning Into Minimum Number Of Deci-Binary Numbers
  link:: https://leetcode.com/problems/partitioning-into-minimum-number-of-deci-binary-numbers/
  difficulty:: Medium
  duration:: 1 min
  number_of_times:: 1
  id:: 62b7c421-c1f2-4541-aeb6-6b35d85c351e
	- easy, just find the biggest digit
- [[2022-06-28 Tuesday]]
  id:: 62b9c6b7-21dd-4bfa-9ac3-5c2a6a885023
  problem:: Minimum Deletions to Make Character Frequencies Unique
  link:: https://leetcode.com/problems/minimum-deletions-to-make-character-frequencies-unique/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
	- count the character frequency first
	- then sort the array
	- use two level iterations to find the answer
	- it's solvable with one iteration, or using priority queue
- [[2022-06-30 Thursday]] #Array #Math #Sorting 
  problem:: Minimum Moves to Equal Array Elements II
  link:: https://leetcode.com/problems/minimum-moves-to-equal-array-elements-ii/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62ba4d0c-a078-48bd-8162-71140aaa3583
	- find the medium and calculate the total differences
	- we don't need to find the medium, just remember we need to make a pair of numbers become the same
- [Running Sum of 1d Array](((6296b079-b2d2-4b64-a16d-450c13eccbb4))) is very easy
- [Transpose Matrix](((6297b175-3783-4644-a017-00121dbe5a25))) is very easy
- [Range Sum Query 2D - Immutable](((629969bd-4439-4d52-909e-c3287f70bc2f))) is an easy 2D prefix sum problem, and maybe we don't need to use extra space
- [N-Queens](((629abba3-1adf-4d07-98c9-501cf93d5c47))) is a simple backtracking problem
- [N-Queens II](((629abc22-e9dc-4b31-b1f9-e09d9df651a3))) is a simple backtracking problem, and we only need to store the information about queens' position
- [Intersection of Two Linked Lists](((629c0d4d-7860-43fe-b0b8-6a3e57b26b8e))) is a simple two pointers problem
- [Merge Sorted Array](((629d4a69-6f3b-43bd-b84f-8c27eaafa88f))) is an easy two pointers problem, but the key is to construct the answer from the back
- [Remove Palindromic Subsequences](((629f73bf-f1bd-4e13-b7d6-3a3ff48d0062))) is a brain teaser, use the fact that the string only contains two types of character
- [Two Sum II - Input Array Is Sorted](((62a0ce40-4df8-4c52-8286-19cf7e0f5f13))) is a very easy two pointers problem
  id:: 633d85e0-f2f7-40fa-a3b7-fa30eb9f24c1
- [Longest Substring Without Repeating Characters](((62a209c0-6ac9-4099-a09f-c30ccf4fcdbe))) is a sliding window problem, and we can replace the hash table with a bit set
- [Minimum Operations to Reduce X to Zero](((62a3ff30-2aad-44ac-aece-d43ed2954b0f))) need to be solved using a combination of prefix sum and hash table
- [Maximum Erasure Value](((62a4000f-15b3-43de-a935-3a57fcc33b8d))) is an easy two pointers problem
- [Triangle](((62a54874-f2af-4564-95d7-eb5c6ba2b863))) is a bottom up DP problem, but we can solve it only using the given space
- [Delete Operation for Two Strings](((62a7d80b-a589-4822-ac36-efb4ad21e6b5))) is a DP problem, the state of this problem is the steps it takes from one substring to another substring
- [Longest String Chain](((62a8a544-5cf9-43b9-9a49-ff1c2b45dc91))) is a DP problem, but it requires a small trick about constructing the predecessor, and using an array will cause TLE, use hash table instead
- [Longest Palindromic Substring](((62aa0ee4-563b-41d1-886f-08983d8500f1))) is a two pointers problem
- [Search Suggestions System](((62acada9-7f1a-4892-8492-3c7821343653))) is a trie problem, be we can also solve it using binary search
  id:: 62ae87e7-91af-48ec-8e3f-4dd6966de37c
- [Furthest Building You Can Reach](((62ae87e4-333a-4e01-816f-47db5132e38f))) is a greedy problem that can be solved with a priority queue
- [Kth Largest Element in an Array](((62b11611-f766-40ad-9322-f2688548b68c))) can be solved using a min-heap, but we can save some space using quick select
- [Course Schedule III](((62b26771-5b93-4358-97ae-3cabefad4b86))) is an interesting greedy problem, it requires us to sort the array and maintain a priority queue
- [Non-decreasing Array](((62b3bb73-dd66-4d11-b31f-099910c1ff58))) uses a similar idea of prefix sum
- [Maximum Points You Can Obtain from Cards](((62b7bcd5-c2a9-4d97-bddb-3b6f46be47be))) can be solved using sliding window or prefix sum
  id:: 62b7c425-9cc7-4178-98c3-47139158e4b6
- [Partitioning Into Minimum Number Of Deci-Binary Numbers](((62b7c421-c1f2-4541-aeb6-6b35d85c351e))) is very easy
- [Minimum Deletions to Make Character Frequencies Unique](((62b9c6b7-21dd-4bfa-9ac3-5c2a6a885023))) can be solved by sorting the frequency array, but one level iteration is enough
- [Minimum Moves to Equal Array Elements II](((62ba4d0c-a078-48bd-8162-71140aaa3583))) can be solved without actually finding the medium