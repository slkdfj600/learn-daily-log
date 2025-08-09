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
