@[TOC](leetcode刷题总结)
# 双指针

## 数组双指针
[两数之和 II - 输入有序数组
https://leetcode-cn.com/problems/two-sum-ii-input-array-is-sorted/
](https://leetcode-cn.com/problems/two-sum-ii-input-array-is-sorted/)分析： 数组已经有序了，那其实可以用二分的思路: if 首尾之和大于target; j--; else i++;

## 字符串双指针
[反转单个单词 
https://leetcode-cn.com/problems/reverse-string/](https://leetcode-cn.com/problems/reverse-string/)
  分析：简单题，利用反转字符的**i = n - i - 1**这个关系式，其次就是指针i移动到数组一半的位置即反转完毕
  
  [反转字符串中的每个单词 
  https://leetcode-cn.com/problems/reverse-words-in-a-string-iii/](https://leetcode-cn.com/problems/reverse-words-in-a-string-iii/)
分析：利用1的解题思路，**添加while循环即可，找出空格字符的位置**

## 链表双指针
[链表的中间结点
https://leetcode-cn.com/problems/middle-of-the-linked-list/](https://leetcode-cn.com/problems/middle-of-the-linked-list/)
使用**快慢指针**，快指针走两步，慢指针走一步，快指针走到链表末尾，则慢指针走到链表的一半。

[删除链表的倒数第N个结点
https://leetcode-cn.com/problems/remove-nth-node-from-end-of-list/](https://leetcode-cn.com/problems/remove-nth-node-from-end-of-list/)
**快慢指针**：让快指针fast=head先走n步，再定义slow = (0, head)
则当快指针走到头，慢指针的next结点即为要删除的倒n结点

**计算链表长度**：定义p指针计数链表的长度，q指针用来删除倒n的结点
最后返回dumNode.next

**栈**【先进后出】，弹出栈的第n个结点


