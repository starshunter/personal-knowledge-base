- 8 easy, 10 medium, 0 hard
- 8 problems were solved for the first time
- [[2022-11-01 Tuesday]] #Array #DP #DFS #Matrix #Simulation 
  problem:: Where Will the Ball Fall
  link:: https://leetcode.com/problems/where-will-the-ball-fall/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 63606fed-d268-46b8-9939-f66f8c493a0c
	- do simulation row by row to change the ball's position
	- can be solved by simulating dropping each ball from each column
- [[2022-11-02 Wednesday]] #[[Hash Table]] #String #BFS 
  problem:: Minimum Genetic Mutation
  link:: https://leetcode.com/problems/minimum-genetic-mutation/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 2
  id:: 63607051-ab8c-4604-8685-261c51d0d36b
	- use BFS and a hash table
	- use hash table to store the minimum steps to reach to that mutation
	- compare current mutation to every other unreached mutation
- [[2022-11-04 Friday]] #[[Two Pointers]] #String 
  problem:: Reverse Vowels of a String
  link:: https://leetcode.com/problems/reverse-vowels-of-a-string/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 3
  id:: 6361c055-3a32-4760-97a0-cb43fd77524c
	- use two pointers
	- remember to check index out of bounds
- [[2022-11-07 Monday]] #Math #Greedy 
  problem:: Maximum 69 Number
  link:: https://leetcode.com/problems/maximum-69-number/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 6364f2d6-4480-4251-a9ca-c2b8e5bf8db3
	- easy, find the first digit that is six
- [[2022-11-08 Tuesday]] #String #Stack 
  problem:: Make The String Great
  link:: https://leetcode.com/problems/make-the-string-great/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 6368551d-854b-40d1-881a-8803d017d6d5
	- iterate through the string, check backward first, then check frontword
	- can use two pointers and do it in place
- [[2022-11-09 Wednesday]] #Stack #Design #[[Monotonic Stack]] #[[Data Stream]] 
  problem:: Online Stock Span
  link:: https://leetcode.com/problems/online-stock-span/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 1
  id:: 6369a78b-446d-4f5f-9d2e-7dfc2e9c0208
	- maintain a decreasing monotonic stack
- [[2022-11-10 Thursday]] #String #Stack 
  problem:: Remove All Adjacent Duplicates In String
  link:: https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string/description/
  difficulty:: Easy
  duration:: 5 mins
  number_of_times:: 1
  id:: 636afbe0-c056-4c29-a0f5-9fb8c90593ca
	- construct a new string
	- we can only remove two characters at once
	- can be solved by using two pointers
- [[2022-11-11 Friday]] #Array #[[Two Pointers]] 
  problem:: Remove Duplicates from Sorted Array
  link:: https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 3
  id:: 636d9892-2241-4464-8250-4e9c60f9ee38
	- use two pointers
- [[2022-11-13 Sunday]] #[[Two Pointers]] #String 
  problem:: Reverse Words in a String
  link:: https://leetcode.com/problems/reverse-words-in-a-string/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 2
  id:: 636d9bea-4fac-4b9b-8354-6c785a916b83
	- first reverse the entire string
	- then use two pointers to reverse each word, and cleanup white space as well
	- we can clean up the white space after reversing each rowd
- [[2022-11-16 Wednesday]] #[[Binary Search]] #Interactive 
  problem:: Guess Number Higher or Lower
  link:: https://leetcode.com/problems/guess-number-higher-or-lower/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 4
  id:: 63706658-8f4b-4340-84fb-1afe2a756f95
	- binary search on the answer space
- [[2022-11-17 Thursday]] #Math #Geometry 
  problem:: Rectangle Area
  link:: https://leetcode.com/problems/rectangle-area/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 63743273-d770-4a44-921d-15c09360a0e4
	- calculate the sum of the two areas
	- check if two rectangles overlap
	- calculate the overlap area
- [[2022-11-18 Friday]] #Math 
  problem:: Ugly Number
  link:: https://leetcode.com/problems/ugly-number/description/
  difficulty:: Easy
  duration:: 1 min
  number_of_times:: 3
  id:: 637583c0-aa4a-421d-ae1f-2121447c0228
	- divide the number by 2, 3, 5 until it can't, then check the equality with 1
- [[2022-11-21 Monday]] #Array #BFS #Matrix 
  problem:: Nearest Exit from Entrance in Maze
  link:: https://leetcode.com/problems/nearest-exit-from-entrance-in-maze/description/
  difficulty:: Medium
  duration:: 30 mins
  number_of_times:: 1
  id:: 637b68b5-afd7-444d-aff2-58ea8de99898
	- use BFS
	- use hash table to record visited places
- [[2022-11-22 Tuesday]] #Math #DP #BFS 
  problem:: Perfect Squares
  link:: https://leetcode.com/problems/perfect-squares/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 3
  id:: 637b6b20-e853-4217-aa35-61c6a1994ee3
	- use DP
	- calculate the least number of perfect square numbers from `1` to `n`
- [[2022-11-24 Thursday]] #Array #Backtracking #Matrix 
  problem:: Word Search
  link:: https://leetcode.com/problems/word-search/description/
  difficulty:: Medium
  duration:: 15 mins
  number_of_times:: 4
  id:: 637c1c04-2eec-4b78-a695-6dcbb2cd95cc
	- do DFS from every position
	- use a 2D vector to record visited positions
- [[2022-11-28 Monday]] #Array #[[Hash Table]] #Sorting #Counting 
  problem:: Find Players With Zero or One Losses
  link:: https://leetcode.com/problems/find-players-with-zero-or-one-losses/description/
  difficulty:: Medium
  duration:: 5 mins
  number_of_times:: 1
  id:: 637ec249-6c13-4bb0-ad99-dca75a3a1117
	- use a hash table to track the number of losses
- [[2022-11-29 Tuesday]] #Array #[[Hash Table]] #Math #Design #Randomized 
  problem:: Insert Delete GetRandom O(1)
  link:: https://leetcode.com/problems/insert-delete-getrandom-o1/description/
  difficulty:: Medium
  duration:: 10 mins
  number_of_times:: 3
  id:: 6384a398-d687-4bba-965e-85c9dce27e94
	- use a hash table to record each number's position in the array
	- move the number to the back of the array before removing it
	- use the length of the array to choose a random number
- [[2022-11-30 Wednesday]] #Array #[[Hash Table]] 
  problem:: Unique Number of Occurrences
  link:: https://leetcode.com/problems/unique-number-of-occurrences/description/
  difficulty:: Easy
  duration:: 2 mins
  number_of_times:: 1
  id:: 6385f3b8-5143-435a-9e0e-289f41483305
	- use two hash tables, one to record the occurrence of each number, another to record the unique occurrence
	- can be solved by counting sort
- [Where Will the Ball Fall](((63606fed-d268-46b8-9939-f66f8c493a0c))) can be solved by doing simulation
- [Minimum Genetic Mutation](((63607051-ab8c-4604-8685-261c51d0d36b))) can be solved by using BFS and a hash table
- [Reverse Vowels of a String](((6361c055-3a32-4760-97a0-cb43fd77524c))) is an easy two pointers problem
- [Maximum 69 Number](((6364f2d6-4480-4251-a9ca-c2b8e5bf8db3))) is an easy problem
- [Make The String Great](((6368551d-854b-40d1-881a-8803d017d6d5))) can be solved by just iterating through the string, but it can also be solved in place using two pointers
- [Online Stock Span](((6369a78b-446d-4f5f-9d2e-7dfc2e9c0208))) can be solved by using a decreasing monotonic stack
- [Remove All Adjacent Duplicates In String](((636afbe0-c056-4c29-a0f5-9fb8c90593ca))) is an easy two pointers problem
- [Remove Duplicates from Sorted Array](((636d9892-2241-4464-8250-4e9c60f9ee38))) is an easy two pointers problem
- [Reverse Words in a String](((636d9bea-4fac-4b9b-8354-6c785a916b83))) can be solved by using two pointers
- [Guess Number Higher or Lower](((63706658-8f4b-4340-84fb-1afe2a756f95))) is an easy binary search problem
- [Rectangle Area](((63743273-d770-4a44-921d-15c09360a0e4))) can be solved by checking and calculating the overlap area
- [Ugly Number](((637583c0-aa4a-421d-ae1f-2121447c0228))) is an easy math problem
- [Nearest Exit from Entrance in Maze](((637b68b5-afd7-444d-aff2-58ea8de99898))) is a basic BFS problem
- [Perfect Squares](((637b6b20-e853-4217-aa35-61c6a1994ee3))) can be solved by DP, we can calculate the answer from 1 to n
- [Word Search](((637c1c04-2eec-4b78-a695-6dcbb2cd95cc))) is a basic DFS problem
- [Find Players With Zero or One Losses](((637ec249-6c13-4bb0-ad99-dca75a3a1117))) is an easy hash table problem
- [Insert Delete GetRandom O(1)](((6384a398-d687-4bba-965e-85c9dce27e94))) can be solved by using a hash table to record the position of a number
- [Unique Number of Occurrences](((6385f3b8-5143-435a-9e0e-289f41483305))) can be solved by using two hash tables or counting sort