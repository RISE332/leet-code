@[TOC](leetcode刷题思路总结)
# leet-code
总结记录leetcode的心得

## 双指针

### 数组双指针
- 两数之和 II - 输入有序数组 https://leetcode-cn.com/problems/two-sum-ii-input-array-is-sorted/
  - 分析： 数组已经有序了，那其实可以用二分的思路: if 首尾之和大于target; j--; else i++;

### 字符串双指针
- 反转单个单词 https://leetcode-cn.com/problems/reverse-string/
  - 分析：简答题，利用反转字符的 i = n - i - 1 这个关系式，其次就是指针i移动到数组一半的位置即反转完毕
- 反转字符串中的每个单词 https://leetcode-cn.com/problems/reverse-words-in-a-string-iii/
  - 分析：利用1的解题思路，添加while循环即可，找出空格字符的位置

### 链表双指针
- 寻找链表的中点
- 
