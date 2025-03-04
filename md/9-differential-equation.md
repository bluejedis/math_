# 引言

<ul>

本节内容较少。

若一曲线过点$(1,2)$，且该曲线上任一点$M\,(x,y)$处的切线的斜率为$2x$，求该曲线的方程。

**解：**  
令所求曲线为$\varphi(x)$，则$\dfrac{\mathrm{d}y}{\mathrm{d}x}=2x$，且满足$x=1$时$y=2$。  
两边积分：  
$\int \mathrm{d}y = \int 2x \, \mathrm{d}x$  
$y = x^2 + C$  
代入$(1,2)$：$2 = 1^2 + C$，得$C=1$。  
因此，曲线方程为：$y = x^2 + 1$。

</ul>

# 微分方程基本概念

<ul>

## 微分方程构成

<ul>

**定义：** 表示未知函数、未知函数的导数与自变量之间关系的方程，即含导数的方程，称为**微分方程**。导数可以是一阶或高阶。

**常微分方程：** 未知函数为一元函数的微分方程。例如：  
- $y''' - y'' + 6y = 0$  
- $y \, \mathrm{d}x - (x + \sqrt{x^2 + y^2}) \, \mathrm{d}y = 0$

**定义：** 微分方程中未知函数的最高阶导数的阶数即为该微分方程的**阶**。  
$n$阶微分方程的一般形式为：$F(x, y, y', \cdots, y^{(n)}) = 0$。若能解出最高阶导数，则为：$y^{(n)} = f(x, y, y', \cdots, y^{(n-1)})$。

</ul>

## 微分方程的解

<ul>

微分方程的解是函数。

**定义：** 若解中含有与方程阶数相同的任意常数，则为**通解**。  
例如：$y'' = 3$  
- $y' = 3x + C_1$  
- $y = \frac{3}{2}x^2 + C_1x + C_2$  
含有两个任意常数$C_1$和$C_2$，与二阶相符。

**定义：** 确定通解中的任意常数后，得到**特解**。

**定义：** 给出$x = x_0$时的$y_0$和$y_0'$等值，称为**初值条件**。  
求解$y' = f(x, y)$满足$y|_{x=x_0} = y_0$的特解，构成一阶微分方程的初值问题：  
$$
\begin{cases}
    y' = f(x, y) \\
    y|_{x=x_0} = y_0
\end{cases}
$$

**积分曲线：** 微分方程解的图形为曲线，初值问题即求通过某点的积分曲线。

**例题：** 判断$x = C_1 \cos kt + C_2 \sin kt$是否为$\dfrac{\mathrm{d}^2 x}{\mathrm{d} t^2} + k^2 x = 0$的解，若是，求满足$x|_{t=0} = A$，$\dfrac{\mathrm{d} x}{\mathrm{d} t}|_{t=0} = 0$的特解。  
**解：**  
- 求导：  
  $x' = -k C_1 \sin kt + k C_2 \cos kt$  
  $x'' = -k^2 C_1 \cos kt - k^2 C_2 \sin kt$  
- 代入：  
  $x'' + k^2 x = -k^2 (C_1 \cos kt + C_2 \sin kt) + k^2 (C_1 \cos kt + C_2 \sin kt) = 0$  
  成立，故$x = C_1 \cos kt + C_2 \sin kt$是解。  
- 初值条件：  
  $x(0) = C_1 \cos 0 + C_2 \sin 0 = C_1 = A$  
  $x'(0) = -k C_1 \sin 0 + k C_2 \cos 0 = k C_2 = 0 \Rightarrow C_2 = 0$  
- 特解：$x = A \cos kt$。

</ul>

</ul>

# 可分离变量的微分方程

<ul>

**定义：** 形如$y' = f(x) g(y)$的方程为**变量可分离型**。  
可变形为$\dfrac{\mathrm{d}y}{g(y)} = f(x) \mathrm{d}x$，两边积分得：  
$$
\int \frac{\mathrm{d}y}{g(y)} = \int f(x) \, \mathrm{d}x
$$
解为$G(y) = F(x) + C$，可进一步化为显式解。

**例题：** 求$\dfrac{\mathrm{d}y}{\mathrm{d}x} = 2x y$。  
**解：**  
分离变量：$\dfrac{\mathrm{d}y}{y} = 2x \, \mathrm{d}x$  
积分：$\int \dfrac{\mathrm{d}y}{y} = \int 2x \, \mathrm{d}x$  
$\ln |y| = x^2 + C$  
$y = C_2 e^{x^2}$（$C_2 = \pm e^C$为任意常数）。  
**注意：** 在微分方程中，可直接写$\ln y = x^2 + C$，$C$的正负由$y$的取值决定。

</ul>

# 可化为可分离变量型

<ul>

## 多项式换元

<ul>

形如$\dfrac{\mathrm{d}y}{\mathrm{d}x} = f(ax + by + c)$的方程。  
令$u = ax + by + c$，则$\dfrac{\mathrm{d}u}{\mathrm{d}x} = a + b \dfrac{\mathrm{d}y}{\mathrm{d}x}$，代入得：  
$\dfrac{\mathrm{d}u}{\mathrm{d}x} = a + b f(u)$，可分离变量求解。

</ul>

## 自然齐次方程

<ul>

若方程可化为$\dfrac{\mathrm{d}y}{\mathrm{d}x} = \varphi\left(\dfrac{y}{x}\right)$，则为**齐次方程**。  
令$u = \dfrac{y}{x}$，$y = u x$，则$\dfrac{\mathrm{d}y}{\mathrm{d}x} = u + x \dfrac{\mathrm{d}u}{\mathrm{d}x}$，代入得：  
$x \dfrac{\mathrm{d}u}{\mathrm{d}x} = \varphi(u) - u$  
分离变量：$\dfrac{\mathrm{d}u}{\varphi(u) - u} = \dfrac{\mathrm{d}x}{x}$。

**例题：** 求$y^2 + x^2 \dfrac{\mathrm{d}y}{\mathrm{d}x} = x y \dfrac{\mathrm{d}y}{\mathrm{d}x}$。  
**解：**  
整理得：$\dfrac{\mathrm{d}y}{\mathrm{d}x} = \dfrac{y^2}{x y - x^2} = \dfrac{\left(\dfrac{y}{x}\right)^2}{\dfrac{y}{x} - 1}$  
令$u = \dfrac{y}{x}$，则$\dfrac{\mathrm{d}y}{\mathrm{d}x} = u + x \dfrac{\mathrm{d}u}{\mathrm{d}x}$，代入：  
$u + x \dfrac{\mathrm{d}u}{\mathrm{d}x} = \dfrac{u^2}{u - 1}$  
$x \dfrac{\mathrm{d}u}{\mathrm{d}x} = \dfrac{u^2}{u - 1} - u = \dfrac{u}{u - 1}$  
分离变量：$\dfrac{u - 1}{u} \mathrm{d}u = \dfrac{\mathrm{d}x}{x}$  
积分：$u - \ln |u| = \ln |x| + C$  
代入$u = \dfrac{y}{x}$，得：$\ln |y| = \dfrac{y}{x} + C$，即$y = C e^{\frac{y}{x}}$。

</ul>

## 可化为齐次方程

<ul>

形如$\dfrac{\mathrm{d}y}{\mathrm{d}x} = \dfrac{A_1 x + B_1 y + C_1}{A_2 x + B_2 y + C_2}$的方程。  
令$x = X + h$，$y = Y + k$，使常数项消失：  
$A_1 h + B_1 k + C_1 = 0$  
$A_2 h + B_2 k + C_2 = 0$  
解出$h$和$k$后，方程化为齐次形式。

</ul>

</ul>

# 一阶线性微分方程

<ul>

## 线性方程

<ul>

形如$\dfrac{\mathrm{d}y}{\mathrm{d}x} + P(x) y = Q(x)$为一阶线性方程。  
- 若$Q(x) \equiv 0$，为齐次方程，通解：$y = C e^{-\int P(x) \, \mathrm{d}x}$  
- 若$Q(x) \neq 0$，为非齐次方程，通解：  
  $y = e^{-\int P(x) \, \mathrm{d}x} \left( \int Q(x) e^{\int P(x) \, \mathrm{d}x} \, \mathrm{d}x + C \right)$

**例题：** 求$\dfrac{\mathrm{d}y}{\mathrm{d}x} = \dfrac{1}{x + y}$。  
**解：**  
改写为：$\dfrac{\mathrm{d}x}{\mathrm{d}y} - x = y$，再化为$\dfrac{\mathrm{d}x}{\mathrm{d}y} - x = y$  
$P(y) = -1$，$Q(y) = y$  
通解：$x = e^{\int 1 \, \mathrm{d}y} \left( \int y e^{-\int 1 \, \mathrm{d}y} \, \mathrm{d}y + C \right) = e^y \left( \int y e^{-y} \, \mathrm{d}y + C \right)$  
计算积分后得特解。

</ul>

## 伯努利方程

<ul>

形如$\dfrac{\mathrm{d}y}{\mathrm{d}x} + P(x) y = Q(x) y^n$。  
令$z = y^{1-n}$，化为线性方程求解。

</ul>

</ul>

# 可降阶的高阶微分方程

<ul>

## $y^{(n)} = f(x)$ 型

<ul>

直接对$f(x)$积分$n$次，得通解含$n$个常数。

</ul>

## $y'' = f(x, y')$ 型

<ul>

令$y' = p$，$y'' = \dfrac{\mathrm{d}p}{\mathrm{d}x}$，得$\dfrac{\mathrm{d}p}{\mathrm{d}x} = f(x, p)$，解出$p$后积分得$y$。

**例题：** 求$(1 + x^2) y'' = 2x y'$，满足$y|_{x=0} = 1$，$y'|_{x=0} = 3$。  
**解：**  
令$y' = p$，则$(1 + x^2) \dfrac{\mathrm{d}p}{\mathrm{d}x} = 2x p$  
分离变量：$\dfrac{\mathrm{d}p}{p} = \dfrac{2x}{1 + x^2} \mathrm{d}x$  
积分：$p = C (1 + x^2)$  
初值$y'(0) = 3$，得$p = 3 (1 + x^2)$  
$y = x^3 + 3x + 1$。

</ul>

## $y'' = f(y, y')$ 型

<ul>

令$y' = p$，$y'' = p \dfrac{\mathrm{d}p}{\mathrm{d}y}$，解出$p$后积分得$y$。

</ul>

</ul>

# 高阶线性微分方程

<ul>

## 概念

<ul>

**定义：** $y'' + P(x) y' + Q(x) y = f(x)$ 为二阶变系数线性微分方程。  
- $f(x) \equiv 0$：齐次方程  
- 否则：非齐次方程  
**定义：** $y'' + p y' + q y = f(x)$ 为二阶常系数线性微分方程。

</ul>

## 解的结构

<ul>

- 若$\varphi_1(x)$和$\varphi_2(x)$为齐次方程的解，则$y = C_1 \varphi_1(x) + C_2 \varphi_2(x)$也为解。  
- 若$\varphi_1(x)$和$\varphi_2(x)$分别为齐次和非齐次方程的解，则$y = \varphi_1(x) + \varphi_2(x)$为非齐次解。

</ul>

## 二阶常系数齐次线性微分方程的通解

<ul>

特征方程$\lambda^2 + p \lambda + q = 0$：  
1. $p^2 - 4q > 0$：$y = C_1 e^{\lambda_1 x} + C_2 e^{\lambda_2 x}$  
2. $p^2 - 4q = 0$：$y = (C_1 + C_2 x) e^{\lambda x}$  
3. $p^2 - 4q < 0$：$y = e^{\alpha x} (C_1 \cos \beta x + C_2 \sin \beta x)$

</ul>

## 二阶常系数非齐次线性微分方程的特解

<ul>

通解为齐次通解加特解，特解形式根据$f(x)$确定。

</ul>

</ul>

# 欧拉方程

<ul>

## 概念

<ul>

**定义：** $x^2 y'' + p x y' + q y = f(x)$ 为欧拉方程，$p, q$为常数。

</ul>

## 解法

<ul>

令$x = e^t$，化为常系数方程求解。

**例题：** 求$x^2 \dfrac{\mathrm{d}^2 y}{\mathrm{d} x^2} + 4x \dfrac{\mathrm{d} y}{\mathrm{d} x} + 2y = 0$（$x > 0$）。  
**解：**  
令$x = e^t$，化为$\dfrac{\mathrm{d}^2 y}{\mathrm{d} t^2} + 3 \dfrac{\mathrm{d} y}{\mathrm{d} t} + 2y = 0$  
特征方程：$\lambda^2 + 3\lambda + 2 = 0$，解得$\lambda = -1, -2$  
$y = C_1 e^{-t} + C_2 e^{-2t} = \dfrac{C_1}{x} + \dfrac{C_2}{x^2}$。

</ul>

</ul>