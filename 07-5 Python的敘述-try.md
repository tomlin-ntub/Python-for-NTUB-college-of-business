# 07-5 Python的敘述-try

### 用try敘述捕捉不預期的例外.


## [範例-1] 畫面示例
![GitHub Logo](/images/07a-5-1.jpg)

## [範例-1] 程式
```python
#--------------------------
# 檢查是否為數值
#--------------------------
try:
    score=int(input('輸入成績'))

    if score>=60:
        print('及格')
    else:
        print('不及格')
except ValueError:
    print('輸入錯誤') 
```



## [範例-1] 執行結果
```
輸入成績 a
輸入錯誤
```



## [範例-2] 程式
```python
#--------------------------
# 檢查是否為合理範圍的數值
#--------------------------
try:
    score=int(input('輸入成績'))

    if score>100 or score<0:
        raise ValueError
    else:
        if score>=60:
            print('及格')
        else:
            print('不及格')
except ValueError:
    print('輸入錯誤') 
```



## [範例-2] 執行結果
```
輸入成績 0
不及格
```
