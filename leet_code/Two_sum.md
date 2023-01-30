# Simple solution|| Time Complexity O(N) || Space Complexity O(N)
<!-- Describe your first thoughts on how to solve this problem. -->

# Approach : 
* Create a empty dictionary 
* we know that sum of two numbers in the array would be equal to target, so let us assume that two numbers as x and y.
* we can say that x + y = target
   y = target - x
using this equation we can solve the problem...
<!-- Describe your approach to solving the problem. -->

# Complexity
- Time complexity: O(N)
<!-- Add your time complexity here, e.g. $$O(n)$$ -->

- Space complexity:O(N)
<!-- Add your space complexity here, e.g. $$O(n)$$ -->

# Code
```
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        dic = {}
        for i in range(len(nums)):
            y = target - nums[i]
            
            if y in dic:
                return dic[y],i
            dic[nums[i]]= i

        
```
