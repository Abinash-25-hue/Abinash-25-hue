<img width="1000" height="199" alt="Learning_never_stops_in_Computer_Science  (2)" src="https://github.com/user-attachments/assets/826f060b-3572-497e-99a7-ad3739af0125" />


# Hello World, I am Abinash Nayak.

💻 I'm currently learning **Java** and **Object Oriented Programming**.

---

## Languages

<a href="https://github.com/Abinash-25-hue/Optimization-Techniques--Operations-Research"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" width="55" /></a> &nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/cplusplus/cplusplus-original.svg" width="55"/>&nbsp;
<a href="https://github.com/Abinash-25-hue/CODSOFT"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original-wordmark.svg" width='62'/></a>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" width="63"/>
          
---
<h2 align="center"> 🏆 Completed 500 Contributions in last year ✅</h2>


---
## Daily Problem Solving
<!--My Last LeetCode Problem : -->

### [11. Container With Most Water](https://leetcode.com/problems/container-with-most-water) <p align="right"><img src="https://img.shields.io/badge/Medium-%23f0bd07?style=plastic" width="60"></p>
- Topics : -
  - Array
  - Two Pointers
  - Greedy
 
#### Description :
You are given an integer array **height** of length **n**. There are **n** vertical lines drawn such that the two endpoints are of the **i th** line are **{i, 0}** and **{i, height[i]}**.

Find two lines that together with the x-axis form a container, such that the container contains the most water.

Return *the maximum amount of water a container can store.*

**Notice** you may not slant the container.

<img width="801" height="383" alt="image" src="https://github.com/user-attachments/assets/c391850e-7e7b-4d9a-becb-a3c97f099d5a" />


### Solution:
```
class Solution {
public:
    int maxArea(vector<int>& height) {

        int water = 0;
        if (height.size() == 2)
        {
            if (height[0] < height[1])
            {
                water = height[0];
            }
            else
            {
                water = height[1];
            }
        }
        else
        {
            int left = 0, right = height.size() - 1, curr = 0;
            while (left < right)
            {
                if (height[left] < height[right])
                {
                    curr = height[left] * (right - left);
                    left++;
                }
                else
                {
                    curr = height[right] * (right - left);
                    right--;
                }

                if (curr > water)
                {
                    water = curr;
                }
            }
            
        }
        return water;
    }
};

```

