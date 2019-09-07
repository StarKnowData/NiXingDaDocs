# 人工智能必备数学基础与 Python 实现[www.nixingda.com 社区]


## 第1章 高等数学基础

### 1-1 课程简介
本课程是针对51CTO学院唐宇迪老师的课程<<人工智能-必备数学基础视频课程>>的课堂笔记和 Python 实现,文章无意侵权,也希望看到本文的人去 https://edu.51cto.com/course/14225.html 进行购买学习.

* 课程目标
掌握数据科学中必备的数学基础
* 适用人群
人工智能与数据科学方向的同学们
* 课程简介
数据科学与人工智能必备数学基础课程旨在帮助同学们快速打下数学基础，通俗讲解其中每一个知识点。课程内容涉及高等数学，线性代数，概率论与统计学，同学们在学习过程中应当以理解为出发点并不需要死记每一个公式，快速掌握核心知识点。课程章节内容较多，零基础同学按顺序学习即可，有基础的同学们可以按照自己的需求来有选择的学习！

**唐宇迪**
讲师评分：4.9

计算机博士，著有《跟迪哥学机器学习》，人工智能培训专家，课程风格通俗易懂，用最接地气的讲解带领同学们进军AI。
![](2019-09-07-15678244267206.jpg)



笔记作者:林肯叔叔 

![](2019-09-07-15678449638400.jpg)



### 1-2-1 函数的数学定义
![-w1239](2019-09-07-15678245476542.jpg)

![-w1238](2019-09-07-15678438656889.jpg)


>[维基百科关于函数的介绍](https://zh.wikipedia.org/wiki/%E5%87%BD%E6%95%B0)

![](2019-09-07-15678347399104.jpg)

**函数**在[数学](https://zh.wikipedia.org/wiki/%E6%95%B0%E5%AD%A6 "数学")中为两不为空集的[集合](https://zh.wikipedia.org/wiki/%E9%9B%86%E5%90%88 "集合")间的一种对应关系：输入值集合中的每项元素皆能对应​​**唯一**一项输出值集合中的元素。例如[实数](https://zh.wikipedia.org/wiki/%E5%AE%9E%E6%95%B0 "实数")x对应到其[平方](https://zh.wikipedia.org/wiki/%E5%B9%B3%E6%96%B9 "平方")x<sup>2</sup>的关系就是一个函数，若以3作为此函数的输入值，所得的输出值便是9。
所得的输出值便是9。

为方便起见，一般做法是以符号 $ f,g,h $等等来指代一个函数。若函数$ f $以$ x $作为输入值，则其输出值一般写作 $ f(x)$，读作'f of x' 。上述的平方函数关系写成数学式记为$f(x)=x^2$。函数的概念并不局限于数之间的映射关系，例如若定义函数$ Captial() $为每个国家当前的首都，那么给予输入值**西班牙**就会输出唯一值**马德里**：$ Captial(Spain) = Mardrid $。 **气温**的分布也能用函数表达，以时间和地点作为参量输入，以该时该地的温度作为输出。表达函数有多种方式，例如解析法是用数学式表达两个变量之间的对应关系，图像法是用[坐标系](https://zh.wikipedia.org/wiki/%E5%9D%90%E6%A0%87%E7%B3%BB "坐标系")上的[函数图形](https://zh.wikipedia.org/wiki/%E5%87%BD%E6%95%B8%E5%9C%96%E5%BD%A2 "函数图形")表达两个变量之间的对应关系，列表法用表格表达两个变量之间的对应关系。

现代数学中，函数所有输入值的[集合](https://zh.wikipedia.org/wiki/%E9%9B%86%E5%90%88 "集合")被称作该函数的**[定义域](https://zh.wikipedia.org/wiki/%E5%AE%9A%E4%B9%89%E5%9F%9F "定义域")**，而其输出值所存在的集合称为**[到达域](https://zh.wikipedia.org/wiki/%E5%B0%8D%E6%87%89%E5%9F%9F "到达域")**。其中**[值域](https://zh.wikipedia.org/wiki/%E5%80%BC%E5%9F%9F "值域")**特指该函数的输出值集合，意即上域包含了值域，值域为上域的[子集](https://zh.wikipedia.org/wiki/%E5%AD%90%E9%9B%86 "子集")。通常输入值称作函数的**参数**或**参量**，输出值称作函数的**值**。函数将有效的输入值变换为唯一的输出值，同一输入总是对应同一输出，但反之未必成立。因此如$Root(x)=\pm \sqrt{x} $这样的表达式并没有定义出一个函数，因为输出值有两个可能。定义函数时需确定每一个输入值只对应唯一输出值，因此必须明确地选择一个平方根。例如定义$Posroot(x)=\sqrt{x} $，亦即对于任何非负输入值，选择其非负平方根作为函数值。

函数可以看作机器或[黑箱](https://zh.wikipedia.org/wiki/%E9%BB%91%E7%AE%B1 "黑箱")，通常最常见的函数的参数和函数值都是数字，其对应关系用函数式表示，函数值可以通过直接将参数值代入函数式得到。$f(x)=x^2$，$x$的平方即是函数值。也可以将函数很简单的推广到与多个参量相关的情况。例如$g(x,y)=xy$有两个参量$x$和$y$，以乘积$xy$为值。将这两个输入看作一个[有序对](https://zh.wikipedia.org/wiki/%E6%9C%89%E5%BA%8F%E5%AF%B9 "有序对")$(x,y)$。$g$即为以这个有序对$(x,y)$作参数的函数，而函数值是$xy$。函数能被抽象定义为某种[数学关系](https://zh.wikipedia.org/wiki/%E6%95%B0%E5%AD%A6%E5%85%B3%E7%B3%BB "数学关系")，由于其定义的一般性，在几乎所有的数学分支都是基础概念。一些领域中比如在[λ演算](https://zh.wikipedia.org/wiki/%CE%9B%E6%BC%94%E7%AE%97 "Λ演算")中，函数可以是作为一个原始概念而不像在[集合论](https://zh.wikipedia.org/wiki/%E9%9B%86%E5%90%88%E8%AB%96 "集合论")般有所定义。在大部分的数学领域内，术语[对应](https://zh.wikipedia.org/wiki/%E5%B0%8D%E6%87%89 "对应")、[映射](https://zh.wikipedia.org/wiki/%E6%98%A0%E5%B0%84 "映射")、[变换](https://zh.wikipedia.org/w/index.php?title=%E5%8F%98%E6%8D%A2&action=edit&redlink=1 "变换（页面不存在）")通常是函数的近义词。不过某些情况这些术语可能有别的特定意思，例如在[拓扑学](https://zh.wikipedia.org/wiki/%E6%8B%93%E6%89%91%E5%AD%A6 "拓扑学")中一个映射有时被定义成一个[连续函数](https://zh.wikipedia.org/wiki/%E8%BF%9E%E7%BB%AD%E5%87%BD%E6%95%B0 "连续函数")。

从输入值集合$X$到可能的输出值集合$Y$的函数$f$（记作$f: X\longrightarrow Y$）是$X$与$Y$的[关系](https://zh.wikipedia.org/wiki/%E4%BA%8C%E5%85%83%E5%85%B3%E7%B3%BB "二元关系")，满足如下条件：
1. $f$是完全的:对集合$X$中任一元素$x$都有集合$Y$中的元素$y$满足$xfy$($x$与$y$是$f$相关的).即,对每一个输入值,$y$中都有与之对应的输出量.
2. $f$是多对一的:若$f(x)=y$且$f(x)=z$,则$y=z$.即,多个输入可以映射一个输出,但每一个输入不能映射到多个输出.

![](2019-09-07-15678356703763.jpg)

表示方法:
* 描述法
* 表格
* 公式法
* 图形

![](2019-09-07-15678364753930.jpg)

![](2019-09-07-15678365396365.jpg)

函数范例

参见：[函数列表](https://zh.wikipedia.org/wiki/%E5%87%BD%E6%95%B0%E5%88%97%E8%A1%A8 "函数列表")

* 首都之于国家（若不把多首都国[[1]](http://geography.about.com/library/misc/bl2capitals.htm) 计算在内)。
* 每个[自然数](https://zh.wikipedia.org/wiki/%E8%87%AA%E7%84%B6%E6%95%B0 "自然数")$n$的平方$n^2$是$n$的函数。
* [对数函数](https://zh.wikipedia.org/wiki/%E5%AF%B9%E6%95%B0%E5%87%BD%E6%95%B0 "对数函数")。$\ln$是[正](https://zh.wikipedia.org/wiki/%E6%AD%A3%E6%95%B0 "正数")[实数](https://zh.wikipedia.org/wiki/%E5%AE%9E%E6%95%B0 "实数")$x$的函数。注意，虽然可以把对数函数推广到复数情况，但结果就不是函数了，而是多值函数。
* 对每个在$\mathbb {R} ^{2}$平面上的点，其和[原点](https://zh.wikipedia.org/wiki/%E5%8E%9F%E9%BB%9E "原点")$(0,0)$的距离是确定的。

常用的数学函数包括[多项式函数](https://zh.wikipedia.org/wiki/%E5%A4%9A%E9%A1%B9%E5%BC%8F%E5%87%BD%E6%95%B0 "多项式函数")、[根式函数](https://zh.wikipedia.org/w/index.php?title=%E6%A0%B9%E5%BC%8F%E5%87%BD%E6%95%B8&action=edit&redlink=1 "根式函数（页面不存在）")、[幂函数](https://zh.wikipedia.org/wiki/%E5%B9%82%E5%87%BD%E6%95%B0 "幂函数")、[对数函数](https://zh.wikipedia.org/wiki/%E5%AF%B9%E6%95%B0%E5%87%BD%E6%95%B0 "对数函数")、[有理函数](https://zh.wikipedia.org/wiki/%E6%9C%89%E7%90%86%E5%87%BD%E6%95%B8 "有理函数")、[三角函数](https://zh.wikipedia.org/wiki/%E4%B8%89%E8%A7%92%E5%87%BD%E6%95%B0 "三角函数")、[反三角函数](https://zh.wikipedia.org/wiki/%E5%8F%8D%E4%B8%89%E8%A7%92%E5%87%BD%E6%95%B0 "反三角函数")等。它们都是[初等函数](https://zh.wikipedia.org/wiki/%E5%88%9D%E7%AD%89%E5%87%BD%E6%95%B0 "初等函数")。非初等函数（或[特殊函数](https://zh.wikipedia.org/wiki/%E7%89%B9%E6%AE%8A%E5%87%BD%E6%95%B0 "特殊函数")）包括[伽马函数](https://zh.wikipedia.org/wiki/%E4%BC%BD%E9%A9%AC%E5%87%BD%E6%95%B0 "伽马函数")和[贝塞尔函数](https://zh.wikipedia.org/wiki/%E8%B4%9D%E5%A1%9E%E5%B0%94%E5%87%BD%E6%95%B0 "贝塞尔函数")等。

函数的特性

函数可分为

* [奇函数](https://zh.wikipedia.org/wiki/%E5%A5%87%E5%87%BD%E6%95%B8 "奇函数")或[偶函数](https://zh.wikipedia.org/wiki/%E5%81%B6%E5%87%BD%E6%95%B8 "偶函数")
* [连续函数](https://zh.wikipedia.org/wiki/%E9%80%A3%E7%BA%8C%E5%87%BD%E6%95%B8 "连续函数")或[不连续函数](https://zh.wikipedia.org/wiki/%E4%B8%8D%E9%80%A3%E7%BA%8C%E5%87%BD%E6%95%B8 "不连续函数")
* [实函数](https://zh.wikipedia.org/wiki/%E5%AE%9E%E5%87%BD%E6%95%B0 "实函数")或[虚函数](https://zh.wikipedia.org/wiki/%E8%99%9B%E5%87%BD%E6%95%B8 "虚函数")
* [标量函数](https://zh.wikipedia.org/w/index.php?title=%E7%B4%94%E9%87%8F%E5%87%BD%E6%95%B8&action=edit&redlink=1 "标量函数（页面不存在）")或[向量函数](https://zh.wikipedia.org/w/index.php?title=%E5%90%91%E9%87%8F%E5%87%BD%E6%95%B8&action=edit&redlink=1 "向量函数（页面不存在）")
* [单调增函数](https://zh.wikipedia.org/w/index.php?title=%E5%8D%95%E8%B0%83%E5%A2%9E%E5%87%BD%E6%95%B0&action=edit&redlink=1 "单调增函数（页面不存在）")或[单调减函数](https://zh.wikipedia.org/w/index.php?title=%E5%8D%95%E8%B0%83%E5%87%8F%E5%87%BD%E6%95%B0&action=edit&redlink=1 "单调减函数（页面不存在）")

分段函数

**分段函数**（德语：Abschnittsweise definierte Funktion），在定义域内不同部分上，有不同的解析表达式，这样的函数通常叫分段函数。

![](2019-09-07-15678423320684.jpg)
![](2019-09-07-15678423540313.jpg)


### 1.2 函数 Python 代码实现

* Python Number 类型转换

```
int(x [,base ])         将x转换为一个整数  
long(x [,base ])        将x转换为一个长整数  
float(x )               将x转换到一个浮点数  
complex(real [,imag ])  创建一个复数  
str(x )                 将对象 x 转换为字符串  
repr(x )                将对象 x 转换为表达式字符串  
eval(str )              用来计算在字符串中的有效Python表达式,并返回一个对象  
tuple(s )               将序列 s 转换为一个元组  
list(s )                将序列 s 转换为一个列表  
chr(x )                 将一个整数转换为一个字符  
unichr(x )              将一个整数转换为Unicode字符  
ord(x )                 将一个字符转换为它的整数值  
hex(x )                 将一个整数转换为一个十六进制字符串  
oct(x )                 将一个整数转换为一个八进制字符串  
```

* Python math 模块、cmath 模块  

Python 中数学运算常用的函数基本都在 math 模块、cmath 模块中。
Python math 模块提供了许多对浮点数的数学运算函数。
Python cmath 模块包含了一些用于复数运算的函数。
cmath 模块的函数跟 math 模块函数基本一致，区别是 cmath 模块运算的是复数，math 模块运算的是数学运算。
要使用 math 或 cmath 函数必须先导入：

```
import math
```
查看 math 查看包中的内容:

```
>>> import math
>>> dir(math)
['__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__', 'acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh', 'ceil', 'copysign', 'cos', 'cosh', 'degrees', 'e', 'erf', 'erfc', 'exp', 'expm1', 'fabs', 'factorial', 'floor', 'fmod', 'frexp', 'fsum', 'gamma', 'gcd', 'hypot', 'inf', 'isclose', 'isfinite', 'isinf', 'isnan', 'ldexp', 'lgamma', 'log', 'log10', 'log1p', 'log2', 'modf', 'nan', 'pi', 'pow', 'radians', 'sin', 'sinh', 'sqrt', 'tan', 'tanh', 'tau', 'trunc']
>>>
```

查看 cmath 查看包中的内容

```
>>> import cmath
>>> dir(cmath)
['__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__', 'acos', 'acosh', 'asin', 'asinh', 'atan', 'atanh', 'cos', 'cosh', 'e', 'exp', 'inf', 'infj', 'isclose', 'isfinite', 'isinf', 'isnan', 'log', 'log10', 'nan', 'nanj', 'phase', 'pi', 'polar', 'rect', 'sin', 'sinh', 'sqrt', 'tan', 'tanh', 'tau']
>>>
```

示例

```
>>> import cmath
>>> cmath.sqrt(-1)
1j
>>> cmath.sqrt(9)
(3+0j)
>>> cmath.sin(1)
(0.8414709848078965+0j)
>>> cmath.log10(100)
(2+0j)
>>>
```

* Python数学函数


函数                                                                     | 返回值 ( 描述 )                                             
---------------------------------------------------------------------- | -------------------------------------------------------
[abs(x)](https://www.runoob.com/python/func-number-abs.html)           | 返回数字的绝对值，如abs(-10) 返回 10                               
[ceil(x) ](https://www.runoob.com/python/func-number-ceil.html)        | 返回数字的上入整数，如math.ceil(4.1) 返回 5                         
[cmp(x, y)](https://www.runoob.com/python/func-number-cmp.html)        |  如果 x < y 返回 -1, 如果  x == y 返回 0,  如果 x > y 返回 1       
[exp(x) ](https://www.runoob.com/python/func-number-exp.html)          | 返回e的x次幂(e<sup>x</sup>),如math.exp(1) 返回2.718281828459045
[fabs(x)](https://www.runoob.com/python/func-number-fabs.html)         | 返回数字的绝对值，如math.fabs(-10) 返回10.0                        
[floor(x) ](https://www.runoob.com/python/func-number-floor.html)      | 返回数字的下舍整数，如math.floor(4.9)返回 4                         
[log(x) ](https://www.runoob.com/python/func-number-log.html)          | 如math.log(math.e)返回1.0,math.log(100,10)返回2.0           
[log10(x) ](https://www.runoob.com/python/func-number-log10.html)      | 返回以10为基数的x的对数，如math.log10(100)返回 2.0                   
[max(x1, x2,...) ](https://www.runoob.com/python/func-number-max.html) | 返回给定参数的最大值，参数可以为序列。                                    
[min(x1, x2,...) ](https://www.runoob.com/python/func-number-min.html) | 返回给定参数的最小值，参数可以为序列。                                    
[modf(x) ](https://www.runoob.com/python/func-number-modf.html)        | 返回x的整数部分与小数部分，两部分的数值符号与x相同，整数部分以浮点型表示。                 
[pow(x, y)](https://www.runoob.com/python/func-number-pow.html)        |  x**y 运算后的值。                                           
[round(x [,n])](https://www.runoob.com/python/func-number-round.html)  | 返回浮点数x的四舍五入值，如给出n值，则代表舍入到小数点后的位数。                      
[sqrt(x) ](https://www.runoob.com/python/func-number-sqrt.html)        | 返回数字x的平方根                                                

* Python随机数函数

随机数可以用于数学，游戏，安全等领域中，还经常被嵌入到算法中，用以提高算法效率，并提高程序的安全性。

Python包含以下常用随机数函数：

函数                                                                                             | 描述                                                       
---------------------------------------------------------------------------------------------- | ---------------------------------------------------------
[choice(seq)](https://www.runoob.com/python/func-number-choice.html)                           | 从序列的元素中随机挑选一个元素，比如random.choice(range(10))，从0到9中随机挑选一个整数。
[randrange ([start,] stop [,step]) ](https://www.runoob.com/python/func-number-randrange.html) | 从指定范围内，按指定基数递增的集合中获取一个随机数，基数默认值为 1                       
[random() ](https://www.runoob.com/python/func-number-random.html)                             |  随机生成下一个实数，它在[0,1)范围内。                                   
[seed([x]) ](https://www.runoob.com/python/func-number-seed.html)                              | 改变随机数生成器的种子seed。如果你不了解其原理，你不必特别去设定seed，Python会帮你选择seed。  
[shuffle(lst) ](https://www.runoob.com/python/func-number-shuffle.html)                        | 将序列的所有元素随机排序                                             
[uniform(x, y)](https://www.runoob.com/python/func-number-uniform.html)                        | 随机生成下一个实数，它在[x,y]范围内。                                      

---

* Python三角函数
![](2019-09-07-15678443046835.jpg)
![](2019-09-07-15678443701451.jpg)

Python包括以下三角函数：

函数  | 描述                                    
------- | --------------------------------------
[acos(x)](https://www.runoob.com/python/func-number-acos.html)       | 返回x的反余弦弧度值。                           
[asin(x)](https://www.runoob.com/python/func-number-asin.html)       | 返回x的反正弦弧度值。                           
[atan(x)](https://www.runoob.com/python/func-number-atan.html)       | 返回x的反正切弧度值。                           
[atan2(y, x)](https://www.runoob.com/python/func-number-atan2.html)  | 返回给定的 X 及 Y 坐标值的反正切值。                 
[cos(x)](https://www.runoob.com/python/func-number-cos.html)         | 返回x的弧度的余弦值。                           
[hypot(x, y)](https://www.runoob.com/python/func-number-hypot.html)  | 返回欧几里德范数 sqrt(x*x + y*y)。             
[sin(x)](https://www.runoob.com/python/func-number-sin.html)         | 返回的x弧度的正弦值。                           
[tan(x)](https://www.runoob.com/python/func-number-tan.html)         | 返回x弧度的正切值。                            
[degrees(x)](https://www.runoob.com/python/func-number-degrees.html) | 将弧度转换为角度,如degrees(math.pi/2) ，  返回90.0
[radians(x)](https://www.runoob.com/python/func-number-radians.html) | 将角度转换为弧度                                

* Python数学常量

| 常量 | 描述 |
---------------------------------------------------------------------- | -------------------------------------------------------
| pi  | 数学常量 pi（圆周率，一般以π来表示） |
| e   | 数学常量 e，e即自然常数（自然常数） |

### 1-3 极限
### 1-4 无穷小与无穷大
### 1-5 连续型与偏导数
### 1-6 偏导数
### 1-7 方向导数
### 1-8 梯度

## 第2章 微积分

### 2-1 微积分基本想法
### 2-2 微积分的解释
### 2-3 定积分
### 2-4 定积分性质
### 2-5 牛顿-莱布尼茨公式

## 第3章 泰勒公式与拉格朗日

### 3-1 泰勒公式出发点
### 3-2 一点一世界
### 3-3 阶数的作用
### 3-4 阶乘的作用
### 3-5 拉格朗日乘子法
### 3-6 求解拉格朗日乘子法

## 第4章 线性代数基础

### 4-1 行列式概述
### 4-2 矩阵与数据的关系
### 4-3 矩阵基本操作
### 4-4 矩阵的几种变换
### 4-5 矩阵的秩
### 4-6 内积与正交

## 第5章 特征值与矩阵分解

### 5-1 特征值与特征向量
### 5-2 特征空间与应用
### 5-3 SVD要解决的问题
### 5-4 特征值分解
### 5-5 SVD矩阵分解

## 第6章 随机变量与概率估计

### 6-1 离散型随机变量
### 6-2 连续型随机变量
### 6-3 简单随机抽样
### 6-4 似然函数
### 6-5 极大似然估计

## 第7章 概率论基础

### 7-1 概率与频率
### 7-2 古典概型
### 7-3 条件概率
### 7-4 条件概率小例子
### 7-5 独立性
### 7-6 二维离散随机变量
### 7-7 二维连续型随机变量
### 7-8 边缘分布
### 7-9 期望
### 7-10 期望求解
### 7-11 马尔科夫不等式
### 7-12 切比雪夫不等式
### 7-13 后验概率估计
### 7-14 贝叶斯拼写纠错实例
### 7-15 垃圾邮件过滤实例

## 第8章 数据科学你得知道的几种分布

### 8-1 正太分布
### 8-2 二项式分布
### 8-3 泊松分布
### 8-4 均匀分布
### 8-5 卡方分布
### 8-6 beta分布

## 第9章 核函数变换

### 9-1 核函数的目的
### 9-2 线性核函数
### 9-3 多项式核函数
### 9-4 核函数实例
### 9-5 高斯核函数
### 9-6 参数的影响

## 第10章 熵与激活函数

### 10-1 熵的概念
### 10-2 熵的大小意味着什么
### 10-3 激活函数
### 10-4 激活函数的问题

## 第11章 回归分析

### 11-1 回归分析概述
### 11-2 回归方程定义
### 11-3 误差项的定义
### 11-4 最小二乘法推导与求解
### 11-5 回归方程求解小例子
### 11-6 回归直线拟合优度
### 11-7 多元与曲线回归问题
### 11-8 Python工具包介绍
### 11-9 statsmodels回归分析
### 11-10 高阶与分类变量实例
### 11-11 案例：汽车价格预测任务概述
### 11-12 缺失值填充
### 11-13 特征相关性
### 11-14 预处理问题
### 11-15 回归求解

## 第12章 假设检验

### 12-1 假设检验基本思想
### 12-2 左右侧检验与双侧检验
### 12-3 Z检验基本原理
### 12-4 Z检验实例
### 12-5 T检验基本原理
### 12-6 T检验实例
### 12-7 T检验应用条件
### 12-8 卡方检验
### 12-9 假设检验中的两类错误
### 12-10 Python假设检验实例
### 12-11 Python卡方检验实例

## 第13章 相关分析

### 13-1 相关分析概述
### 13-2 皮尔森相关系数
### 13-3 计算与检验
### 13-4 斯皮尔曼等级相关
### 13-5 肯德尔系数
### 13-6 质量相关分析
### 13-7 偏相关与复相关

## 第14章 方差分析

### 14-1 方差分析概述
### 14-2 方差的比较
### 14-3 方差分析计算方法
### 14-4 方差分析中的多重比较
### 14-5 多因素方差分析
### 14-6 Python方差分析实例

## 第15章 聚类分析

### 15-1 层次聚类概述
### 15-2 层次聚类流程
### 15-3 层次聚类实例
### 15-4 KMEANS算法概述
### 15-5 KMEANS工作流程
### 15-6 KMEANS迭代可视化展示
### 15-7 DBSCAN聚类算法
### 15-8 DBSCAN工作流程
### 15-9 DBSCAN可视化展示

## 第16章 贝叶斯分析

### 16-1 贝叶斯分析概述
### 16-2 概率的解释
### 16-3 贝叶斯学派与经典统计学派的争论
### 16-4 贝叶斯算法概述
### 16-5 贝叶斯推导实例
### 16-6 贝叶斯拼写纠错实例
### 16-7 垃圾邮件过滤实例
### 16-8 贝叶斯解释
### 16-9 经典求解思路
### 16-10 MCMC概述
### 16-11 PYMC3概述
### 16-12 模型诊断
### 16-13 模型决策
### 16-14 作业
