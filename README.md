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

### [347. Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) <p align="right"><img src="https://img.shields.io/badge/Medium-%23f0bd07?style=plastic" width="60"></p>
- Topics : -
  - Array
  - Hash Table
  - Divide and Conquer
  - Sorting
  - Heap (Priority Queue)
  - Bucket Sort
  - Counting
  - Quick Select

#### Description :
Given an integer array *nums* and an integer *k*, return **the *k* most frequent elements**. You may return the answer in **any order**.

### Solution:
```
class Solution {
public:
    vector<int> topKFrequent(vector<int>& nums, int k) 
    {
        unordered_map<int, int> hash_map;

        for (int x : nums)
        {
            hash_map[x]++;
        }

        vector <int> solution;
        /*
        int max, element;
        vector <int> solution;
        while (k > 0)
        {
            max = 0;
            for (auto x : hash_map)
            {
                if (x.second > max)
                {
                    max = x.second;
                    element = x.first;
                }
            }
            hash_map[element] = -1;
            solution.push_back(element);
            k--;
        }*/

        priority_queue<pair<int, int>> pq;
        for (auto x : hash_map)
        {
            pq.push({x.second, x.first});
        }

        while (k > 0)
        {
            pair <int, int> temp = pq.top();
            solution.push_back(temp.second);
            pq.pop();
            k--;
        }
        
        return solution;
    }
};

```

