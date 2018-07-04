# 04-2 Python的文字-切割文字

### Python的文字資料可以使用「中括號」選擇文字段落.  

以下是一個使用文字資料的例子:

## [範例-1] 畫面示例
![GitHub Logo](/images/04-2-1.jpg)

## [範例-1] 程式
```python
#---------------------------
# 切割文字範例
#---------------------------
a='國立臺北商業大學'

#切割前2個字
b=a[0:2]    

#切割後2個字
k=len(a)    
c=a[k-2:k]

#印出結果
print(a)
print(b)
print(c)
```

## [範例-1] 執行結果
```
國立臺北商業大學
國立
大學
```



## [範例-2] 程式
```python
#------------------------
# 建立一個str物件
#------------------------
sentence='With legacies as varied as its adventure landscape and spirited traditions thriving alongside the cream of Asian sophistication, Taiwan is a continent on one green island.'

print(sentence)
print('-'*30)

#------------------------
# str的方法
#------------------------
print('轉大寫')
print(sentence.upper()) 
print('-'*30)

#------------------------
# str的方法
#------------------------
print('結束文字檢查')
print(sentence.endswith('.')) 
print(sentence.endswith('?')) 
print('-'*30)

#------------------------
# str的方法
#------------------------
print('更改文字')
print(sentence.replace('Taiwan', 'TAIWAN')) 
print('-'*30)

#------------------------
# str的方法
#------------------------
print('切割文字')
print(sentence.split(' ')) 
print('-'*30)
```

## [範例-2] 執行結果
```
With legacies as varied as its adventure landscape and spirited traditions thriving alongside the cream of Asian sophistication, Taiwan is a continent on one green island.
------------------------------
轉大寫
WITH LEGACIES AS VARIED AS ITS ADVENTURE LANDSCAPE AND SPIRITED TRADITIONS THRIVING ALONGSIDE THE CREAM OF ASIAN SOPHISTICATION, TAIWAN IS A CONTINENT ON ONE GREEN ISLAND.
------------------------------
結束文字檢查
True
False
------------------------------
更改文字
With legacies as varied as its adventure landscape and spirited traditions thriving alongside the cream of Asian sophistication, TAIWAN is a continent on one green island.
------------------------------
切割文字
['With', 'legacies', 'as', 'varied', 'as', 'its', 'adventure', 'landscape', 'and', 'spirited', 'traditions', 'thriving', 'alongside', 'the', 'cream', 'of', 'Asian', 'sophistication,', 'Taiwan', 'is', 'a', 'continent', 'on', 'one', 'green', 'island.']
------------------------------



```
