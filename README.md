<img width="1000" height="199" alt="Learning_never_stops_in_Computer_Science  (2)" src="https://github.com/user-attachments/assets/826f060b-3572-497e-99a7-ad3739af0125" />


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

### [Group Anagrams](https://leetcode.com/problems/group-anagrams) <p align="right"><img src="https://img.shields.io/badge/Easy-green?style=plastic" width="40"></p>
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

