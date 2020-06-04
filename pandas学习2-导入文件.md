# pandas学习2-导入文件
import pandas as pd

pd.options.display.max_rows=10

## 读取文件
pd.read_csv( filepath_or_buffer : 要读入的文件路径

sep = ',' : 列分割符

header = 'infer' : 指定数据中的第几行作为变量名

names = None : 自定义变量名列表

index_col = None : 将会被工作索引的列名，多列时只能用作序号列表

usecols = None : 指定只读入某些列，使用索引列表或者名称列表均可以

encoding = None : 读入文件的编码

utf-8/gbk,中文数据最好设定为utf-8
na_values : 指定将被读入为缺失值的数值列表，默认下列数据被读入为缺失值：

'','#N/A','#N/A N/A'等
)：读取CSV格式文件，但也可通用与文本文件读取
## 导入CSV文件
df2 = pd.read_csv(r"daxuebumen.csv",encoding = "gbk")

df2
## pandas.read_table(): 更通用与文本文件读取命令
## 导入文本文件
df2 = pd.read_table(r"daxuebumen.csv",sep=",",encoding="gbk")

df2
