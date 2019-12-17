# python基本数据结构

## 布尔值

True False

### 以下值都为False

* False
* None
* 0
* ""
* ()
* []
* {}

## 数字

### int整数

```python
x = int(3)
x = int('010', 8)
x = 3
```

### float浮点数

```python
x = 3.1
x = float(3.1)
```

### complex复数

a = complex('1+2j')加号两边不能有空格，a.real取实部，a.imag取虚部

## 字符串String

### 单引号字符串以及对引号转义

```python
"Let's go!"
'Let\'s go!'
```

### 字符串拼接

使用 +

### 字符串str和repr

换行符 \n

### 常字符串，原始字符串和字节

长字符串(跨越多行的字符串)使用三引号 ''' '''

### 字符串方法

* find 在字符串中查找子串，返回第一个字的索引，或者-1
* join 合并序列
* lower 返回字符串的小写版本
* title 所有单词首字母大写，或者使用string模块的capwords()
* replace 将指定字符串替换为另一个字符串
* split 将字符串分割成序列
* strip 删除字符串开头和末尾的空白
* translate 单字符替换，同时替换多个字符，效率比raplace高
* is开头，判断字符串是否满足特定条件，返回True False

## 列表List

有序，可更改。最常用的数据类型

```python
list = ['qhj', 786, 22.3, 'john', 88]
tinylist = [22.3, 123, 'john']

print(list)
print(list[0])
print(list[1:3])
print(list[2:])
print(tinylist*2) # *重复操作
print(list + tinylist) # +连接
```

### 方法

```python
len(list)
max(list)
min(list)
```

list.append()

list.extend

## 元组Tuple

援助内部元素用逗号分割，不能二次赋值，只读。

```python
tuple = ('qhj', 786, 22.3, 'john', 88)
tinytuple = (22.3, 123, 'john')

print(tuple)
print(tuple[0])
print(tuple[1:3])
print(tuple[2:])
print(tuple * 2)
print(tuple + tinytuple)
```

## 字典Dictionary

{} 无序的对象集合，通过键来存取值。

```python
dict1 = {}
dict1['one'] = "This is one"
dict1[2] = "This is two"

tinydict1 = {'name': 'john', 'code': 6734, 'dept': 'sales'}

print(dict1['one'])  # 输出键为'one' 的值
print(dict1[2])  # 输出键为 2 的值
print(tinydict1)  # 输出完整的字典
print(tinydict1.keys())  # 输出所有键
print(tinydict1.values())  # 输出所有值
```

字典遍历

```python
for key in dict.keys():
    print(key)

for value in dict.values():
    print(value)

for item in dict.items():
    print(item)

for key,value in dict.items():
    print("key=%s"%key, "valu=%s"%value)
```

## 集合Set

无序，不重复集合不能被切片也不能被索引

```python
a_set = {1, 3, 5, 2, 4}
a_set.add(7)
a_set.discard(5)
```

## 栈

## 队列

## 堆

## 树

## 图