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

a = []
b = []
a.append(x) 将x元素放到列表末尾
a.insert(0，x) 在列表索引0位置添加元素x
a.count(x) 返回x在列表中出现的次数
a.remove(x) 移除任意指定值
a.reverse() 反转整个列表
a.attend(b) 添加b的元素 而不是b本身
a.sort() 排序
del a[-1] 航处制定位置的列表元素



## 数据类型
### 元组tuple
用逗号创建元组
data = ("a","b");
name,country = data
name // a
country // 
元组是由数个逗号分割的值组成
元祖不可变类型，不能在元组内删除或添加或编辑任何值

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

列表推导式
a = [result for x in b ]
for x in b
    result

### 集合
集合是一个无需不重复的元素集。支持union联合，intersection交，difference差和symmetric difference对称差集
{}或者set()可以创建集合
如果创建空集合必须用set()
a.pop()弹出最后一个
a.add('x')在0位置加入元素x

### 字典
字典是无序的键值对（key:value），键必须互不相同，用{}来创建
a[key]来取值 但是如果key不存在 则会报错 所以用
dict.get(key,default)来索引
a[key1] = value1 在尾部加入配对
del a[key] 来删除
in 来查找
dict() 可以从包含键值对的元组中创建字典

遍历用items()来使用
for x, y in data.items():

遍历列表的同时获得元素索引
for i, j in enumerate(['a', 'b', 'c'])

同时遍历两个序列类型zip()
for x, y in zip(a,b):


data.setdefault(('name',[]).append('Ruby'))


### 栈和队列
栈 后进先出
a = [1,2,3]
a.pop() // 3
b = [1,2,3]
b.pop(0)//1

队列 先进先出

## 字符串
‘’ "" 一行字符串
''' ''' """ """ 多行字符串，报货换行符
s.split() 按括号内的元素对字符串进行分割 返回字符串列表
"-".join() 使用指定字符连接多个字符串 
s.title() 返回字符串标题版本
s.upper() 大写
s.lower() 小写
s.swapcase() 交换大小写
s.isalnum(）检查所有字符是否为字母数字（空格不算字符）
s.isalpha() 检查字符串之中是否只有字母

### 字符串剥离
s.strip() 剥离字符串首尾中指定的字符 默认剥离首尾的空格和换行符
s.lstrip() 剥离左边
s.rstrip() 剥离右边
s.find() 搜索字符串里的文本或子字符串 返回字符串首字母的index 没找到则为-1
s.startswith("fa") 检查字符串是否以fa开头
s.endswith("reason") 检查字符串是否以 reason 结尾

回文
z = s[::-1]

"%d" % (变量)



