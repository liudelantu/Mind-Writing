```python
word = ['a', 'b', 'c', 'd', 'f']  : 创建
word[0]                   : 访问
word.append('g')          : 追加1个元素
word.extend(['h', 'i'])   : 追加多个元素
word.insert(0, 'z')       : 指定位置 插入元素
word.remove('a')          : 删除 第一个匹配的元素
word.pop()                : 删除 最后一个元素
del word[0]               : 删除 指定位置的元素
word.sort()               : 排序 字母在前，数字在后
word.reverse()            : 反转列表
new_list = word.copy()    : 拷贝列表
combined_list = list1 + list2   : 连接2个列表
repeated_list = list1 * 2       : 重复1次列表

# 遍历列表
for c in word:
    print(c)

```

