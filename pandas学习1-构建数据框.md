# Pandas 学习
## 导入pandas
import pandas as pd
## 设定自由列表输出最多10行
pd.options.display.max_rows = 10
## 查看pandas版本
pd.__version__
## 构建数据框
### 构建数据框，以列为变量
df1 = pd.DataFrame(
    {
        'var1':1.0,
        'var2':[1,2,3,4],
        'var3':['a','b','c','d'],
        'var4':'cons'
    }
)
df1
### 以行为变量
df1 = pd.DataFrame(data=[[1,'text'],[2,'train'],
                         [3,'text'],[4,'train']],
                   columns=['var1', 'var2']
                  )
df1
