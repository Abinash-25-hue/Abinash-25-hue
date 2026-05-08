# Hello World, I am Abinash Nayak.

💻 I'm currently learning **Java** and **Object Oriented Programming**.

---

## Languages

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" width="55" /> &nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/cplusplus/cplusplus-original.svg" width="55"/>&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original-wordmark.svg" width='62'/>

---
## Daily Problem Solving
<!--My Last LeetCode Problem : -->
### [Valid Anagram](https://leetcode.com/problems/valid-anagram)
- Topics : -
  - Array
  - Hash Table

#### Description :
Given two strings *s* and *t*, return true if *t* is an anagram of *s*, and false otherwise.


### Solution:
```
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target)
    {
        unordered_map<int, int> hash_map;

        for (int index = 0; index < nums.size(); index++)
        {
            if (hash_map.count(target - nums[index]))
            {
                return {index, hash_map[target - nums[index]]};
            }
            hash_map.insert({nums[index], index});
        }
        return {};
    }
}

```

