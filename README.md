# 整数浮点数操作实验

## 目标
熟悉整型和浮点型数据的编码方式，熟悉C/C++中的位操作运算。

## 要求
请按照要求补全 bits.c 中的函数，并进行验证。包括以下7个函数：

### a. int conditional(int x, int y, int z)
* 功能：实现与三目运算符表达式 x ? y : z 具有等价功能的函数
* 合法的运算符：! ~ & ^ | + << >>
* 可使用的运算符数：16
* 难度：4

### b. int isNonNegative(int x)
* 功能：当 x >=0 时，返回1；否则返回0
* 合法的运算符：! ~ & ^ | + << >>
* 可使用的运算符数：6
* 难度：3

### c. int isGreater(int x, int y)
* 功能：当 x > y 时，返回1，否则返回0
* 合法的运算符：! ~ & ^ | + << >>
* 可使用的运算符数：24
* 难度：3

### d. int absVal(int x)
* 功能：计算x的绝对值
* 合法的运算符：! ~ & ^ | + << >>
* 可使用的运算符数：10
* 难度：4

### e. int isPower2(int x)
* 功能：判断x是否恰好等于 $2^n$，如果等于则返回1，否则返回0
* 提示：负数必然不是$2^n$
* 示例：isPower2(5) = 0, isPower2(8) = 1, isPower2(0) = 0
* 合法的运算符：! ~ & ^ | + << >>
* 可使用的运算符数：20
* 难度：4

### f. unsigned float_neg(unsigned uf)
* 功能：求浮点数f的相反数
* 说明：参数uf为浮点数f为在计算机中的二进制编码所对应的无符号数。返回值为浮点数-f在计算机中的二进编码所对应的无符号数。
* 合法的运算符：全部有符号数和无符号数的运算符、||、&&、if 和 while
* 注意：如果输入为NaN，则返回值等于uf
* 可使用的运算符数：10
* 难度：2

### g. unsigned float_i2f(int x)
* 功能：返回浮点数(float)x在计算机中的二进制编码所对应的无符号数
* 合法的运算符：全部有符号数和无符号数的运算符、||、&&、if 和 while
* 可使用的运算符数：30
* 难度：4

### 程序内允许使用：
a. 每个题目所规定的合法运算符（注意：题f-g所规定的合法运算符与题a-e不同）
b. 范围在0 - 255之间的常数
c. 局部变量

### 程序内禁止以下行为：
a. 声明和使用全局变量
b. 声明和使用定义宏
c. 声明和调用其他的函数
d. 类型的强制转换
e. 使用许可范围之外的运算符
f. 使用控制跳转语句：if else switch do while for

#### 注意：违背以上原则均视为程序不正确！！

## 评价方法
本次作业总分共38分，其中包括：

* 正确分：24

    每个题目都有对应的难度系数，正确完成一道题目则会获得和该题难度系数相同的分值。难度系数总和为24。

* 性能分：14

    每到题目都可以使用布尔代数的方法进行暴力求解。但是，我希望大家能够使用一些更聪明和更优雅的方式来解题。因此，我们对每个题目所使用运算符总数进行了限制，如果该题结果正确且运算符总数满足题目要求，则该题获得2分性能分。


## 一些说明
与实验1相同。

## 实验文件的位置
在simpleedu用户目录的lab2目录下

## simpleedu用户密码
Simplexue123

## 提交方法
执行make命令成功编译后，会自动生成lab2-handing.zip文件。将该文件上传至系统。不需要填写实验报告。

## 说明

本实验引用自 https://www.csapp.cs.cmu.edu/