# 09-1 使用pandas模組-選擇單一欄位

### 使用pandas模組讀入csv檔, 得到一個data frame.

以下是一個讀入「iris.csv」檔案, 得到data frame的例子:

## [範例-1] 畫面示例
![GitHub Logo](/images/06-1-1.jpg)

## [範例-1] 程式
```python
#----------------------------------
# 匯入pandas模組
#----------------------------------
import pandas as pd

#----------------------------------
# 用pandas的read_csv()讀入資料,
# 讀入的結構是一個 data frame
#----------------------------------
df = pd.read_csv('iris.csv', names=['sepalL', 'sepalW', 'petalL', 'petalW', 'species'])

#所有內容
print(df)

#所有記錄的單一欄位
print(df['sepalL'])

#有條件部分記錄的單一欄位
print(df['sepalL'][df['species']=='山鳶尾花'])   
```

## [範例-1] 執行結果
```
     sepalL  sepalW  petalL  petalW  species
0       5.1     3.5     1.4     0.2     山鳶尾花
1       4.9     3.0     1.4     0.2     山鳶尾花
2       4.7     3.2     1.3     0.2     山鳶尾花
3       4.6     3.1     1.5     0.2     山鳶尾花
4       5.0     3.6     1.4     0.2     山鳶尾花
5       5.4     3.9     1.7     0.4     山鳶尾花
6       4.6     3.4     1.4     0.3     山鳶尾花
7       5.0     3.4     1.5     0.2     山鳶尾花
8       4.4     2.9     1.4     0.2     山鳶尾花
9       4.9     3.1     1.5     0.1     山鳶尾花
10      5.4     3.7     1.5     0.2     山鳶尾花
...(略)
```

## [範例-1] 輸入檔
資料來源:[UCI dataset] https://archive.ics.uci.edu/ml/datasets.html

```
[花萼長], [花萼寬], [花瓣長], [花瓣寬], [花名]
```


```
5.1,3.5,1.4,0.2,山鳶尾花
4.9,3.0,1.4,0.2,山鳶尾花
4.7,3.2,1.3,0.2,山鳶尾花
4.6,3.1,1.5,0.2,山鳶尾花
5.0,3.6,1.4,0.2,山鳶尾花
5.4,3.9,1.7,0.4,山鳶尾花
4.6,3.4,1.4,0.3,山鳶尾花
5.0,3.4,1.5,0.2,山鳶尾花
4.4,2.9,1.4,0.2,山鳶尾花
4.9,3.1,1.5,0.1,山鳶尾花
5.4,3.7,1.5,0.2,山鳶尾花
4.8,3.4,1.6,0.2,山鳶尾花
4.8,3.0,1.4,0.1,山鳶尾花
4.3,3.0,1.1,0.1,山鳶尾花
5.8,4.0,1.2,0.2,山鳶尾花
5.7,4.4,1.5,0.4,山鳶尾花
5.4,3.9,1.3,0.4,山鳶尾花
5.1,3.5,1.4,0.3,山鳶尾花
5.7,3.8,1.7,0.3,山鳶尾花
5.1,3.8,1.5,0.3,山鳶尾花
5.4,3.4,1.7,0.2,山鳶尾花
5.1,3.7,1.5,0.4,山鳶尾花
4.6,3.6,1.0,0.2,山鳶尾花
5.1,3.3,1.7,0.5,山鳶尾花
4.8,3.4,1.9,0.2,山鳶尾花
5.0,3.0,1.6,0.2,山鳶尾花
5.0,3.4,1.6,0.4,山鳶尾花
5.2,3.5,1.5,0.2,山鳶尾花
5.2,3.4,1.4,0.2,山鳶尾花
4.7,3.2,1.6,0.2,山鳶尾花
4.8,3.1,1.6,0.2,山鳶尾花
5.4,3.4,1.5,0.4,山鳶尾花
5.2,4.1,1.5,0.1,山鳶尾花
5.5,4.2,1.4,0.2,山鳶尾花
4.9,3.1,1.5,0.1,山鳶尾花
5.0,3.2,1.2,0.2,山鳶尾花
5.5,3.5,1.3,0.2,山鳶尾花
4.9,3.1,1.5,0.1,山鳶尾花
4.4,3.0,1.3,0.2,山鳶尾花
5.1,3.4,1.5,0.2,山鳶尾花
5.0,3.5,1.3,0.3,山鳶尾花
4.5,2.3,1.3,0.3,山鳶尾花
4.4,3.2,1.3,0.2,山鳶尾花
5.0,3.5,1.6,0.6,山鳶尾花
5.1,3.8,1.9,0.4,山鳶尾花
4.8,3.0,1.4,0.3,山鳶尾花
5.1,3.8,1.6,0.2,山鳶尾花
4.6,3.2,1.4,0.2,山鳶尾花
5.3,3.7,1.5,0.2,山鳶尾花
5.0,3.3,1.4,0.2,山鳶尾花
7.0,3.2,4.7,1.4,變色鳶尾花
6.4,3.2,4.5,1.5,變色鳶尾花
6.9,3.1,4.9,1.5,變色鳶尾花
5.5,2.3,4.0,1.3,變色鳶尾花
6.5,2.8,4.6,1.5,變色鳶尾花
5.7,2.8,4.5,1.3,變色鳶尾花
6.3,3.3,4.7,1.6,變色鳶尾花
4.9,2.4,3.3,1.0,變色鳶尾花
6.6,2.9,4.6,1.3,變色鳶尾花
5.2,2.7,3.9,1.4,變色鳶尾花
5.0,2.0,3.5,1.0,變色鳶尾花
5.9,3.0,4.2,1.5,變色鳶尾花
6.0,2.2,4.0,1.0,變色鳶尾花
6.1,2.9,4.7,1.4,變色鳶尾花
5.6,2.9,3.6,1.3,變色鳶尾花
6.7,3.1,4.4,1.4,變色鳶尾花
5.6,3.0,4.5,1.5,變色鳶尾花
5.8,2.7,4.1,1.0,變色鳶尾花
6.2,2.2,4.5,1.5,變色鳶尾花
5.6,2.5,3.9,1.1,變色鳶尾花
5.9,3.2,4.8,1.8,變色鳶尾花
6.1,2.8,4.0,1.3,變色鳶尾花
6.3,2.5,4.9,1.5,變色鳶尾花
6.1,2.8,4.7,1.2,變色鳶尾花
6.4,2.9,4.3,1.3,變色鳶尾花
6.6,3.0,4.4,1.4,變色鳶尾花
6.8,2.8,4.8,1.4,變色鳶尾花
6.7,3.0,5.0,1.7,變色鳶尾花
6.0,2.9,4.5,1.5,變色鳶尾花
5.7,2.6,3.5,1.0,變色鳶尾花
5.5,2.4,3.8,1.1,變色鳶尾花
5.5,2.4,3.7,1.0,變色鳶尾花
5.8,2.7,3.9,1.2,變色鳶尾花
6.0,2.7,5.1,1.6,變色鳶尾花
5.4,3.0,4.5,1.5,變色鳶尾花
6.0,3.4,4.5,1.6,變色鳶尾花
6.7,3.1,4.7,1.5,變色鳶尾花
6.3,2.3,4.4,1.3,變色鳶尾花
5.6,3.0,4.1,1.3,變色鳶尾花
5.5,2.5,4.0,1.3,變色鳶尾花
5.5,2.6,4.4,1.2,變色鳶尾花
6.1,3.0,4.6,1.4,變色鳶尾花
5.8,2.6,4.0,1.2,變色鳶尾花
5.0,2.3,3.3,1.0,變色鳶尾花
5.6,2.7,4.2,1.3,變色鳶尾花
5.7,3.0,4.2,1.2,變色鳶尾花
5.7,2.9,4.2,1.3,變色鳶尾花
6.2,2.9,4.3,1.3,變色鳶尾花
5.1,2.5,3.0,1.1,變色鳶尾花
5.7,2.8,4.1,1.3,變色鳶尾花
6.3,3.3,6.0,2.5,維吉尼亞鳶尾花
5.8,2.7,5.1,1.9,維吉尼亞鳶尾花
7.1,3.0,5.9,2.1,維吉尼亞鳶尾花
6.3,2.9,5.6,1.8,維吉尼亞鳶尾花
6.5,3.0,5.8,2.2,維吉尼亞鳶尾花
7.6,3.0,6.6,2.1,維吉尼亞鳶尾花
4.9,2.5,4.5,1.7,維吉尼亞鳶尾花
7.3,2.9,6.3,1.8,維吉尼亞鳶尾花
6.7,2.5,5.8,1.8,維吉尼亞鳶尾花
7.2,3.6,6.1,2.5,維吉尼亞鳶尾花
6.5,3.2,5.1,2.0,維吉尼亞鳶尾花
6.4,2.7,5.3,1.9,維吉尼亞鳶尾花
6.8,3.0,5.5,2.1,維吉尼亞鳶尾花
5.7,2.5,5.0,2.0,維吉尼亞鳶尾花
5.8,2.8,5.1,2.4,維吉尼亞鳶尾花
6.4,3.2,5.3,2.3,維吉尼亞鳶尾花
6.5,3.0,5.5,1.8,維吉尼亞鳶尾花
7.7,3.8,6.7,2.2,維吉尼亞鳶尾花
7.7,2.6,6.9,2.3,維吉尼亞鳶尾花
6.0,2.2,5.0,1.5,維吉尼亞鳶尾花
6.9,3.2,5.7,2.3,維吉尼亞鳶尾花
5.6,2.8,4.9,2.0,維吉尼亞鳶尾花
7.7,2.8,6.7,2.0,維吉尼亞鳶尾花
6.3,2.7,4.9,1.8,維吉尼亞鳶尾花
6.7,3.3,5.7,2.1,維吉尼亞鳶尾花
7.2,3.2,6.0,1.8,維吉尼亞鳶尾花
6.2,2.8,4.8,1.8,維吉尼亞鳶尾花
6.1,3.0,4.9,1.8,維吉尼亞鳶尾花
6.4,2.8,5.6,2.1,維吉尼亞鳶尾花
7.2,3.0,5.8,1.6,維吉尼亞鳶尾花
7.4,2.8,6.1,1.9,維吉尼亞鳶尾花
7.9,3.8,6.4,2.0,維吉尼亞鳶尾花
6.4,2.8,5.6,2.2,維吉尼亞鳶尾花
6.3,2.8,5.1,1.5,維吉尼亞鳶尾花
6.1,2.6,5.6,1.4,維吉尼亞鳶尾花
7.7,3.0,6.1,2.3,維吉尼亞鳶尾花
6.3,3.4,5.6,2.4,維吉尼亞鳶尾花
6.4,3.1,5.5,1.8,維吉尼亞鳶尾花
6.0,3.0,4.8,1.8,維吉尼亞鳶尾花
6.9,3.1,5.4,2.1,維吉尼亞鳶尾花
6.7,3.1,5.6,2.4,維吉尼亞鳶尾花
6.9,3.1,5.1,2.3,維吉尼亞鳶尾花
5.8,2.7,5.1,1.9,維吉尼亞鳶尾花
6.8,3.2,5.9,2.3,維吉尼亞鳶尾花
6.7,3.3,5.7,2.5,維吉尼亞鳶尾花
6.7,3.0,5.2,2.3,維吉尼亞鳶尾花
6.3,2.5,5.0,1.9,維吉尼亞鳶尾花
6.5,3.0,5.2,2.0,維吉尼亞鳶尾花
6.2,3.4,5.4,2.3,維吉尼亞鳶尾花
5.9,3.0,5.1,1.8,維吉尼亞鳶尾花
```


