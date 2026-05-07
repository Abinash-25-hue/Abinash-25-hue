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
### [Two Sum](https://leetcode.com/problems/two-sum?envType=problem-list-v2&envId=array)
- Array
- Hash Table
<!--Given an array of integers <u>nums</u> and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.

### Solution:
```
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target)
    {
        unordered_map<int, int> hash_map;

        // Remove all the comments for the most optimal answer

        /*vector <int> v;
        v[0] = -1
        v[1] = -1*/
        for (int index = 0; index < nums.size(); index++)
        {
            if (hash_map.count(target - nums[index]))
            {
                //v[0] = index;
                //v[1] = hash_map[target - nums[index];]
                //return v;
                return {index, hash_map[target - nums[index]]};
            }
            hash_map.insert({nums[index], index});
        }

        //return v;
        return {};
    }
}

```

-->
