# 一、Typroa下载安装



# 二、Typora常用功能

## 1. 公式编辑

### 1.1 公式添加方式

#### 		① 公式块

​			创建独立的一块公式区域，插入公式块，上部分为公式输入区，下部分为即时显示区，编辑完成后点击其他区域即只剩下显示区内容。

​			例如：
$$
θ_2=t+1
$$
​			创建方式一：菜单栏点击段落，再点击公式块

​			创建方式二：在文中输入$$，再按下回车

#### 		② 行内公式

​			将公式嵌入文字内。

​			例如：插入符号$\theta$。

​			创建方式：在$$的中间加入需要的公式

​								或者先写$再按“esc”键

​			行内公式是需要提前再偏好设置中把内联公式勾选上的。

## 1.2 常用的符号代码

### 	①上下标，正负无穷

| 数学表达式 | LaTex代码 |
| :--------: | :-------: |
|   $x^2$    |    x^2    |
|   $y_1$    |    y_1    |
|  $\infty$  |  \infty   |
| $-\infty$  |  -\infty  |

### 	② 加减乘，分式，根号，省略号

|  数学表达式   |  LaTex代码  |
| :-----------: | :---------: |
|   $a+b-c*d$   |   a+b-c*d   |
|  $a\div{b}$   |  a\div{b}   |
|   $a\pm{b}$   |   a\pm{b}   |
| $\frac{a}{b}$ | \frac{a}{b} |
|  $\sqrt{b}$   |  \sqrt{b}   |
|   $\cdots$    |   \cdots    |

### 	③ 三角函数

|   数学表达式   |  LaTex代码   |
| :------------: | :----------: |
| $\sin{\theta}$ | \sin{\theta} |
| $\cos{\theta}$ | \cos{\theta} |
| $\tan{\theta}$ | \tan{\theta} |
| $\cot{\theta}$ | \cot{\theta} |

### 	④ 矢量，累加累乘，极限

|            数学表达式             |            LaTex代码            |
| :-------------------------------: | :-----------------------------: |
|             $\vec{F}$             |             \vec{F}             |
|       $\sum_{i=1}^{n}{a_i}$       |       \sum_{i=1}^{n}{a_i}       |
|      $\prod_{i=1}^{n}{a_i}$       |      \prod_{i=1}^{n}{a_i}       |
| $\lim_{a\rightarrow+\infty}{a+b}$ | \lim_{a\rightarrow+\infty}{a+b} |

### 	⑤ 希腊字母

|  数学表达式   |  LaTex代码  |
| :-----------: | :---------: |
|   $\alpha$    |   \alpha    |
|    $\beta$    |    \beta    |
|   $\gamma$    |   \gamma    |
|   $\delta$    |   \delta    |
|  $\epsilon$   |  \epsilon   |
| $\varepsilon$ | \varepsilon |
|    $\eta$     |    \eta     |
|   $\theta$    |   \theta    |
|   $\kappa$    |   \kappa    |
|    $\iota$    |    \iota    |
|    $\zeta$    |    \zeta    |
|   $\lambda$   |   \lambda   |
|     $\mu$     |     \mu     |
|    $\phi$     |    \phi     |
|     $\pi$     |     \pi     |
|    $\rho$     |    \rho     |
|     $\xi$     |     \xi     |
|     $\nu$     |     \nu     |
|  $\upsilon$   |  \upsilon   |
|   $\varphi$   |   \varphi   |
|    $\chi$     |    \chi     |
|    $\psi$     |    \psi     |
|   $\omega$    |   \omega    |

​	⑥关系运算符

| 数学表达式 | LaTex代码 |
| :--------: | :-------: |
|   $\leq$   |   \leq    |
|   $\geq$   |   \geq    |

## 1.3 矩阵

### 	①简单矩阵

​	使用`\begin{matrix}…\end{matrix}`生成， 每一行以`\\`结尾表示换行，元素间以`&`间隔，式子的表示序号`\tag{1}`（右边的序号）。
$$
\begin{matrix}
 1 & 2 & 3 \\
 4 & 5 & 6 \\
 7 & 8 & 9 
\end{matrix} \tag{1}
$$

### 	②带括号的矩阵

​	方法一：在`\begin{}`之前和`\end{}`之后添加左右括号的代码。

​	大括号：
$$
\left\{
 \begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix}
  \right\} \tag{2}
$$
​	中括号：
$$
\left[
 \begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix}
  \right] \tag{3}
$$
​	小括号：
$$
 \left(
 \begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix}
  \right) \tag{4}
$$
​	方法二：改变`\begin{matrix}`和`\end{matrix}`中`{matrix}`

​	大括号：
$$
\begin{Bmatrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{Bmatrix} \tag{6}
$$
​	中括号：
$$
\begin{bmatrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{bmatrix} \tag{6}
$$


### 	③包含希腊字母与省略号

​	行省略号`\cdots`，列省略号`\vdots`，斜向省略号（左上至右下）`\ddots`。
$$
\left\{
 \begin{matrix}
 1      & 2        & \cdots & 5        \\
 6      & 7        & \cdots & 10       \\
 \vdots & \vdots   & \ddots & \vdots   \\
 \alpha & \alpha+1 & \cdots & \alpha+4 
 \end{matrix}
 \right\}
$$

## 1.4 公式序号

​	见“矩阵”小节，代码最后的一行即表示右端序号

```text
......
\tag{6}
```

## 1.5 行列式

行列式相关语法与矩阵类似
$$
\begin{vmatrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{vmatrix}
\tag{7}
$$

## 1.6 表格

### 	① 简易表格

$$
\begin{array}{|c|c|c|}
	\hline 2&9&4\\
	\hline 7&5&3\\
	\hline 6&1&8\\
	\hline
\end{array}
$$

​		开头结尾： `\begin{array}` ， `\end{array}`

​		定义式：例：`{|c|c|c|}`，其中`c` `l` `r` 分别代表居中、左对齐及右对齐。

​		分割线：①**竖直分割线**：在定义式中插入 `|`， （`||`表示两条竖直分割线）。

​						②**水平分割线**：在下一行输入前插入 `\hline`，以下图真值表为例。

​		其他：每行元素间均须要插入 `&` ，每行元素以 `\\` 结尾。

### 	② 真值表

$$
\begin{array}{cc|c}
	       A&B&F\\
	\hline 0&0&0\\
	       0&1&1\\
	       1&0&1\\
	       1&1&1\\
\end{array}
$$

## 1.7 多行等式对齐

$$
\begin{aligned}
a &= b + c \\
  &= d + e + f
\end{aligned}
$$

## 1.8 方程式、条件表达式

​		方程组：
$$
\begin{cases}
3x + 5y +  z \\
7x - 2y + 4z \\
-6x + 3y + 2z
\end{cases}
$$
​		同理，条件表达式：
$$
f(n) =
\begin{cases} 
n/2,  & \text{if }n\text{ is even} \\
3n+1, & \text{if }n\text{ is odd}
\end{cases}
$$

## 1.9 间隔（大小空格、紧贴）

​		紧贴 + 无空格 + 小空格 + 中空格 + 大空格 + 真空格 + 双真空格
$$
a\!b + ab + a\,b + a\;b + a\ b + a\quad b + a\qquad b
$$
​		紧贴`\!`

​		无空格 小空格`\,` 中空格`\;` 大空格`\`

​		真空格`\quad` 双真空格`\qquad`

## 1.10 通过Python生成Latex表达式

​		**step1：安装latexify-py模块**

​		**step2：编写代码**

```
import math				//引入数学模块(有些运算的函数需要)
import latexify			//引入latexify模块

@latexify.with_latex	//特定语法，表示之后定义的函数可以转化为LaTeX代码
def f(x,y,z):		    //包含的参数
    pass			   //此处填写可能需要的数学表达式
    return result		//也可以直接体现数学关系

print(f)			   //直接print(函数名)
```

​		**step3：在输出区得到需要的LaTeX数学表达式**

​		特别说明**，生成的表达式为**定义式，即 ，如果只需要等式 ，可以把生成表达式中的`\triangleq`改成`=` ！

参考：

https://zhuanlan.zhihu.com/p/261750408