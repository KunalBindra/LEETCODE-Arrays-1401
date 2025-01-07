# LEETCODE-Arrays-1401
**String Matching**

This Java class provides a solution to the "String Matching" problem.

**Problem Description:**

Given an array of strings `words`, return a list of strings that are substrings of another string in the array.

**Solution Approach:**

1. **Iterate through the array:** 
   - For each string `words[i]`, iterate through the remaining strings in the array.
2. **Check for substring:** 
   - If a string `words[j]` contains `words[i]` as a substring, add `words[i]` to the `result` list and break the inner loop.

**Time Complexity:**

- The time complexity of this solution is O(n^2 * m), where n is the number of strings in the array, and m is the average length of the strings.

**Space Complexity:**

- The space complexity is O(n) in the worst case, where n is the number of strings that are substrings of other strings in the array.

**Example Usage:**

```java
String[] words = {"mass","as","hero","superhero"};
Solution solution = new Solution();
List<String> result = solution.stringMatching(words); 
System.out.println(result); // Output: ["as", "hero"]
```
