# 01 Python基本架構

## 先建立Python整體架構概念, 避免實際撰寫Python程式時, 迷失在Python的某個角落之間.

#### 參考資料:https://docs.python.org/3/library/index.html

```
     Python
        |___ 1.指令敘述(statements)
        |       |___ if
        |       |___ for
        |       |___ while
        |       |___ with
        |       |___ import
        |       |___ try...except
        |       |___ ...        
        |
        |___ 2.運算子(operators)      
        |       |___ +, -, *, /
        |       |___ //, %
        |       |___ **
        |       |___ is, is not
        |       |___ ...
        |          
        |___ 3.內建(built-in)
        |       |
        |       |___ 3-1.型態(types)
        |       |        |__ <基本型態>
        |       |        |       |__ int
        |       |        |       |__ float
        |       |        |       |__ bool
        |       |        |       |__ str
        |       |        |
        |       |        |__ <序列型態>
        |       |        |       |__ list
        |       |        |       |__ range
        |       |        |       |__ tuple
        |       |        |
        |       |        |__ <集合型態>
        |       |        |       |__ set
        |       |        |
        |       |        |__ <映對型態>
        |       |        |       |__ dict 
        |       |        |__ ...
        |       |        
        |       |___ 3-2.函式(functions)
        |                |__ split()
        |                |__ sort()
        |                |__ strip()
        |                |__ slice()  
        |                |__ ...     
        |        
        | 
        |___ 4.加匯模組(import modules)
                |
                |___ 4-1.外部模組  
                |        |__ numpy  
                |        |__ scipy
                |        |__ pandas
                |        |__ sklearn
                |        |__ math 
                |        |__ matplotlib              
                |        |__ jieba
                |        |__ statistics
                |        |__ collections
                |        |__ .......
                |              
                |___ 4-2.自製模組 
                         |__ .......  
                         |__ .......
                         |__ .......               
                
```
