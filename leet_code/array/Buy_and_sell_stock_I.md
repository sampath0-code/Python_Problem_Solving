# 
<!-- Describe your first thoughts on how to solve this problem. -->

# 
<!-- Describe your approach to solving the problem. -->

# Complexity
- Time complexity: O(N)
<!-- Add your time complexity here, e.g. $$O(n)$$ -->

- Space complexity: O(1)
<!-- Add your space complexity here, e.g. $$O(n)$$ -->

# Code
```
class Solution(object):
    def maxProfit(self, prices):
        profit = 0
        min_price = prices[0]
        for i in range(len(prices)):
            min_price = min(prices[i],min_price)
            profit = max(profit,prices[i]- min_price)
        return profit
        
```
