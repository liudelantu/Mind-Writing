集合用于存储多个不重复的元素，重复的元素会被自动去除。

```python
word = {'a', 'b', 'c', 'd'}            : 创建  
word = set(['a', 'b', 'b', 'c', 'd'])  : 创建 重复的b会被去除 {'a', 'b', 'c', 'd'} 
word.add('e')          : 添加
word.remove('a')       : 删除
word.discard('a')      : 删除
word = set_a | set_b   : 并集  或者使用 set_a.union(set_b)
word = set_a & set_b   : 交集  或者使用 set_a.intersection(set_b)
word = set_a - set_b   : 差集  或者使用 set_a.difference(set_b)
word = set_a ^ set_b   : 对称差集 或者使用 set_a.symmetric_difference(set_b)
word = frozenset([1, 2, 3, 4])  : 冻结集合, 之后不允许添加新元素

'a' in word    : 检查 集合是否有元素'a'

# 遍历集合
for c in word:
    print(c)

```

