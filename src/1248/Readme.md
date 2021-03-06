## LeetCode 1248: Count Number of Nice Subarrays

### Problem

[Problem link](https://leetcode-cn.com/problems/count-number-of-nice-subarrays/)

### Solution description

Update serval pointers at the same time to traverse the list.

If there is the surplus array of even number before and after "odd region(a minimal arrays of k odd numbers region)", then due to the law of multiplication, the number of nice subarrays expanded by this core "odd region" is: `#left surplus of even number + 1` * `right surplus of even number + 1`.

[Official implementation](https://leetcode-cn.com/problems/count-number-of-nice-subarrays/solution/tong-ji-you-mei-zi-shu-zu-by-leetcode-solution/) points out that even number is redundant to decide so-called core "odd region", therefore, it creates an array to record each odd number and its indices, which could also infer the length of the aforementioned surplus.

### File structure

 - `sol.cpp`: solution

### Performance

| Solution             | Link         | Runtime | Memory Usage |
| ------------------------ | ------- | ------------ | ------------ |
| simulate | [sol.cpp](sol.cpp) | 292ms | 62.8MB |
|          |      |         |              |

