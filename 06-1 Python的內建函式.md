# 06-1 Python的內建函式

### Python提供了許多內建函式, 不需引入模組即可使用. 各個函式使用方法可查看Python文件.


## [範例-1] 畫面示例
![GitHub Logo](/images/06a-1-1.jpg)

## [範例-1] 程式
```python
#--------------------
# 建立一個list物件
#--------------------
test=[True, False, True, True, True]

#--------------------
# 全部為真的判斷
#--------------------
print('是否全部成立:', all(test))
print('-'*30)   

#--------------------
# 任一為真的判斷
#--------------------
print('是否任一成立:', any(test))
print('-'*30)    

#--------------------
# ASCII轉文字
#--------------------
c = chr(65)
print(c)
print(type(c))
print('-'*30)
```

## [範例-1] 執行結果
```
是否全部成立: False
------------------------------
是否任一成立: True
------------------------------
A
<class 'str'>
------------------------------
```


#### 一些Python的內建函式

```
abs()
dict()
help()
min()
setattr()
all()
dir()
hex()
next()
slice()
any()
divmod()
id()
object()
sorted()
ascii()
enumerate()	
input()
oct()
staticmethod()
bin()
eval()
int()
open()
str()
bool()
exec()
isinstance()
ord()
sum()
bytearray()
filter()
issubclass()
pow()
super()
bytes()
float()
iter()
print()
tuple()
callable()
format()
len()
property()
type()
chr()
frozenset()
list()
range()
vars()
classmethod()
getattr()
locals()
repr()
zip()
compile()
globals()
map()
reversed()
__import__()
complex()
hasattr()
max()
round()	 
delattr()
hash()
memoryview()
set()	 
```
