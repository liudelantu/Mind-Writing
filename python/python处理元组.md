元组是 Python 中的一种不可变的序列类型，适合用于存储固定的值。

```python
word = ('x', 'y', 'x')    : 创建          # 注意：单个元素元组需要逗号 例如 (1,) 
word[0]                   : 访问
word[1:3]                 : 获取索引为1，2的值 y z
word.count('y')           : 返回元素的出现次数
word.index('y')           : 返回元素的索引
combined_tuple = tuple1 + tuple2  : 连接元组
repeated_tuple = tuple1 * 2       : 重复1次元组
x, y, z = (1, 2, 3)       : 解包元组  x=1  y=2  z=3


# 遍历元组
for c in word:
    print(c)  # 输出: 1, 2, 3

    
元组的使用场景：
1. 避免数据修改
2. 作为字典的键，非常适合用于存储复合键   {(1, 2): 'A', (3, 4): 'B'}
3. 数据库 表中的一行记录的各个字段   ("Alice", 30, "New York")
4. 作为函数参数，元组的解包功能
5. 存储多种数据类型
```

