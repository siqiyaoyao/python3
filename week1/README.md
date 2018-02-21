#INFO

## vim
vim xxx.py 创建Python 文件并进入
i 进入键入模式
:wq 回车 保存文件并退出

```
#! Shebang 告诉shell使用Python解释器执行下列代码
#!/usr/bin/env python 这种用法是为了防止操作系统用户没有将python装在默认的/usr/bin路径里。当系统看到这一行的时候，首先会到env设置里查找python的安装路径，再调用对应路径下的解释器程序完成操作。
```
chmod +x xxx 为文件添加可执行权限

## python 规则
使用4个空格来缩进，不要混用空格和制表符
函数之间空一行
类之间空两行
，：之后加一个空格
运算符加空格，括号不用
```
# 字符到行尾之间的东西为注释
```
import math 来加载模块

不需要定义变量，自动转义，“”，‘’都可定义字符串 /来转义符号

## python函数
input() 打印屏幕上的字符串参数，返回用户输入字符串
str.format()字符串格式化  
"Year {} Rs. {:.2f}".format(year, value)
year会填充第一个{} value会填充第二个{}转换为2位精度的浮点数

## 数据类型
### 元组tuple
用逗号创建元组
data = ("a","b");
name,country = data
name // a
country // 

### 列表
a = [0,1,2,3,4]

a[0,-1]// 0 1 2 3
省略的第一个索引默认为零，第二个为切片字符串大小

a[1::2]// 1 3
2 为补偿，从切片索引1开始到列表末尾，每隔两个元素取值 

in来搜索
1 in a // true

le(a) 长度
5 

循环 
for x in a
    print(x)

range() 生成等差数列
list(range(4,15,2))
[4,6,8,10,12,14]

