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
  - String
  - Sorting

#### Description :
Given an array of strings *strs*, group the **anagrams** together. You can return the answer in **any order**.

### Solution:
```
class Solution {
public:
    vector<vector<string>> groupAnagrams(vector<string>& strs) 
    {
        unordered_map <string, vector<string>> hash_map;
        for (const string& index : strs){
            string temp = index;
            sort(temp.begin(), temp.end());
            hash_map[temp].push_back(index);
        }
        vector <vector<string>> group;
        for (const auto& x : hash_map){
            group.push_back(x.second);
        }
        return group;
    }
};

```

