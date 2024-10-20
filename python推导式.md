# 1. 列表推导式

**原始代码**：

```python
squares = [x**2 for x in range(10)]
# 结果: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

**改写**：

```python
squares = []
for x in range(10):
    squares.append(x**2)
```

# 2. 字典推导式

**原始代码**：

```python
squared_dict = {x: x**2 for x in range(5)}
# 结果: {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
```

**改写**：

```python
squared_dict = {}
for x in range(5):
    squared_dict[x] = x**2
```

# 3. 集合推导式

**原始代码**：

```python
unique_squares = {x**2 for x in range(-5, 6)}   # range(-5, 6) --->  -5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5
# 结果: {0, 1, 4, 9, 16, 25}
# {}括号存键值对，它就是字典，{}括号存唯一值，它就是集合     集合会自动去掉重复的值
```

**改写**：

```python
unique_squares = set()
for x in range(-5, 6):
    unique_squares.add(x**2)
```

# 4. 生成器表达式

**原始代码**：

```python
gen = (x**2 for x in range(10))
```

**改写**：

```python
def generate_squares():
    for x in range(10):
        yield x**2

gen = generate_squares()
```

# 5. 条件表达式

**原始代码**：

```python
even_squares = [x**2 for x in range(10) if x % 2 == 0]
# 结果: [0, 4, 16, 36, 64]
```

**改写**：

```python
even_squares = []
for x in range(10):
    if x % 2 == 0:
        even_squares.append(x**2)
```

# 6. 多重推导式

**原始代码**：

```python
pairs = [(x, y) for x in range(3) for y in range(3)]
# 结果: [(0, 0), (0, 1), (0, 2), (1, 0), (1, 1), (1, 2), (2, 0), (2, 1), (2, 2)]
```

**改写**：

```python
pairs = []
for x in range(3):
    for y in range(3):
        pairs.append((x, y))
```

# 7. 使用 `filter()` 和 `map()`

**使用 `filter()`**：

**原始代码**：

```python
evens = list(filter(lambda x: x % 2 == 0, range(10)))
# 结果: [0, 2, 4, 6, 8]
```

**改写**：

```python
evens = []
for x in range(10):
    if x % 2 == 0:
        evens.append(x)
```

**使用 `map()`**：

**原始代码**：

```python
squared = list(map(lambda x: x**2, range(10)))
# 结果: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

**改写**：

```python
squared = []
for x in range(10):
    squared.append(x**2)
```