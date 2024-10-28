- 8 easy, 11 medium, 0 hard
- 9 problems were solved for the first time
- [[2024-03-01 Friday]] #Math #String #Greedy 
  problem:: Maximum Odd Binary Number
  link:: https://leetcode.com/problems/maximum-odd-binary-number/description/?envType=daily-question&envId=2024-03-01
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 65e11f1b-cba4-4010-9aa9-2776ea65081c
	- sort the string in decreasing order then swap the last bit of 1
- [[2024-03-02 Saturday]] #Array #[[Two Pointers]] #Sorting 
  problem:: Squares of a Sorted Array
  link:: https://leetcode.com/problems/squares-of-a-sorted-array/description/?envType=daily-question&envId=2024-03-02
  difficulty:: Easy
  duration:: 2 mins
  number-of-times:: 1
  id:: 65e11f53-9b6e-4c76-aa29-e0ce8476e9b7
	- use two pointers to find the bigger absolute value
- [[2024-03-03 Sunday]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Remove Nth Node From End of List
  link:: https://leetcode.com/problems/remove-nth-node-from-end-of-list/description/?envType=daily-question&envId=2024-03-03
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 4
  id:: 65e27241-71b0-45a2-ad40-3a876c726f2e
	- use two pointers
	- move the fast pointer n times first, then move two pointers at the same time until fast pointer reach the end
	- remove the node next to slow pointer
- [[2024-03-04 Monday]] #Array #[[Two Pointers]] #Greedy #Sorting 
  problem:: Bag of Tokens
  link:: https://leetcode.com/problems/bag-of-tokens/description/?envType=daily-question&envId=2024-03-04
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 2
  id:: 65e3c944-b4c6-4162-bb4b-a5c53c7b2d16
	- sort the array and use two pointers
	- be aware of the constraints
- [[2024-03-06 Wednesday]] #[[Hash Table]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Linked List Cycle
  link:: https://leetcode.com/problems/linked-list-cycle/description/?envType=daily-question&envId=2024-03-06
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 4
  id:: 65e51678-93b6-4490-ad68-ebb0ac1075d2
	- use slow-fast pointers to detect the cycle
- [[2024-03-07 Thursday]] #[[Linked List]] #[[Two Pointers]] 
  problem:: Middle of the Linked List
  link:: https://leetcode.com/problems/middle-of-the-linked-list/description/?envType=daily-question&envId=2024-03-07
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 2
  id:: 65e7b4ce-59ed-4c3d-b8f9-340a04f9f325
	- easy two pointers problem
- [[2024-03-08 Friday]] #Array #[[Hash Table]] #Counting 
  problem:: Count Elements With Maximum Frequency
  link:: https://leetcode.com/problems/count-elements-with-maximum-frequency/description/?envType=daily-question&envId=2024-03-08
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 1
  id:: 65ea5a74-a090-43b1-adfe-e4b5647bdea8
	- sort the array then greedy search
	- can do it without sorting
- [[2024-03-09 Saturday]] #Array #[[Hash Table]] #[[Two Pointers]] #[[Binary Search]] 
  problem:: Minimum Common Value
  link:: https://leetcode.com/problems/minimum-common-value/description/?envType=daily-question&envId=2024-03-09
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 1
  id:: 65ea5aa0-916e-4234-b121-758a6d76a16f
	- use two pointers
- [[2024-03-10 Sunday]] #Array #[[Hash Table]] #[[Two Pointers]] #[[Binary Search]] #Sorting 
  problem:: Intersection of Two Arrays
  link:: https://leetcode.com/problems/intersection-of-two-arrays/description/?envType=daily-question&envId=2024-03-10
  difficulty:: Easy
  duration:: 3 mins
  number-of-times:: 3
  id:: d9bfd879-0c42-4202-9bd7-a2a127f6266f
	- sort the arrays first
	- find the duplicate numbers in both arrays using binary search
- [[2024-03-11 Monday]] #[[Hash Table]] #String #Sorting 
  problem:: Custom Sort String
  link:: https://leetcode.com/problems/custom-sort-string/description/?envType=daily-question&envId=2024-03-11
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 65ecff31-bf04-4e59-a970-324d774053c1
	- use a hash table to create a custom sorting function
	- be careful of comparing characters in and not in the order string
- [[2024-03-13 Wednesday]] #Math #[[Prefix Sum]] 
  problem:: Find the Pivot Integer
  link:: https://leetcode.com/problems/find-the-pivot-integer/description/?envType=daily-question&envId=2024-03-13
  difficulty:: Easy
  duration:: 2 mins
  number-of-times:: 1
  id:: 65ee5227-fd7d-44a6-a3c0-1742226d5a81
	- find the sum first
	- then use prefix sum to find the half of it
- [[2024-03-14 Thursday]] #Array #[[Hash Table]] #[[Sliding Window]] #[[Prefix Sum]] 
  problem:: Binary Subarrays With Sum
  link:: https://leetcode.com/problems/binary-subarrays-with-sum/description/?envType=daily-question&envId=2024-03-14
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 65f0f2c0-98a0-431c-aca0-ed661309e586
	- use prefix sum
- [[2024-03-15 Friday]] #Array #[[Prefix Sum]] 
  problem:: Product of Array Except Self
  link:: https://leetcode.com/problems/product-of-array-except-self/description/?envType=daily-question&envId=2024-03-15
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 5
  id:: 65f247b5-fe4e-4c59-a845-3fe7f071743d
	- compute two arrays containing the product from left and right
- [[2024-03-17 Sunday]] #Array 
  problem:: Insert Interval
  link:: https://leetcode.com/problems/insert-interval/description/?envType=daily-question&envId=2024-03-17
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 65f39610-34d4-49c0-94e0-4867aa3d19f1
	- insert the new interval
	- merge the overlapped intervals
- [[2024-03-18 Monday]] #Array #Greedy #Sorting 
  problem:: Minimum Number of Arrows to Burst Balloons
  link:: https://leetcode.com/problems/minimum-number-of-arrows-to-burst-balloons/description/?envType=daily-question&envId=2024-03-18
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 3
  id:: 65f63434-e11e-403d-94dc-091cc2893303
	- sort the balloons by their starting points
	- maintain the minimum endpoint for current balloons
- [[2024-03-20 Wednesday]] #[[Linked List]] 
  problem:: Merge In Between Linked Lists
  link:: https://leetcode.com/problems/merge-in-between-linked-lists/description/?envType=daily-question&envId=2024-03-20
  difficulty:: Medium
  duration:: 5 mins
  number-of-times:: 1
  id:: 65f78adc-59a8-42b0-8e5c-2d95f0a00940
	- traverse the first list and do the modification
- [[2024-03-21 Thursday]] #[[Linked List]] #Recursion 
  problem:: Reverse Linked List
  link:: https://leetcode.com/problems/reverse-linked-list/description/?envType=daily-question&envId=2024-03-21
  difficulty:: Easy
  duration:: 1 min
  number-of-times:: 4
  id:: 65fa2ff9-5deb-4b79-9114-dfe8d83fa92c
	- easy problem
- [[2024-03-24 Sunday]] #Array #[[Two Pointers]] #[[Binary Search]] #[[Bit Manipulation]] 
  problem:: Find the Duplicate Number
  link:: https://leetcode.com/problems/find-the-duplicate-number/description/?envType=daily-question&envId=2024-03-24
  difficulty:: Medium
  duration:: 3 mins
  number-of-times:: 5
  id:: 65fb83f1-7530-40b6-8510-dfe0771f4c54
	- use cycle detection
- [[2024-03-25 Monday]] #Array #[[Hash Table]] 
  problem:: Find All Duplicates in an Array
  link:: https://leetcode.com/problems/find-all-duplicates-in-an-array/description/?envType=daily-question&envId=2024-03-25
  difficulty:: Medium
  duration:: 2 mins
  number-of-times:: 4
  id:: 65ff7077-cc11-4052-9a9d-3e43598acd66
	- use negative numbers on a index to indicate the number of that index exists
- [[2024-03-27 Wednesday]] #Array #[[Sliding Window]] 
  problem:: Subarray Product Less Than K
  link:: https://leetcode.com/problems/subarray-product-less-than-k/description/?envType=daily-question&envId=2024-03-27
  difficulty:: Medium
  duration:: 10 mins
  number-of-times:: 1
  id:: 6600c258-8b83-4c1c-9d9a-b88e4753ff3a
	- use sliding window to calculate subarray product
-
- [Maximum Odd Binary Number](((65e11f1b-cba4-4010-9aa9-2776ea65081c))) is an easy greedy problem
- [Squares of a Sorted Array](((65e11f53-9b6e-4c76-aa29-e0ce8476e9b7))) is an easy two pointers problem
- [Remove Nth Node From End of List](((65e27241-71b0-45a2-ad40-3a876c726f2e))) can be solved by two pointers, and move the fast pointer n times first
- [Bag of Tokens](((65e3c944-b4c6-4162-bb4b-a5c53c7b2d16))) can be solved by sorting the array then using two pointers
- [Linked List Cycle](((65e51678-93b6-4490-ad68-ebb0ac1075d2))) can be solved by using two pointers
- [Middle of the Linked List](((65e7b4ce-59ed-4c3d-b8f9-340a04f9f325))) can be solved by using slow-fast pointers
- [Count Elements With Maximum Frequency](((65ea5a74-a090-43b1-adfe-e4b5647bdea8))) is an easy greedy problem
- [Minimum Common Value](((65ea5aa0-916e-4234-b121-758a6d76a16f))) is an easy two pointers problem
  id:: 65ebabd8-3195-4f5d-b1e9-aee5ca335a98
- [Intersection of Two Arrays](((d9bfd879-0c42-4202-9bd7-a2a127f6266f))) can be solved by sorting the arrays the using binary search
- [Custom Sort String](((65ecff31-bf04-4e59-a970-324d774053c1))) can be created by a custom sorting function
- [Find the Pivot Integer](((65ee5227-fd7d-44a6-a3c0-1742226d5a81))) is an easy prefix sum problem
- [Binary Subarrays With Sum](((65f0f2c0-98a0-431c-aca0-ed661309e586))) is an easy prefix sum problem, but it's much faster using two pointers
- [Product of Array Except Self](((65f247b5-fe4e-4c59-a845-3fe7f071743d))) can be solved by computing the products from left and right in advance
- [Insert Interval](((65f39610-34d4-49c0-94e0-4867aa3d19f1))) is an easy greedy problem
- [Minimum Number of Arrows to Burst Balloons](((65f63434-e11e-403d-94dc-091cc2893303))) can be solved by sorting the balloons by their starting points
- [Merge In Between Linked Lists](((65f78adc-59a8-42b0-8e5c-2d95f0a00940))) can be solved by simple list traversal
- [Reverse Linked List](((65fa2ff9-5deb-4b79-9114-dfe8d83fa92c))) is a very easy problem
- [Find the Duplicate Number](((65fb83f1-7530-40b6-8510-dfe0771f4c54))) can be solved by cycle detection, because duplicate numbers guarantee there's two numbers point to the same position
- [Find All Duplicates in an Array](((65ff7077-cc11-4052-9a9d-3e43598acd66))) is an easy problem
- [Subarray Product Less Than K](((6600c258-8b83-4c1c-9d9a-b88e4753ff3a))) can be solved by using sliding window