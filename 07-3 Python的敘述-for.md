# 07-3 Python的敘述-for

### 用for進行重覆的工作. 迴圈內的敘述應該有相同的內縮.


## [範例-1] 畫面示例
![GitHub Logo](/images/07a-3-1.jpg)

## [範例-1] 程式
```python
#-------------------------
# 一個範圍的迴圈
#-------------------------
for i in range(10):
    print(i)  
```


## [範例-1] 執行結果
```
0
1
2
3
4
5
6
7
8
9
```


## [範例-2] 程式
```python
#-------------------------
# 一個迭代物件(str)的迴圈
#-------------------------
msg='今天天氣很好'

for s in msg:
    print(s)   
```


## [範例-2] 執行結果 (亂數數值, 內容不可預期)
```
今
天
天
氣
很
好
```



## [範例-3] 程式
```python
#-------------------------
# 一個迭代物件(list)的迴圈
#-------------------------
data=[10, 20, 30, 40, 50]

for d in data:
    print(d)   
```


## [範例-3] 執行結果 (亂數數值, 內容不可預期)
```
10
20
30
40
50
```



