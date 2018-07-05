# 07-1 Python的敘述-if

### 用if進行不同情況的處理. 撰寫時, 同一條件內的敘述應有相同的縮行.


## [範例-1] 畫面示例
![GitHub Logo](/images/07a-1-1.jpg)

## [範例-1] 程式
```python
#---------------------------
# 使用者輸入成績
#---------------------------
score=int(input('成績:'))

#---------------------------
# if判斷
#---------------------------
if score>=90:
    rank='優等'
elif score>=80 and score<90:
    rank='甲等'
elif score>=70 and score<80:
    rank='乙等'
elif score>=60 and score<70:
    rank='丙等'
else:
    rank='丁等'    

print('等第: {}'.format(rank))    
```


## [範例-1] 執行結果 (輸入90分的情況)
```
成績: 90
等第: 優等
```

