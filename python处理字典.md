```python
# 操作字典
my_dict = {'name': 'Alice', 'age': 30, 'city': 'New York'}  : 创建
my_dict['name']      : 访问
my_dict.get('name')  : 访问
my_dict['age'] = 31  : 更新
del my_dict['city']  : 删除
len(my_dict)         : 键的个数
cmp(dict1, dict2)    : 比较两个字典
my_dict.clear()      : 清空字典
my_dict.items()      : 以列表形式返回可遍历的(key, value)元组类型数组
my_dict.keys()       : 以列表形式返回字典中所有的 key
my_dict.values()     : 以列表形式返回字典中所有的 value
my_dict.has_key(key) : 如果键 key 在字典中则返回 True
key in my_dict       : 如果键 key 在字典中则返回 True
my_dict.popitem()    : 随即返回并删除一个键值对，并以(key, value)元组方式返回


# 遍历字典
for key in my_dict:
    print(key)  # 输出: name, country
    
for value in my_dict.values():
    print(value)  # 输出: Alice, USA
    
for key, value in my_dict.items():
    print(f"{key}: {value}")  # 输出: name: Alice, country: USA
```



