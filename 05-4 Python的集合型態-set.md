# 05-4 Python的集合型態-set

### 在Python中宣告一個set(集合)物件, 由一對大括號, 其中包括的多個由逗點隔開的元素組成. 在set中的元素不會重覆, 而set物件內容可在設定後再增減(mutable).


## [範例-1] 畫面示例
![GitHub Logo](/images/05a-4-1.jpg)

## [範例-1] 程式
```python
#-----------------------
# 建立一個set物件
#-----------------------
a={2, 4, 5, 6, 2, 1, 4, 6, 8, 9}

#----------------------------------
# 印出a中的所有元素(沒有重覆內容)
#----------------------------------
for i in a:
    print(i)   
```

## [範例-1] 執行結果
```
1
2
4
5
6
8
9
```


##  可以操作在集合型態的運算, 包括set(mutable)及frozenset(immutable)

#### 完整資料建議查看Python文件
```
len(s)
x in s
x not in s
isdisjoint(other)
issubset(other)
set <= other
set < other
issuperset(other)
set >= other
set > other
union(*others)
set | other | ...
intersection(*others)
set & other & ...
difference(*others)
set - other - ...
symmetric_difference(other)
set ^ other
copy()
```

## [範例-2] 程式
```python
#--------------------
# 建立一個set物件
#--------------------
a={2, 4, 5, 6, 2, 1, 4, 6, 8, 9}

print(a)
print('-'*30)

#--------------------
# 是否存在set中
#--------------------
print('10是否存在:', 10 in a)
print('-'*30) 

print('5是否存在:', 5 in a)
print('-'*30) 

#--------------------
# 長度
#--------------------
print('長度:', len(a))
print('-'*30) 
```

## [範例-2] 執行結果
```
{1, 2, 4, 5, 6, 8, 9}
------------------------------
10是否存在: False
------------------------------
5是否存在: True
------------------------------
長度: 7
------------------------------
```



## [範例-3] 程式
```python
#--------------------
# 建立2個set物件
#--------------------
a={5, 6, 8, 9, 3, 1, 8, 7, 5};
b={5, 6, 12, 18, 20}

print('a集合:', a)
print('b集合:',b)
print('-'*40)

print('a,b交集', a & b)
print('a,b聯集', a | b)
print('a,b差集', a - b)
print('-'*40)
```

## [範例-3] 執行結果
```
a集合: {1, 3, 5, 6, 7, 8, 9}
b集合: {5, 6, 12, 18, 20}
----------------------------------------
a,b交集 {5, 6}
a,b聯集 {1, 3, 5, 6, 7, 8, 9, 12, 18, 20}
a,b差集 {1, 3, 7, 8, 9}
----------------------------------------
```



## 可以操作在set型別的mutable運算

#### 完整資料建議查看Python文件
```
update(*others)
set |= other | ...
Update the set, adding elements from all others.

intersection_update(*others)
set &= other & ...
Update the set, keeping only elements found in it and all others.

difference_update(*others)
set -= other | ...
Update the set, removing elements found in others.

symmetric_difference_update(other)
set ^= other
Update the set, keeping only elements found in either set, but not in both.

add(elem)
Add element elem to the set.

remove(elem)
Remove element elem from the set. Raises KeyError if elem is not contained in the set.

discard(elem)
Remove element elem from the set if it is present.

pop()
Remove and return an arbitrary element from the set. Raises KeyError if the set is empty.

clear()
Remove all elements from the set.
```


## [範例-4] 程式
```python
#--------------------
# 建立1個set物件
#--------------------
a={5, 6, 8, 9, 3, 1, 8, 7, 5};

print(a)
print(type(a))
print('-'*30)

#--------------------
# 增加1個元素
#--------------------
a.add(10)
print('加入10')
print(a)
print('-'*30)

#--------------------
# 刪除set中符合元素
#--------------------
a.remove(5)
print('刪除5')
print(a)
print('-'*30)
```

## [範例-4] 執行結果
```
{1, 3, 5, 6, 7, 8, 9}
<class 'set'>
------------------------------
加入10
{1, 3, 5, 6, 7, 8, 9, 10}
------------------------------
刪除5
{1, 3, 6, 7, 8, 9, 10}
------------------------------
```
