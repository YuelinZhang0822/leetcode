# Leetcode
Just want to push myself to practice coding

| # | Title | Solution | Basic idea (One line) |
|---| ----- | -------- | --------------------- |
| | **n sum** | | |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum/) | [Java](./src/twoSum.java) | 1. HashMap O(n) and O(n) space.<br>2. Sort with two points O(nlogn) and O(1) space. |
| 167 | [Two Sum II - Input Array is sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/) | [Java](./src/twoSumSorted.java) | 1. two pointers O(n) 2. binary search O(log(n!)) |
| 170 | [Two Sum III - Data Structure Design](https://leetcode.com/problems/two-sum-iii-data-structure-design/) | [Java](./src/twoSumDataStructure.java) | Use HashMap to store numbers. Maintain a list with distinct elements. |
| 653 | [Two Sum IV - Input is a BST](https://leetcode.com/problems/two-sum-iv-input-is-a-bst/) | [Java](./src/twoSumIV.java) | 1. DFS + HashSet Time: O(n), Space: O(n).<br>2. Inorder traversal + two pointers Time: O(n), Space: O(n) <br>3. BST iterator + stack Time: O(n), Space: O(logn) |
| 15 | [3 sum](https://leetcode.com/problems/3sum/) | [Java](./src/threeSum.java) | for loop + two sum(pay attention to duplicates) Time: O(n^2)|
| | **sliding window algorithm** | | |
| 3 | [Longest Substring without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) |[Java](./src/longestSubstringWithoutRepeatingCharacters.java) | two pointers, sliding window algorithm |
| 76 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/) | [Java](./src/minWindowSubstring.java) | two pointers, sliding window algorithm |
| 159 | [Longest Substring with At Most Two Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-two-distinct-characters/) | [Java](./src/longestSubstringTwoDistinct.java) | two pointers, sliding window algorithm |
| 340 | [Longest Substring with At Most k Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters/) | [Java](./src/longestSubstringKDisctince.java) | two pointers, sliding window algorighm | 
| 438 | [Find All Anagrams in a String](https://leetcode.com/problems/find-all-anagrams-in-a-string/) | [Java](./src/anagramsInString.java) | 1. sliding window 固定窗口，比较两格hashmap -> 比较两个array -> 维护一个array <br> 2. two pointers + sliding window 活动窗口 |
| 567 | [Permutation in String](https://leetcode.com/problems/permutation-in-string/) | [Java](./src/permutationInString.java) | sliding window 固定窗口，比较两格hashmap -> 比较两个array -> 维护一个array|
| | **binary search** | | |
| 278 | [First Bad Version](https://leetcode.com/problems/first-bad-version/) | [Java](./src/firstBadVersion.java) | Binary Search Time: O(logN) Space: O(1)|
| 35 | [Search Insert Position](https://leetcode.com/problems/search-insert-position/) | [Java](./src/searchInsertPosition.java) | Binary Search, 注意边界条件 |
| 852 | [Peak Index in a Mountain Array](https://leetcode.com/problems/peak-index-in-a-mountain-array/) | [Java](./src/peakIndex.java) | 1. Binary Search iterative Time: O(logN) Space: O(1) <br> 2. Binary Search recursive Time: O(logN) Space: O(logN) <br> 3. for loop .. |
| 162 | [Find Peak Element](https://leetcode.com/problems/find-peak-element/) | [Java](./src/peakElement.java) | same as 852 山峰数组，关键找出判断二分的条件 |
| 153 | [Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/) | [Java](./src/findMinInRotatedSortedArray.java) |Binary Search 跟nums[right]比较|
| 154 | [Find Minimum in Rotated Sorted Array II](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array-ii/) | [Java](./src/findMinInRotatedSortedArrayII.java) | 包含duplicates,还是Binary Search 当nums[mid]和nums[right]相等时，right--。但是时间复杂度变O(n), worst case: 11101111 |
| 33 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/) | [Java](./src/searchInRotatedSortedArray.java) | 两次二分法，先找出rotate的点，再在一边进行normal binary search |
| 74 | [Search a 2D metrix](https://leetcode.com/problems/search-a-2d-matrix/) | [Java](./src/search2DMetrix.java) | 把2Dmetric看成一个sorted array，还是binary search Time: O(log(m*n)) = O(log(m)+log(n)) |
| 240 | [Search a 2D metrix II](https://leetcode.com/problems/search-a-2d-matrix-ii/) | [Java](./src/search2DMetrixII.java) |1. binary search tree model. Time: O(m+n) <br> 2. binary search Time:O(m*log(n)) |
| | **back tracking** | | |
| 78 | [Subsets](https://leetcode.com/problems/subsets/) | [Java](./src/subsets.java) | back tracking 两种方法构造recursion tree 剪枝的那个TREE更容易处理remove duplicates的问题|
| 90 | [SubsetsII](https://leetcode.com/problems/subsets-ii/) | [Java](./src/subsetsII.java) | 有duplicates应该怎样处理(对于每个node，剪掉相同的branches) |
| 77 | [Combinations](https://leetcode.com/problems/combinations/) | [Java](./src/combinations.java) |自己稍微改动一下，练习了一下应对duplicates的情况。Time: O(C(n,k)/C(K)) ~ O(n!) |
| 39 | [Combination Sum](https://leetcode.com/problems/combination-sum/) | [Java](./src/combinationSum.java) | 1. 引入index来确定有多少branches <br> 2。去重问题 T:exponential|
| 40 | [Combination Sum II](https://leetcode.com/problems/combination-sum-ii/) | [Java](./src/combinationSummII.java) | 相同的recursion tree,不同的限制条件|
| 216 | [Combination Sum III](https://leetcode.com/problems/combination-sum-iii/description/) | [Java](./scr/combinationSummIII.java) | 相同的recursion tree,不同的限制条件 |
| 46 | [Permutations](https://leetcode.com/problems/permutations/) |[Java](./src/permutations.java) |1. remove/add elements from arraylist <br> 2. use a boolean array |
| 47 | [PermutationsII](https://leetcode.com/problems/permutations-ii/)|[Java](./src/permutationsII.java)|For each node, remove duplicate branches|
| 20 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses/) |[Java](./src/validParentheses.java)| valid parentheses: 每当我们放一个右括号的时候，已经放的左括号要比右括号的数量多|
| 22 | [Generate Parentheses](https://leetcode.com/problems/generate-parentheses/) |[Java](./src/generateParentheses.java) | backtracking的经典题目，对于每一个position（Node）,有两个branches：（ 或 ）|
| 401 | [Binary Watch](https://leetcode.com/problems/binary-watch/) |[Java](./src/binaryWatch.java) |把num分成两个数num1，num2。分别对hours和minutes求combination sum。<br> 9.5 notes: 这几天系统刷backtracking的题。发现这道题的子问题其实就是combination sum |
| 17 | [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number/) |[Java](./src/letterCombinations.java) | |
| 79 | [Word Search](https://leetcode.com/problems/word-search/) | [Java](./src/wordSearch.java) |Time complexity: time O(mn*4^k) where k is the length of the string|


