# 不定积分

<ul>

## 定义

<ul>

设 $f(x)$ 定义在区间 $I$ 上，若存在可导函数 $F(x)$，使得 $F'(x) = f(x)$ 对于任意 $x \in I$ 都成立，则称 $F(x)$ 为 $f(x)$ 在区间 $I$ 上的一个**原函数**。

**定理：** 任意的两个原函数只相差一个常数。

在区间 $I$ 上，函数 $f(x)$ 带有任意常数项的原函数 $F(x) + C$ 称为 $f(x)$ 或 $f(x) \, \text{d}x$ 在该区间上的不定积分，记为 $\int f(x) \, \text{d}x$，其中：

- $\int$ 为**积分号**，
- $f(x)$ 为**被积函数**，
- $f(x) \, \text{d}x$ 为**被积表达式**，
- $x$ 为**积分变量**。

积分是导数的逆运算，即：

$$
\int f(x) \, \text{d}x = F(x) + C, \quad F'(x) = f(x).
$$

</ul>

## 性质

<ul>

### 计算性质

<ul>

积分运算可以将求导的过程逆向进行。隐函数求导法和参数方程求导法可视为复合函数求导法则的变式。积分运算具有以下两个性质：

1. **分项积分法**：

   $$
   \int [f(x) + g(x)] \, \text{d}x = \int f(x) \, \text{d}x + \int g(x) \, \text{d}x.
   $$

2. **常数因子提出**：

   $$
   \int k f(x) \, \text{d}x = k \int f(x) \, \text{d}x \quad (k \neq 0).
   $$

复合函数求导法则的逆运算对应**换元积分法**，函数乘积求导法则的逆运算对应**分部积分法**。

</ul>

### 存在性性质

<ul>

即一元函数的常义可积性（区间有限，函数有界）。

**定理：** 连续函数必有原函数。但反过来，有原函数的函数不一定是连续的，可能存在第二类间断点。

**定理：** 含有第一类间断点或无穷间断点的函数 $f(x)$ 在包含其间断点的区间内必没有原函数 $F(x)$。可以用导数介值定理反证：一个函数的导数不可能导出不可导的点。

若原函数含有震荡间断点，则可能导出导函数。例如：

$$
F(x) = \begin{cases} 
x^2 \sin \frac{1}{x}, & x \neq 0 \\ 
0, & x = 0 
\end{cases}, \quad f(x) = \begin{cases} 
2x \sin \frac{1}{x} - \cos \frac{1}{x}, & x \neq 0 \\ 
0, & x = 0 
\end{cases}.
$$

此函数 $F(x)$ 是连续函数，而 $f(x)$ 在靠近 0 时的极限为：

$$
\lim_{x \to 0} (2x \sin \frac{1}{x} - \cos \frac{1}{x}) = -\lim_{x \to 0} \cos \frac{1}{x},
$$

这是一个振荡间断点。

</ul>

</ul>

## 换元积分法

<ul>

### 第一类换元法（凑微分法）

<ul>

**定理：** 若 $\int f(u) \, \text{d}u = F(u) + C$，则：

$$
\int f[\varphi(x)] \varphi'(x) \, \text{d}x = \int f[\varphi(x)] \, \text{d}\varphi(x) = F[\varphi(x)] + C.
$$

即用中间变量（如 $t$）替换 $x$ 的复杂表达式，使式子更接近基本积分公式。例如：

$$
\int \frac{x}{\sqrt{1 + x^2}} \, \text{d}x = \frac{1}{2} \int \frac{\text{d}(1 + x^2)}{\sqrt{1 + x^2}} = \sqrt{1 + x^2} + C.
$$

凑微分法适用于式子较简单的情况，要求凑出的微分形式符合简单积分公式，且部分表达式可提至微分号后。

**例题：**

1. $$
   \int (1 + 3x)^{100} \, \text{d}x = \frac{1}{3} \int (1 + 3x)^{100} \, \text{d}(1 + 3x) = \frac{1}{303} (1 + 3x)^{101} + C.
   $$

2. $$
   \int \cos^2 x \, \text{d}x = \frac{1}{2} \int (1 + \cos 2x) \, \text{d}x = \frac{1}{2} \left( x + \frac{1}{2} \sin 2x \right) + C.
   $$

3. $$
   \int \cos^3 x \, \text{d}x = \int \cos^2 x \, \text{d} \sin x = \int (1 - \sin^2 x) \, \text{d} \sin x = \sin x - \frac{1}{3} \sin^3 x + C.
   $$

4. $$
   \int \frac{\text{d}x}{x \sqrt{1 + \ln x}} = \int \frac{\text{d}(1 + \ln x)}{\sqrt{1 + \ln x}} = 2 \sqrt{1 + \ln x} + C.
   $$

5. $$
   \int \frac{\text{d}x}{\sqrt{x} (1 + x)} = 2 \int \frac{\text{d} \sqrt{x}}{1 + (\sqrt{x})^2} = 2 \arctan \sqrt{x} + C.
   $$

6. $$
   \int \frac{\arcsin \sqrt{x}}{\sqrt{x (1 - x)}} \, \text{d}x = 2 \int \arcsin \sqrt{x} \, \text{d} \arcsin \sqrt{x} = (\arcsin \sqrt{x})^2 + C.
   $$

7. $$
   \int \frac{\text{d}x}{\sqrt{a^2 - x^2}} = \int \frac{\text{d} \left( \frac{x}{a} \right)}{\sqrt{1 - \left( \frac{x}{a} \right)^2}} = \arcsin \frac{x}{a} + C.
   $$

8. $$
   \int \frac{\text{d}x}{a^2 + x^2} = \int \frac{\text{d} \left( \frac{x}{a} \right)}{1 + \left( \frac{x}{a} \right)^2} = \frac{1}{a} \arctan \frac{x}{a} + C.
   $$

9. $$
   \int \frac{\text{d}x}{x^2 - a^2} = \frac{1}{2a} \ln \left| \frac{x - a}{x + a} \right| + C.
   $$

</ul>

### 第二类换元法

<ul>

**定理：** 设 $x = \varphi(t)$ 为单调可导函数，且 $\varphi'(t) \neq 0$，若：

$$
\int f[\varphi(t) \varphi'(t)] \, \text{d}t = F(t) + C,
$$

则：

$$
\int f(x) \, \text{d}x = F[\varphi^{-1}(x)] + C.
$$

第二类换元法适用于第一类换元法无效的情况，关键在于选择中间变量 $t$，使其使原式接近积分公式，并注意变量取值范围。它是将简单 $x$ 转为复杂 $t$ 表达式，与第一类相反。

**注意：** $\varphi'(t) \neq 0$ 保证函数有反函数，严格单调函数必有反函数，故若 $\varphi(t)$ 严格单调，$\varphi'(t)$ 可为 0。

**例题：** 求 $\int \sqrt{a^2 - x^2} \, \text{d}x \ (a > 0)$。

**解：** 凑微分法需提取部分至微分后符合简单公式，但此式提取 $x$ 后仍复杂，故用第二类换元法。设 $x = a \sin t$，则 $\sqrt{a^2 - x^2} = a \cos t$。考虑 $t$ 取值范围：

- $-a \leq x \leq a$，即 $-1 \leq \sin t \leq 1$，
- $\varphi'(t) = a \cos t \neq 0$，故 $t \in \left[-\frac{\pi}{2}, 0\right) \cup \left(0, \frac{\pi}{2}\right]$，
- 但在 $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$ 上，$\varphi(t) = a \sin t$ 严格单调递增，故 $t \in \left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$。

计算：

$$
\int \sqrt{a^2 - x^2} \, \text{d}x = a^2 \int \cos^2 t \, \text{d}t = \frac{a^2}{2} \left( t + \frac{1}{2} \sin 2t \right) + C = \frac{a^2}{2} \left( \arcsin \frac{x}{a} + \frac{x}{a} \sqrt{1 - \frac{x^2}{a^2}} \right) + C.
$$

**例题：**

1. $\int \frac{\text{d}x}{\sqrt{a^2 + x^2}} \ (a > 0)$，设 $x = a \tan t$：

   $$
   = \int \sec t \, \text{d}t = \ln \left| \sec t + \tan t \right| + C = \ln \left| \sqrt{1 + \frac{x^2}{a^2}} + \frac{x}{a} \right| + C.
   $$

2. $\int \frac{\text{d}x}{\sqrt{x^2 - a^2}} \ (a > 0)$，设 $x = a \sec t$：

   $$
   = \ln \left| \sec t + \tan t \right| + C = \ln \left| \frac{x}{a} + \sqrt{\frac{x^2}{a^2} - 1} \right| + C.
   $$

常用替换方式：
- $\sqrt{a^2 - x^2}$：$x = a \sin t$ 或 $a \cos t$，
- $\sqrt{a^2 + x^2}$：$x = a \tan t$，
- $\sqrt{x^2 - a^2}$：$x = a \sec t$。

换元法适合将式子转为已知积分公式的简单形式。

</ul>

</ul>

## 分部积分法

<ul>

由 $(uv)' = u v' + u' v$，得：

$$
\int u \, \text{d}v = uv - \int v \, \text{d}u.
$$

适用于被积函数可拆为两部分，一部分易积分的情况。

### 基本分部积分

<ul>

**例题：**

1. $$
   \int x e^x \, \text{d}x = x e^x - \int e^x \, \text{d}x = x e^x - e^x + C.
   $$

2. $$
   \int x \sin x \, \text{d}x = \sin x - x \cos x + C.
   $$

3. $$
   \int x \ln x \, \text{d}x = \frac{1}{2} x^2 \ln x - \frac{1}{4} x^2 + C.
   $$

4. $$
   \int x \arctan x \, \text{d}x = \frac{1}{2} \left( x^2 \arctan x - x + \arctan x \right) + C.
   $$

</ul>

### 多次分部积分还原

<ul>

当被积函数含 $\sin x$、$\cos x$、$e^x$ 等积分后变化小的因式时，可多次分部积分，使右侧还原左侧形式。

**例题：**

1. $$
   \int e^x \sin x \, \text{d}x = \frac{e^x \sin x - e^x \cos x}{2} + C.
   $$

2. $$
   \int \sec^3 x \, \text{d}x = \frac{\sec x \tan x + \ln |\sec x + \tan x|}{2} + C.
   $$

常用方式：
- $\int x^n e^x \, \text{d}x$ 等：对 $e^x$ 或三角函数分部，
- $\int x^n \ln x \, \text{d}x$ 等：对 $x^n$ 分部，
- $\int e^x \sin x \, \text{d}x$：对任一部分分部，多次还原。

</ul>

</ul>

## 有理函数的积分

<ul>

有理函数 $\frac{P(x)}{Q(x)}$ 若 $P(x)$ 次数小于 $Q(x)$ 为真分式，否则可分解为多项式加真分式。真分式可拆为部分分式和。例如：

$$
\frac{2x + 3}{(x + 1)(x + 2)(x^2 + 3x + 1)} = -\frac{1}{x + 1} - \frac{1}{x + 2} + \frac{2x + 3}{x^2 + 3x + 1}.
$$

</ul>

</ul>

# 定积分

<ul>

## 定义

<ul>

设 $f(x)$ 在 $[a, b]$ 上连续，将区间分为 $n$ 个子区间，积分和极限定义为：

$$
\int_a^b f(x) \, \text{d}x = \lim_{\lambda \to 0} \sum_{i=1}^n f(\xi_i) \Delta x_i,
$$

若极限存在，则 $f(x)$ 在 $[a, b]$ 上可积。

</ul>

## 性质

<ul>

### 计算性质

<ul>

1. $\int_a^a f(x) \, \text{d}x = 0$，
2. $\int_a^b f(x) \, \text{d}x = -\int_b^a f(x) \, \text{d}x$，
3. $\int_a^b k f(x) \, \text{d}x = k \int_a^b f(x) \, \text{d}x$，
4. $\int_a^b [f(x) \pm g(x)] \, \text{d}x = \int_a^b f(x) \, \text{d}x \pm \int_a^b g(x) \, \text{d}x$，
5. $\int_a^b f(x) \, \text{d}x = \int_a^c f(x) \, \text{d}x + \int_c^b f(x) \, \text{d}x$。

</ul>

### 存在性性质

<ul>

充分条件：
- $f(x)$ 连续、单调或有界且有限间断点时可积。

必要条件：可积函数必有界。

</ul>

</ul>

## 牛顿-莱布尼茨公式

<ul>

**定理：** 若 $F(x)$ 是 $f(x)$ 的原函数，则：

$$
\int_a^b f(x) \, \text{d}x = F(b) - F(a).
$$

</ul>

## 积分法

<ul>

### 换元积分法

<ul>

**定理：** 若 $x = \varphi(t)$ 满足条件，则：

$$
\int_a^b f(x) \, \text{d}x = \int_\alpha^\beta f[\varphi(t)] \varphi'(t) \, \text{d}t.
$$

**例题：** $\int_0^\pi \sqrt{\sin^3 x - \sin^5 x} \, \text{d}x = \frac{4}{5}$.

</ul>

### 分部积分法

<ul>

**定理：**

$$
\int_a^b u \, \text{d}v = [uv]_a^b - \int_a^b v \, \text{d}u.
$$

</ul>

</ul>

</ul>

# 变限积分

<ul>

## 定义

<ul>

$$
\Phi(x) = \int_a^x f(t) \, \text{d}t.
$$

</ul>

## 性质

<ul>

**定理：** 若 $f(x)$ 连续，则：

$$
\left( \int_a^x f(t) \, \text{d}t \right)' = f(x).
$$

</ul>

</ul>

# 反常积分

<ul>

## 无穷区间

<ul>

$$
\int_a^{+\infty} f(x) \, \text{d}x = \lim_{t \to +\infty} \int_a^t f(x) \, \text{d}x.
$$

</ul>

## 无界函数

<ul>

$$
\int_a^b f(x) \, \text{d}x = \lim_{t \to a^+} \int_t^b f(x) \, \text{d}x.
$$

</ul>

</ul>

# 定积分应用

<ul>

## 几何应用

<ul>

### 面积

<ul>

- **直角坐标系**：$S = \int_a^b |y_1(x) - y_2(x)| \, \text{d}x$，
- **参数方程**：$S = \int_\alpha^\beta y(t) x'(t) \, \text{d}t$，
- **极坐标**：$S = \frac{1}{2} \int_\alpha^\beta \rho^2(\theta) \, \text{d}\theta$.

</ul>

### 体积

<ul>

- **旋转体**：$V_x = \pi \int_a^b f^2(x) \, \text{d}x$.

</ul>

</ul>

</ul>

# 积分表

<ul>

| 原函数                   | 积分函数                   | 原函数                   | 积分函数                   |
|--------------------------|----------------------------|--------------------------|----------------------------|
| $\int k \, \text{d}x$   | $kx + C$                  | $\int x^\mu \, \text{d}x$ | $\frac{x^{\mu+1}}{\mu+1} + C$ |
| $\int \frac{\text{d}x}{x}$ | $\ln |x| + C$          | $\int \frac{\text{d}x}{1 + x^2}$ | $\arctan x + C$          |

</ul>