# 栈
### 栈的常用操作
- `push()`  入栈  时间复杂度:O(1)  
- `pop()`   出栈  时间复杂度:O(1)
- `peek()`  访问栈顶元素  时间复杂度:(1)

---
```cpp
struct ListNode{
    int val;
    ListNode* next;
    ListNode(int v, ListNode* n = nullptr)
        : val(v), next(n) {}
};
```

- `struct`和`class`的区别是：`struct`默认成员是public,`class`默认成员是private
- `next`的类型是：指向`ListNode`的指针
- 最后的`ListNode()`是构造函数
- 形参`v`的值被用来初始化成员变量`val`
- 指针`n`默认为空值
- 冒号后面的`val(v), next(n)`叫成员初始化列表
- 创建对象的时候直接：
- `ListNode n1(10, &n1);`
- 则，`val = 10, next = &n1`

---

析构函数在对象生命周期结束后被自动调用  

---

- `.h`(头文件)里放一些，类的定义，结构体的定义，函数的声明等等
- 它告诉你
- `.cpp`(源文件)里放一些，类成员函数的具体实现，非类函数的具体实现，全局变量的定义和初始化
- 类成员函数需要对象来调用
- 非类成员函数可以直接调用

---

`pragma once`的作用是防止头文件被重复包含  


