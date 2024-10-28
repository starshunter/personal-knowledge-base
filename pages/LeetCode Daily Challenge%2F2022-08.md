title:: LeetCode Daily Challenge/2022-08

- 9 easy, 12 medium, 4 hard
- 9 problems were solved for the first time
- [[2022-08-01 Monday]] #Math #DP #Combinatorics 
  problem:: Unique Paths
  link:: https://leetcode.com/problems/unique-paths/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 4
  id:: 62e722bf-8106-4ceb-bf2f-b507baf2cc98
	- implemented math solution
	- remember to subtract one from both sides
- [[2022-08-02 Tuesday]] #Array #[[Binary Search]] #Sorting #Heap #Matrix
  id:: 62e72331-3e40-44a5-b869-240732ebebeb
  problem:: Kth Smallest Element in a Sorted Matrix
  link:: https://leetcode.com/problems/kth-smallest-element-in-a-sorted-matrix/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
	- do binary search on the answer space
	- we can guarantee the final answer we get is in the matrix
	  collapsed:: true
		- otherwise the binary search should continue
		- The `lo` we returned is guaranteed to be an element in the matrix is because:Let us assume element `m` is the kth smallest number in the matrix, and `x` is the number of element m in the matrix. When we are about to reach convergence, if `mid=m-1` , its `count` value (the number of elements which are <= mid) would be `k-x` , so we would set lo as `(m-1)+1=m` , in this case the `hi` will finally reach `lo` ; and if `mid=m+1` , its `count` value would be `k+x-1` , so we would set `hi` as `m+1` , in this case the lo will finally reach `m` .To sum up, because the number `lo` found by binary search find is exactly the element which has k number of elements in the matrix that are <= `lo` , The equal sign guarantees there exists and only exists one number in range satisfying this condition. So `lo` must be the only element satisfying this element in the matrix.
- [[2022-08-03 Wednesday]] #[[Binary Search]] #Design #[[Segment Tree]] #[[Ordered Set]]
  problem:: My Calendar I
  link:: https://leetcode.com/problems/my-calendar-i/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 1
  id:: 62e87482-0e2d-4287-b9c1-e88169dcd2f7
	- use ordered map and do binary search
	- remember `lower_bound` will return the smallest element that is equal or greater than the target
- [[2022-08-05 Friday]] #Array #DP
  problem:: Combination Sum IV
  link:: https://leetcode.com/problems/combination-sum-iv/
  difficulty:: Medium
  duration:: 20 mins
  number_of_times:: 2
  id:: 62ecc823-717d-4573-9983-4634c1695f7b
	- use DP, kind of like knapsack problem
	- use `unsigned int` because its overflow behavior is defined
- [[2022-08-06 Saturday]] #Math #DP #Combinatorics
  problem:: Poor Pigs
  link:: https://leetcode.com/problems/poor-pigs/
  difficulty:: Hard
  duration:: 1 hr
  number_of_times:: 1
  id:: 62eccebc-2a8e-45fc-bf83-7c5c1e490fbf
	- a math problem
	- encode each bucket with different based number
- [[2022-08-07 Sunday]] #DP
  problem:: Count Vowels Permutation
  link:: https://leetcode.com/problems/count-vowels-permutation/
  difficulty:: Hard
  duration:: 10 mins
  number_of_times:: 1
  id:: 62edcc7b-9632-464b-896a-ff7eab4bb098
	- easy after finding out the pattern
	- number of strings with certain length can be inferenced by the number of string with certain length minus one
- [[2022-08-08 Monday]] #Array #[[Binary Search]] #DP
  problem:: Longest Increasing Subsequence
  link:: https://leetcode.com/problems/longest-increasing-subsequence/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 62ef1c0c-cf23-4086-896e-7c8ec3536c92
	- use binary search
	- the idea is not maintaining an array that represents the answer during the process, but make sure this array can tell you the length of the longest increasing subsequence
	- if current number is bigger than the number at the end of the array, then append it
	- it it's not, use binary search to find the appropriate position to insert it, so that in the future we may have a smaller number at the end of the array, so it's easier to extend the array
- [[2022-08-10 Wednesday]] #Array #[[Divide and Conquer]]  #[[Tree]] #[[Binary Search Tree]] #[[Binary Tree]] 
  problem:: Convert Sorted Array to Binary Search Tree
  link:: https://leetcode.com/problems/convert-sorted-array-to-binary-search-tree/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 3
  id:: 62f26976-9cb5-4491-bbba-023fe8c56f97
	- easy using recursion
	- choose the middle element as the root in every round, then construct left and right subtree using the remaining array
- [[2022-08-11 Thursday]] #Tree #DFS #BFS #[[Binary Tree]] # [[In-order Traversal]] 
  problem:: Validate Binary Search Tree
  link:: https://leetcode.com/problems/validate-binary-search-tree/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 2
  id:: 62f5474f-a6ef-415d-81ae-132f257fdea2
	- use iterative in-order traversal
	- use a variable to record previously visited node
- [[2022-08-12 Friday]] #Tree #DFS #[[Binary Search Tree]] #[[Binary Tree]] 
  problem:: Lowest Common Ancestor of a Binary Search Tree
  link:: https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 2
  id:: 62f599a6-ea14-47ee-9106-2138f3339b22
	- use iterative DFS
	- compare two targets with current node
		- if one of the node equals to current node, then return current node
		- if two targets exists in two different subtrees, then return current node
- [[2022-08-13 Saturday]] #[[Hash Table]] #String #[[Sliding Window]] 
  problem:: Substring with Concatenation of All Words
  link:: https://leetcode.com/problems/substring-with-concatenation-of-all-words/
  difficulty:: Hard
  duration:: 1 hr
  number_of_times:: 1
  id:: 62f6012f-61f5-4e1a-a272-dcaa7fb19af4
	- use two hash tables to test each starting point
- [[2022-08-15 Monday]] #[[Hash Table]] #Math #String 
  problem:: Roman to Integer
  link:: https://leetcode.com/problems/roman-to-integer/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 3
  id:: 62f71515-26e7-47b3-b911-bf2a1f6886a0
	- use a hash table to record the mapping
	- iterate from the back, if we find a symbol that is smaller than the next one, then we subtract its number from the total value
- [[2022-08-16 Tuesday]] #[[Hash Table]] #String #Queue #Counting 
  problem:: First Unique Character in a String
  link:: https://leetcode.com/problems/first-unique-character-in-a-string/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 2
  id:: 62fa5468-1688-4210-89b7-f3ea44ee126b
	- easy using a hash table to record each character's occurrence
- [[2022-08-17 Wednesday]] #Array #[[Hash Table]] #String 
  problem:: Unique Morse Code Words
  link:: https://leetcode.com/problems/unique-morse-code-words/
  difficulty:: Easy
  duration:: 3 mins
  number_of_times:: 2
  id:: 62fb9689-ef93-42df-83f9-e2c010a7f4d3
	- use two hash tables to store the mapping and the transformations
- [[2022-08-18 Thursday]] #Array #[[Hash Table]] #Greedy #Sorting #Heap 
  problem:: Reduce Array Size to The Half
  link:: https://leetcode.com/problems/reduce-array-size-to-the-half/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 62fcf06b-d288-44e2-834b-75edc7fef6d6
	- use a hash table to store the occurrences
	- sort the occurrences and start to reduce array size by deleting number with most occurrences
- [[2022-08-19 Friday]] #Array #[[Hash Table]] #Greedy #Heap 
  problem:: Split Array into Consecutive Subsequences
  link:: https://leetcode.com/problems/split-array-into-consecutive-subsequences/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 1
  id:: 62fe46fa-653a-4cb3-b45f-eb1edb6e580e
	- no idea, see discussion
	- maintain the information of how many string ending at a certain position with a certain length
	- use this information, iterate through the array and update it
- [[2022-08-20 Saturday]] #Array #DP #Greedy #Heap 
  problem:: Minimum Number of Refueling Stops
  link:: https://leetcode.com/problems/minimum-number-of-refueling-stops/
  difficulty:: Hard
  duration:: 1 hr
  number_of_times:: 1
  id:: 62ff7779-8a61-4b27-b26c-16c95b5594e3
	- use DP
	- treat the farthest position of stopping at different number of gas station as subproblem
- [[2022-08-22 Monday]] #Math #[[Bit Manipulation]] #Recursion 
  problem:: Power of Four
  link:: https://leetcode.com/problems/power-of-four/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 2
  id:: 63004b49-9cc9-4dc0-8639-18cf701eafc3
	- divide the number by 4 until it's not dividable, and check if it equals to 1
- [[2022-08-23 Tuesday]] #[[Linked List]] #[[Two Pointers]] #Stack #Recursion 
  problem:: Palindrome Linked List
  link:: https://leetcode.com/problems/palindrome-linked-list/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 63039a20-176a-41f0-b78e-4a54eb761113
	- use two pointers to find the middle of the linked list, and the node before it
	- then reverse second half of the linked list
		- remember to unlink the middle node and its previous node
	- traverse from two ends and check the equality
- [[2022-08-24 Wednesday]] #Math #Recursion 
  problem:: Power of Three
  link:: https://leetcode.com/problems/power-of-three/
  difficulty:: Easy
  duration:: 30 mins
  number_of_times:: 2
  id:: 6304d1c7-f3e5-4345-a7db-d654e45c9e0a
	- use log
	- remember to do the rounding, and handle the floating point precision problem
- [[2022-08-25 Thursday]] #[[Hash Table]] #String #Counting 
  problem:: Ransom Note
  link:: https://leetcode.com/problems/ransom-note/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 3
  id:: 63076e14-e9d6-4d36-b9cd-4e8e6988ee47
	- easy using an array to count character appearance
- [[2022-08-26 Friday]] #Math #Sorting #Counting #Enumeration 
  problem:: Reordered Power of 2
  link:: https://leetcode.com/problems/reordered-power-of-2/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 6307741e-6948-483d-b832-598d131b0535
	- use counting for each power of 2
	- then use counting for the input then compare it to each power of 2
- [[2022-08-28 Sunday]] #Array #Sorting #Matrix 
  problem:: Sort the Matrix Diagonally
  link:: https://leetcode.com/problems/sort-the-matrix-diagonally/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 1
  id:: 63089ce4-a870-42c7-b790-0d98b2883c8e
	- do bubble sort on each diagonal
- [[2022-08-29 Monday]] #Array #DFS #BFS #[[Union Find]] #Matrix 
  problem:: Number of Islands
  link:: https://leetcode.com/problems/number-of-islands/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 630acb8a-b385-4598-b954-712077c4fc7c
	- use union find
	- only merge a root with another root that has been visited
- [[2022-08-30 Tuesday]] #Array #Math #Matrix 
  problem:: Rotate Image
  link:: https://leetcode.com/problems/rotate-image/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 630cad7c-5718-4a96-b84e-7f942c5cefe0
	- first transpose the matrix, then reverse each row
- [Unique Paths](((62e722bf-8106-4ceb-bf2f-b507baf2cc98))) can be solved using math, but remember to subtract one
- [Kth Smallest Element in a Sorted Matrix](((62e72331-3e40-44a5-b869-240732ebebeb))) need to be solved using binary search on the answer space
- [My Calendar I](((62e87482-0e2d-4287-b9c1-e88169dcd2f7))) can be solved by using ordered map and doing binary search on it
- [Combination Sum IV](((62ecc823-717d-4573-9983-4634c1695f7b))) is a simple DP problem, but need to remember how to handle overflow problem
- [Poor Pigs](((62eccebc-2a8e-45fc-bf83-7c5c1e490fbf))) is a tricky math problem
- [Count Vowels Permutation](((62edcc7b-9632-464b-896a-ff7eab4bb098))) is not hard at all after finding out the pattern
- [Longest Increasing Subsequence](((62ef1c0c-cf23-4086-896e-7c8ec3536c92))) can be solved using binary search to find the appropriate position to insert the number
- [Convert Sorted Array to Binary Search Tree](((62f26976-9cb5-4491-bbba-023fe8c56f97))) can be solved divide and conquer and recursion
- [Validate Binary Search Tree](((62f5474f-a6ef-415d-81ae-132f257fdea2))) can be solved by using in-order traversal
- [Lowest Common Ancestor of a Binary Search Tree](((62f599a6-ea14-47ee-9106-2138f3339b22))) can be solved using DFS, and comparing the targets with current node
- [Substring with Concatenation of All Words](((62f6012f-61f5-4e1a-a272-dcaa7fb19af4))) can be solved by using two hash tables, but sliding window method has better performance
- [Roman to Integer](((62f71515-26e7-47b3-b911-bf2a1f6886a0))) can be solved by iterating from the back and find every pair of symbols that their values are increasing
- [First Unique Character in a String](((62fa5468-1688-4210-89b7-f3ea44ee126b))) is an easy hash table problem
- [Unique Morse Code Words](((62fb9689-ef93-42df-83f9-e2c010a7f4d3))) is an easy hash table problem
- [Reduce Array Size to The Half](((62fcf06b-d288-44e2-834b-75edc7fef6d6))) is an easy hash table problem, and can be solved without using sorting
- [Split Array into Consecutive Subsequences](((62fe46fa-653a-4cb3-b45f-eb1edb6e580e))) is a greedy problem, but requires the information of how many strings ending with at a position with a certain length
- [Minimum Number of Refueling Stops](((62ff7779-8a61-4b27-b26c-16c95b5594e3))) can be solved by using DP, and the farthest position of stopping by a number of gas station should be the subproblem
- [Power of Four](((63004b49-9cc9-4dc0-8639-18cf701eafc3))) is an easy problem
- [Palindrome Linked List](((63039a20-176a-41f0-b78e-4a54eb761113))) can be solved by using two pointers to reverse the linked list, and remember to break the link to avoid infinite loop
- [Power of Three](((6304d1c7-f3e5-4345-a7db-d654e45c9e0a))) can be solved by using math
- [Ransom Note](((63076e14-e9d6-4d36-b9cd-4e8e6988ee47))) is an easy counting problem
- [Reordered Power of 2](((6307741e-6948-483d-b832-598d131b0535))) can be solved by using counting on the input and each power of 2
- [Sort the Matrix Diagonally](((63089ce4-a870-42c7-b790-0d98b2883c8e))) can be solved by sorting each diagonal, and we can achieve this by using hash table with priority queue
- [Number of Islands](((630acb8a-b385-4598-b954-712077c4fc7c))) can be solved by union find, and remember only merge a root with another visited root
- [Rotate Image](((630cad7c-5718-4a96-b84e-7f942c5cefe0))) can be solved by transposing then reversing the matrix