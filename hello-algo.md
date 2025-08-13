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
