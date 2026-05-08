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
Given an array of integers *nums* and an integer *target*, return indices of the two numbers such that they add up to *target*.
You may assume that each input would have exactly one solution, and you may not use the same element twice.


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

