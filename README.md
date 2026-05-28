# Hello World, I am Abinash Nayak.

💻 I'm currently learning **Java** and **Object Oriented Programming**.

---

## Languages

<a href="https://github.com/Abinash-25-hue/Optimization-Techniques--Operations-Research"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" width="55" /></a> &nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/cplusplus/cplusplus-original.svg" width="55"/>&nbsp;
<a href="https://github.com/Abinash-25-hue/CODSOFT"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original-wordmark.svg" width='62'/></a>

---
## Daily Problem Solving
<!--My Last LeetCode Problem : -->

### [Contains Duplicate](https://leetcode.com/problems/contains-duplicate) <p align="right"><img src="https://img.shields.io/badge/Easy-green?style=plastic" width="40"></p>
- Topics : -
  - Array
  - Hash Table
  - Sorting

#### Description :
Given an integer array *nums*, return *true* if any value appears at least twice in the array, and return *false* if every element is distinct.

### Solution:
```
class Solution {
public:
    bool containsDuplicate(vector<int>& nums) {
        sort(nums.begin(), nums.end());
        for (int i = 0; i < nums.size() - 1; i++)
        {
            if (nums[i] == nums[i + 1])
            {
                return true;
            }
        }
        return false;
    }
};

```

