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
### [Contains Duplicate](https://leetcode.com/problems/contains-duplicate)
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
        // int s = nums.size();
        // for (int i = 0; i < s - 1; i++){
        //     for (int j = i + 1; j < s; j++){
        //         if (nums[i] == nums[j]){
        //             return true;
        //         }
        //     }    
        // }
        // return false;
        // set<int> s;
        // for (int i : nums)
        // {
        //     if (s.find(i) != s.end())
        //     {
        //         return true;
        //     }
        //     else
        //     {
        //         s.insert(i);
        //     }
        // }
        // return false;

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

