>`a = [1, 2, 3]` 这里的a是一个列表
---
>python中，单引号''和双引号""，没区别
---
>全小写：lower()  
>全大写：upper()  
>每个单词首字母大写：title()
---
>s.lstrip([chars]):从左侧开始删，直到遇到第一个不在chars集合的字符为止  
>s.rstrip([chars]):从右侧开始删，直到遇到第一个不在chars集合的字符为止  
>s.strip([chars]):左右都删  
>不传chars时，默认删除“空白字符”：空格，制表符，换行符，回车...
---
>`removesuffix()`是一个字符串方法  
>`filename.removesuffix('.txt')`会检查`filename`字符串的末尾是否是`.txt`  
>如果是就删除，并返回不带后缀的字符串  
>如果不是就直接返回字符串  
>`removesuffix('.txt')`是把`'.txt'`当作一个完整的，固定的字符串来匹配  
>`rstrip('.txt')`：把`'.xt'`当作一个字符集合`{'.', 't', 'x'}来处理

 ---

 ```python
from typing import List

class Solution:
    def search(self, nums: List[int], target: int) -> int:
#在定义函数时使用了类型提示
#nums要是元素为int类型的列表
#target的类型也为int
#返回值为int
        l, r = 0, len(nums) -1 

        while l <= r:
            mid = (l + r) // 2
            if nums[mid] < target:
                l = mid + 1
            elif nums[mid] > target:
                r = mid - 1
            else:
                return mid
        
        return -1
            
if __name__ == "__main__":
    sol = Solution()
    
    array1 = [-1, 0 ,3, 5, 9, 12]
    
    t1 = 9
    t2 = 2
    
    result1 = sol.search(array1, t1)
    result2 = sol.search(array1, t2)
    
    print(result1)
    print(result2)
```
