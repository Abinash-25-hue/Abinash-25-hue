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



### Solution:
```
class Solution {
public:
    bool isAnagram(string s, string t) {
        unordered_map <char, int> hash_map;
        if (s.size() != t.size())
        {
            return false;
        }
        for (int index = 0; index < s.size(); index++)
        {
            hash_map[(s[index])]++;
            hash_map[(t[index])]--;
        }

        for (auto x : hash_map)
        {
            if (x.second != 0)
            {
                return false;
            }
        }
        return true;
    }
};

```

