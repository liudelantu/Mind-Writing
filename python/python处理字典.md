```python
word = {'name': 'Alice', 'age': 30, 'city': 'New York'}  : 创建
word['name']      : 访问
word.get('name')  : 访问
word['age'] = 31  : 更新
del word['city']  : 删除
len(word)         : 键的个数
cmp(dict1, dict2) : 比较两个字典
word.clear()      : 清空字典
word.items()      : 以列表形式返回可遍历的(key, value)元组类型数组
word.keys()       : 所有的 key
word.values()     : 所有的 value
word.has_key(key) : 如果键 key 在字典中则返回 True
key in word       : 如果键 key 在字典中则返回 True


# 遍历字典
for key in word:
    print(key) 
    
for value in word.values():
    print(value) 
    
for key, value in word.items():
    print(f"{key}: {value}") 
```



