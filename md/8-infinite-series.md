# 常数项级数

<ul>

## 概念

<ul>

级数的经典悖论为**芝诺悖论**。

### 基本概念

<ul>

<span style="color: violet;">**定义：**</span>给定一个无穷数列 $u_1, u_2, \cdots, u_n, \cdots$，将其各项用加号连接起来得到的记号 $\sum_{n=1}^\infty u_n$，即：

$$
\sum_{n=1}^\infty u_n = u_1 + u_2 + \cdots + u_n + \cdots
$$

称为**无穷级数**，简称**级数**，其中 $u_n$ 称为该级数的**通项**。

若 $u_n$ 是常数而不是函数，则 $\sum_{n=1}^\infty u_n$ 被称为**常数项无穷级数**，简称**常数项级数**。

$S_n = u_1 + u_2 + \cdots + u_n$ 称为级数的**部分和**，$\{S_n\}$ 是级数的**部分和数列**。

<span style="color: violet;">**定义：**</span>若 $\lim_{n \to \infty} S_n = S$，则 $\sum_{n=1}^\infty u_n$ **收敛**，并称 $S$ 为该收敛级数 $\sum_{n=1}^\infty u_n$ 的**和**；若 $\lim_{n \to \infty} S_n$ 不存在或为 $\pm \infty$，则 $\sum_{n=1}^\infty u_n$ **发散**。

研究 $\sum_{n=1}^\infty u_n$ 是收敛还是发散，就是研究级数 $\sum_{n=1}^\infty u_n$ 的**敛散性**。

在级数 $\sum_{n=1}^\infty u_n$ 中去掉前 $m$ 项，得到 $\sum_{n=m+1}^\infty u_n = u_{m+1} + u_{m+2} + \cdots$，称为级数 $\sum_{n=1}^\infty u_n$ 的 **$m$ 项后余项**。

</ul>

### 性质

<ul>

1. **线性性质**：若级数 $\sum_{n=1}^\infty u_n$ 和 $\sum_{n=1}^\infty v_n$ 均收敛，且其和分别为 $S$ 和 $T$，则对于任意常数 $a, b$，级数 $\sum_{n=1}^\infty (a u_n + b v_n)$ 也收敛，且其和为 $aS + bT$，即：

   $$
   \sum_{n=1}^\infty (a u_n + b v_n) = a \sum_{n=1}^\infty u_n + b \sum_{n=1}^\infty v_n
   $$

   （收敛 ± 发散 = 发散，发散 ± 发散 = 不确定）

2. 若级数 $\sum_{n=1}^\infty u_n$ 收敛，则其任意 $m$ 项后余项 $\sum_{n=m+1}^\infty u_n$ 也收敛；若存在某个 $m$ 项后余项 $\sum_{n=m+1}^\infty u_n$ 收敛，则 $\sum_{n=1}^\infty u_n$ 也收敛。

3. 对收敛级数加括号后仍然收敛，但加括号后收敛的级数，原级数不一定收敛。若原级数加括号后发散，则原级数一定发散。

4. **级数收敛的必要条件**：若级数 $\sum_{n=1}^\infty u_n$ 收敛，则 $\lim_{n \to \infty} u_n = 0$。

**证明性质 4**：

$$
u_n = S_n - S_{n-1}
$$

$$
\lim_{n \to \infty} u_n = \lim_{n \to \infty} (S_n - S_{n-1}) = \lim_{n \to \infty} S_n - \lim_{n \to \infty} S_{n-1} = S - S = 0
$$

但极限为 0 不一定意味着级数收敛。

</ul>

</ul>

## 级数敛散性判别

<ul>

### 正项级数

<ul>

#### 正项级数概念

<ul>

<span style="color: violet;">**定义：**</span>若通项 $u_n \geqslant 0$，$n = 1, 2, \cdots$，则 $\sum_{n=1}^\infty u_n$ 为**正项级数**。

正项级数的部分和一定是递增的，根据数列极限的**单调有界准则**，若部分和有上界，则极限存在，即级数收敛。

</ul>

#### 收敛原则

<ul>

<span style="color: aqua;">**定理：**</span>正项级数 $\sum_{n=1}^\infty u_n$ 收敛的充要条件是其部分和数列 $\{S_n\}$ 有界。（某一函数在固定区间内变化率有界，则变化范围有界）

**证明**：

- **必要性**：由于 $u_n \geqslant 0$，因此 $S_n = u_1 + u_2 + \cdots + u_n \geqslant 0$，且 $S_1 \leqslant S_2 \leqslant \cdots \leqslant S_n \leqslant \cdots$，$\{S_n\}$ 单调不减且下界为 0。当 $\sum_{n=1}^\infty u_n$ 收敛时，$\lim_{n \to \infty} S_n$ 存在，则 $\{S_n\}$ 必有上界。结合下界，$\{S_n\}$ 有界。

- **充分性**：由于 $\{S_n\}$ 单调不减，若 $\{S_n\}$ 有界，则根据单调有界准则，$\{S_n\}$ 收敛，即 $\lim_{n \to \infty} S_n$ 存在，因此 $\sum_{n=1}^\infty u_n$ 收敛。

通常使用**放缩法**判断 $\{S_n\}$ 是否有界。

**例题**：判断级数 $\sum_{n=1}^\infty \dfrac{1}{\sqrt{n}}$ 的敛散性。

**解**：

$$
S_n = 1 + \dfrac{1}{\sqrt{2}} + \dfrac{1}{\sqrt{3}} + \cdots + \dfrac{1}{\sqrt{n}} > n \cdot \dfrac{1}{\sqrt{n}} = \sqrt{n}
$$

当 $n \to \infty$ 时，$\sqrt{n} \to \infty$，故 $S_n$ 无上界，因此级数发散。

由于收敛原则使用不便，下面介绍几种更实用的判别方法。

</ul>

#### 比较判别法

<ul>

<span style="color: aqua;">**定理：**</span>给出两个正项级数 $\sum_{n=1}^\infty u_n$ 和 $\sum_{n=1}^\infty v_n$，若从某项开始有 $u_n \leqslant v_n$ 成立，则：

1. 若 $\sum_{n=1}^\infty v_n$ 收敛，则 $\sum_{n=1}^\infty u_n$ 也收敛；
2. 若 $\sum_{n=1}^\infty u_n$ 发散，则 $\sum_{n=1}^\infty v_n$ 也发散。

即：大的收敛，小的也收敛；小的发散，大的也发散。

**例题**：判断调和级数 $\sum_{n=1}^\infty \dfrac{1}{n}$ 的敛散性。

**解**：

由于 $x > 0$ 时，$x > \ln(1 + x)$，因此：

$$
\dfrac{1}{n} > \ln\left(1 + \dfrac{1}{n}\right)
$$

又：

$$
\ln\left(1 + \dfrac{1}{n}\right) = \ln \dfrac{n+1}{n} = \ln(n+1) - \ln n
$$

则：

$$
S_n = \ln \dfrac{2}{1} + \ln \dfrac{3}{2} + \cdots + \ln \dfrac{n+1}{n} = \ln 2 - \ln 1 + \ln 3 - \ln 2 + \cdots + \ln(n+1) - \ln n = \ln(n+1)
$$

当 $n \to \infty$ 时，$\ln(n+1) \to \infty$，故 $\sum_{n=1}^\infty \ln\left(1 + \dfrac{1}{n}\right)$ 发散。因此，由比较判别法，$\sum_{n=1}^\infty \dfrac{1}{n}$ 也发散。

</ul>

#### 比较判别法极限性质

<ul>

这是比较判别法的推论，利用极限的阶数进行比较。

给出两个正项级数 $\sum_{n=1}^\infty u_n$ 和 $\sum_{n=1}^\infty v_n$，$v_n \neq 0$，且 $\lim_{n \to \infty} \dfrac{u_n}{v_n} = A$：

1. 若 $A = 0$，当 $\sum_{n=1}^\infty v_n$ 收敛时，$\sum_{n=1}^\infty u_n$ 也收敛；
2. 若 $A = +\infty$，当 $\sum_{n=1}^\infty v_n$ 发散时，$\sum_{n=1}^\infty u_n$ 也发散；
3. 若 $0 < A < +\infty$，则 $\sum_{n=1}^\infty v_n$ 与 $\sum_{n=1}^\infty u_n$ 具有相同敛散性。

**例题**：判断 $\sum_{n=1}^\infty \left( \dfrac{1}{n} - \sin \dfrac{1}{n} \right)$ 的敛散性。

**解**：

令 $x = \dfrac{1}{n}$，当 $n \to \infty$ 时，$x \to 0^+$。当 $x \to 0^+$ 时，泰勒展开得：

$$
x - \sin x \sim \dfrac{1}{6} x^3
$$

因此：

$$
\lim_{n \to \infty} \dfrac{ \dfrac{1}{n} - \sin \dfrac{1}{n} }{ \dfrac{1}{n^3} } = \dfrac{1}{6} \neq 0
$$

由于 $\dfrac{1}{6}$ 为有限正数，$\dfrac{1}{n} - \sin \dfrac{1}{n}$ 与 $\dfrac{1}{n^3}$ 具有相同敛散性。根据 $p$ 级数定理，$\sum_{n=1}^\infty \dfrac{1}{n^3}$ 当 $p = 3 > 1$ 时收敛，故 $\sum_{n=1}^\infty \left( \dfrac{1}{n} - \sin \dfrac{1}{n} \right)$ 收敛。

</ul>

#### 比值判别法

<ul>

也称为**达朗贝尔判别法**。由等比级数的性质推导，级数的敛散性只与通项的比值有关。

<span style="color: aqua;">**定理：**</span>给出一个正项级数 $\sum_{n=1}^\infty u_n$，若 $\lim_{n \to \infty} \dfrac{u_{n+1}}{u_n} = \rho$，则：

1. 若 $\rho < 1$，则 $\sum_{n=1}^\infty u_n$ 收敛；
2. 若 $\rho > 1$，则 $\sum_{n=1}^\infty u_n$ 发散。

<span style="color: orange;">**注意**：</span>当 $\rho = 1$ 时，无法判断敛散性。例如，$\sum_{n=1}^\infty \dfrac{1}{n}$ 发散，而 $\sum_{n=1}^\infty \dfrac{1}{n^2}$ 收敛。

**例题**：判断级数 $\sum_{n=1}^\infty \dfrac{|a|^n n!}{n^n}$ 的敛散性，其中 $a$ 为非零常数。

**解**：

记 $u_n = \dfrac{|a|^n n!}{n^n}$，则：

$$
\dfrac{u_{n+1}}{u_n} = \dfrac{ |a|^{n+1} (n+1)! }{ (n+1)^{n+1} } \cdot \dfrac{ n^n }{ |a|^n n! } = |a| \cdot \dfrac{n+1}{n+1} \cdot \dfrac{n^n}{(n+1)^n} = |a| \left( \dfrac{n}{n+1} \right)^n
$$

$$
\lim_{n \to \infty} \dfrac{u_{n+1}}{u_n} = |a| \lim_{n \to \infty} \left( \dfrac{n}{n+1} \right)^n = |a| e^{\lim_{n \to \infty} n \ln \dfrac{n}{n+1}} = |a| e^{\lim_{n \to \infty} n (\dfrac{n}{n+1} - 1)} = |a| e^{\lim_{n \to \infty} \dfrac{-n}{n+1}} = |a| e^{-1} = \dfrac{|a|}{e}
$$

- 若 $0 < |a| < e$，则 $\dfrac{|a|}{e} < 1$，级数收敛；
- 若 $|a| > e$，则 $\dfrac{|a|}{e} > 1$，级数发散；
- 若 $|a| = e$，则 $\dfrac{|a|}{e} = 1$，需进一步分析。回代得 $\dfrac{u_{n+1}}{u_n} = e \left( \dfrac{n}{n+1} \right)^n \to 1^+$，且 $u_n > u_1 = e > 0$，故发散。

</ul>

#### 根值判别法

<ul>

也称为**柯西判别法**，由比值判别法类比而来。

<span style="color: aqua;">**定理：**</span>给出正项级数 $\sum_{n=1}^\infty u_n$，若 $\lim_{n \to \infty} \sqrt[n]{u_n} = \rho$，则：

1. 若 $\rho < 1$，则 $\sum_{n=1}^\infty u_n$ 收敛；
2. 若 $\rho > 1$，则 $\sum_{n=1}^\infty u_n$ 发散。

同样，当 $\rho = 1$ 时判别法失效。

**例题**：判断级数 $\sum_{n=1}^\infty \left( n \sin \dfrac{1}{n} \right)^{n^3}$ 的敛散性。

**解**：

记 $u_n = \left( n \sin \dfrac{1}{n} \right)^{n^3}$，则：

$$
\sqrt[n]{u_n} = \left( n \sin \dfrac{1}{n} \right)^{n^2}
$$

令 $t = \dfrac{1}{n}$，当 $n \to \infty$ 时，$t \to 0^+$，则：

$$
n \sin \dfrac{1}{n} = \dfrac{\sin t}{t}
$$

因为 $\sin t \sim t - \dfrac{t^3}{6}$，所以：

$$
\dfrac{\sin t}{t} \sim 1 - \dfrac{t^2}{6}
$$

$$
\sqrt[n]{u_n} = \left( \dfrac{\sin t}{t} \right)^{n^2} = e^{n^2 \ln \left( \dfrac{\sin t}{t} \right)} \sim e^{n^2 \ln \left( 1 - \dfrac{t^2}{6} \right)} \sim e^{n^2 \left( -\dfrac{t^2}{6} \right)} = e^{-\dfrac{n^2}{6 n^2}} = e^{-\dfrac{1}{6}}
$$

因此：

$$
\lim_{n \to \infty} \sqrt[n]{u_n} = e^{-\dfrac{1}{6}} < 1
$$

由根值判别法，级数收敛。

</ul>

#### 积分判别法

<ul>

<span style="color: aqua;">**定理：**</span>设 $f(x)$ 是 $[1, +\infty)$ 上单调递减且非负的连续函数，$a_n = f(n)$，则 $\sum_{n=1}^\infty a_n$ 与 $\int_1^{+\infty} f(x) \, dx$ 同敛散。

**例题**：证明 $p$ 级数 $\sum_{n=1}^\infty \dfrac{1}{n^p}$ 当 $p > 1$ 时的敛散性。

**证明**：

令 $f(x) = \dfrac{1}{x^p}$，则：

$$
\int_1^{+\infty} \dfrac{1}{x^p} \, dx = \lim_{b \to \infty} \int_1^b x^{-p} \, dx = \lim_{b \to \infty} \left[ \dfrac{x^{1-p}}{1-p} \right]_1^b = \lim_{b \to \infty} \left( \dfrac{b^{1-p}}{1-p} - \dfrac{1}{1-p} \right)
$$

- 当 $p > 1$ 时，$1 - p < 0$，$b^{1-p} \to 0$，积分收敛；
- 当 $p \leqslant 1$ 时，积分发散。

因此，$\sum_{n=1}^\infty \dfrac{1}{n^p}$ 当 $p > 1$ 时收敛，否则发散。

</ul>

</ul>

### 交错级数

<ul>

#### 交错级数概念

<ul>

<span style="color: violet;">**定义：**</span>若级数各项**正负相间**出现，则称为**交错级数**，一般写为：

$$
\sum_{n=1}^\infty (-1)^{n-1} u_n = u_1 - u_2 + u_3 - u_4 + \cdots + (-1)^{n-1} u_n + \cdots
$$

其中 $u_n > 0$。

</ul>

#### 莱布尼兹判别法

<ul>

<span style="color: violet;">**定义：**</span>对于交错级数 $\sum_{n=1}^\infty (-1)^{n-1} u_n$，$u_n > 0$，$n = 1, 2, \cdots$，若 $\{u_n\}$ **单调不增**（即 $u_n \geqslant u_{n+1}$）且 $\lim_{n \to \infty} u_n = 0$，则该级数收敛。反之不一定成立。

例如，$\sum_{n=1}^\infty \dfrac{(-1)^{n-1}}{2^{n + (-1)^n}}$ 收敛，但 $u_n$ 不单调递减。

**例题 1**：判断交错调和级数 $\sum_{n=1}^\infty (-1)^{n-1} \dfrac{1}{n}$ 的敛散性。

**解**：

- $\lim_{n \to \infty} u_n = \lim_{n \to \infty} \dfrac{1}{n} = 0$
- $\dfrac{1}{n} > \dfrac{1}{n+1}$，单调递减

由莱布尼兹判别法，级数收敛。

**例题 2**：判断级数 $\sum_{n=1}^\infty \sin (\pi \sqrt{n^2 + a^2})$ 的敛散性，其中 $a$ 为非零常数。

**解**：

利用 $\sin (\alpha + n\pi) = (-1)^n \sin \alpha$，设 $t = \dfrac{1}{n}$：

$$
\pi \sqrt{n^2 + a^2} = \pi n \sqrt{1 + \dfrac{a^2}{n^2}} \sim \pi n + \dfrac{\pi a^2}{2n}
$$

$$
\sin (\pi \sqrt{n^2 + a^2}) \sim (-1)^n \sin \left( \dfrac{\pi a^2}{2n} \right)
$$

令 $u_n = \sin \left( \dfrac{\pi a^2}{2n} \right)$，则：

- $\lim_{n \to \infty} u_n \to 0$
- $u_n$ 随 $n$ 增大而减小（因为 $\dfrac{\pi a^2}{2n}$ 减小，且 $\sin x$ 在 $[0, \pi/2)$ 上单调递增）

由莱布尼兹判别法，级数收敛。

**例题 3**：判断级数 $\sum_{n=1}^\infty (-1)^n \dfrac{\ln (1 + n)}{1 + n}$ 的敛散性。

**解**：

- $\lim_{n \to \infty} u_n = \lim_{n \to \infty} \dfrac{\ln (1 + n)}{1 + n} = \lim_{x \to +\infty} \dfrac{\ln (1 + x)}{1 + x} = \lim_{x \to +\infty} \dfrac{1/(1+x)}{1} = 0$

- 令 $f(x) = \dfrac{\ln (1 + x)}{1 + x}$，求导：

  $$
  f'(x) = \dfrac{\dfrac{1}{1+x} - \dfrac{\ln (1 + x)}{(1 + x)^2}}{1} = \dfrac{1 - \ln (1 + x)}{(1 + x)^2}
  $$

  当 $x$ 足够大时，$\ln (1 + x) > 1$，$f'(x) < 0$，故 $f(x)$ 单调递减。

由莱布尼兹判别法，级数收敛。

</ul>

</ul>

### 任意项级数

<ul>

#### 任意项级数概念

<ul>

<span style="color: violet;">**定义：**</span>若级数 $\sum_{n=1}^\infty (-1)^{n-1} u_n$ 的各项可正可负，也可为零，则称为**任意项级数**。

对其每项取绝对值，得到 $\sum_{n=1}^\infty (-1)^{n-1} |u_n|$，这是一个正项级数，称为原级数的**绝对值级数**。

取绝对值会提高发散性，因为它不改变通项趋于 0 的速度，但阻止了正负项的抵消。

</ul>

#### 绝对收敛

<ul>

<span style="color: violet;">**定义：**</span>设 $\sum_{n=1}^\infty (-1)^{n-1} u_n$ 为任意项级数，若 $\sum_{n=1}^\infty (-1)^{n-1} |u_n|$ 收敛，则称 $\sum_{n=1}^\infty (-1)^{n-1} u_n$ **绝对收敛**。

</ul>

#### 条件收敛

<ul>

<span style="color: violet;">**定义：**</span>设 $\sum_{n=1}^\infty (-1)^{n-1} u_n$ 为任意项级数，若 $\sum_{n=1}^\infty (-1)^{n-1} u_n$ 收敛，但 $\sum_{n=1}^\infty (-1)^{n-1} |u_n|$ 发散，则称 $\sum_{n=1}^\infty (-1)^{n-1} u_n$ **条件收敛**。

<span style="color: aqua;">**定理：**</span>若 $\sum_{n=1}^\infty (-1)^{n-1} |u_n|$ 收敛，则 $\sum_{n=1}^\infty (-1)^{n-1} u_n$ 必收敛。（绝对收敛必收敛）

<span style="color: aqua;">**定理：**</span>收敛级数的项任意加括号后所得新级数仍收敛，且和不变。

<span style="color: aqua;">**定理：**</span>若原级数绝对收敛，无论如何排列其项，新级数仍收敛，且和不变。（绝对收敛具有可交换性）

<span style="color: aqua;">**定理：**</span>条件收敛级数的所有正项（或负项）构成的级数一定发散。

<span style="color: aqua;">**定理：**</span>若 $\sum_{n=1}^\infty |a_n|$ 收敛，则 $\sum_{n=1}^\infty a_n^2$ 收敛。

**例题**：若级数 $\sum_{n=1}^\infty u_n$ 收敛，则下列级数中必收敛的是：

A. $\sum_{n=1}^\infty (-1) \dfrac{u_n}{n}$  
B. $\sum_{n=1}^\infty u_n^2$  
C. $\sum_{n=1}^\infty (u_{2n-1} - u_{2n})$  
D. $\sum_{n=1}^\infty (u_n + u_{n+1})$

**解**：

- **A**：取 $u_n = \dfrac{(-1)^n}{n}$，则 $\sum u_n$ 收敛（交错调和级数），但 $\sum (-1) \dfrac{u_n}{n} = \sum (-1)^{n+1} \dfrac{1}{n^2}$ 收敛。取 $u_n = \dfrac{(-1)^n}{\ln n}$，则 $\sum (-1) \dfrac{u_n}{n} = \sum (-1)^{n+1} \dfrac{1}{n \ln n}$ 仍收敛（莱布尼兹判别法）。但一般情况下，A 不一定必收敛。

- **B**：取 $u_n = \dfrac{(-1)^n}{\sqrt{n}}$，则 $\sum u_n$ 收敛，但 $\sum u_n^2 = \sum \dfrac{1}{n}$ 发散。不必收敛。

- **C**：取 $u_n = \dfrac{(-1)^{n-1}}{n}$，则 $u_{2n-1} - u_{2n} = \dfrac{1}{2n-1} - \dfrac{1}{2n}$，$\sum (u_{2n-1} - u_{2n})$ 发散。不必收敛。

- **D**：若 $\sum u_n$ 收敛，则 $\sum_{n=1}^\infty (u_n + u_{n+1}) = \sum u_n + \sum u_{n+1} = 2 \sum u_n - u_1$，必收敛。

**答案**：D

<span style="color: aqua;">**定理：**</span>广义 $p$ 级数：

$$
\sum_{n=2}^\infty \dfrac{1}{n (\ln n)^p} \begin{cases} 
\text{收敛}, & p > 1 \\ 
\text{发散}, & p \leqslant 1 
\end{cases}
$$

（$n=1$ 无意义，从 $n=2$ 开始不影响敛散性）

<span style="color: aqua;">**定理：**</span>若 $\sum u_n^2$ 收敛，则 $\sum \dfrac{u_n}{n}$ 绝对收敛。

**证明**：

由不等式 $|a||b| \leqslant \dfrac{|a|^2 + |b|^2}{2}$，得：

$$
0 \leqslant \left| \dfrac{u_n}{n} \right| \leqslant \dfrac{u_n^2 + \dfrac{1}{n^2}}{2}
$$

若 $\sum u_n^2$ 收敛，则 $\sum \dfrac{1}{n^2}$ 收敛，故 $\sum \dfrac{u_n^2 + \dfrac{1}{n^2}}{2}$ 收敛，由比较判别法，$\sum \left| \dfrac{u_n}{n} \right|$ 收敛。

</ul>

</ul>

</ul>

</ul>

---

# 幂级数

<ul>

## 幂级数概念

<ul>

### 幂级数定义

<ul>

<span style="color: violet;">**定义：**</span>设函数列 $\{u_n(x)\}$ 定义在区间 $I$ 上，称：

$$
u_1(x) + u_2(x) + \cdots + u_n(x) + \cdots
$$

为定义在 $I$ 上的**函数项级数**，记为 $\sum_{n=1}^\infty u_n(x)$。当 $x$ 取确定值 $x_0$ 时，$\sum_{n=1}^\infty u_n(x_0)$ 成为常数项级数。

<span style="color: violet;">**定义：**</span>若 $\sum_{n=1}^\infty u_n(x)$ 的通项 $u_n(x)$ 为 $n$ 次幂函数，则称其为**幂级数**，一般形式为：

$$
\sum_{n=0}^\infty a_n (x - x_0)^n = a_0 + a_1 (x - x_0) + a_2 (x - x_0)^2 + \cdots + a_n (x - x_0)^n + \cdots
$$

标准形式为：

$$
\sum_{n=0}^\infty a_n x^n = a_0 + a_1 x + a_2 x^2 + \cdots + a_n x^n + \cdots
$$

其中 $a_n$（$n = 0, 1, 2, \cdots$）为**幂级数的系数**。幂级数也称为**泰勒级数**，与泰勒展开式结构相同。

<span style="color: violet;">**定义：**</span>若 $x_0 \in I$，且 $\sum_{n=1}^\infty u_n(x_0)$ 收敛，则 $x_0$ 为**收敛点**；若发散，则为**发散点**。

</ul>

### 阿贝尔定理

<ul>

<span style="color: violet;">**定义：**</span>当幂级数 $\sum_{n=0}^\infty a_n x^n$ 在 $x = x_1$（$x_1 \neq 0$）处收敛时，对于所有满足 $|x| < |x_1|$ 的 $x$，幂级数**绝对收敛**；当在 $x = x_2$（$x_2 \neq 0$）处发散时，对于所有 $|x| > |x_2|$ 的 $x$，幂级数**发散**。

因此，存在一个 $R$，使得 $|x| < R$ 时绝对收敛，$|x| > R$ 时发散，$R$ 称为**收敛半径**。对于 $x = \pm R$，需代入判断敛散性。

</ul>

### 收敛域

<ul>

<span style="color: violet;">**定义：**</span>函数项级数 $\sum_{n=1}^\infty u_n(x)$ 的所有收敛点的集合称为其**收敛域**。

#### 具体型

<ul>

**收敛域求法**：

1. 若 $\lim_{n \to \infty} \left| \dfrac{a_{n+1}}{a_n} \right|$ 或 $\lim_{n \to \infty} \sqrt[n]{|a_n|} = \rho$，则：

   $$
   R = \begin{cases} 
   \dfrac{1}{\rho}, & \rho \neq 0 \\ 
   +\infty, & \rho = 0 \\ 
   0, & \rho = +\infty 
   \end{cases}
   $$

2. 开区间 $(-R, R)$ 为收敛区间。

3. 代入 $x = \pm R$ 判断敛散性，组合得到收敛域。

若只知 $a_n$ 与 $a_{n+2}$ 的关系，则此方法不便。

**统一求法**：

1. 取绝对值 $|u_n(x)| \geqslant 0$，使用正项级数判别法。
2. 求 $\lim_{n \to \infty} \dfrac{|u_{n+1}(x)|}{|u_n(x)|} = \rho$ 或 $\lim_{n \to \infty} \sqrt[n]{|u_n(x)|} = \rho$，令 $\rho < 1$，得收敛区间 $x \in (a, b)$。
3. 单独讨论 $x = a$ 和 $x = b$ 的敛散性，得出收敛域。

<span style="color: aqua;">**定理：**</span>若幂级数 $\sum_{n=0}^\infty a_n x^n$ 在 $x = x_0$ 处条件收敛，则 $x_0$ 是收敛区间的端点。

**例题**：求幂级数 $\sum_{n=1}^\infty \dfrac{x^n}{n}$ 的收敛域。

**解**：

令 $|u_n(x)| = \left| \dfrac{x^n}{n} \right|$，使用比值判别法：

$$
\lim_{n \to \infty} \dfrac{|u_{n+1}(x)|}{|u_n(x)|} = \lim_{n \to \infty} \dfrac{ |x|^{n+1} / (n+1) }{ |x|^n / n } = |x| \cdot \dfrac{n}{n+1} = |x|
$$

令 $|x| < 1$，得 $-1 < x < 1$。

- 当 $x = -1$ 时，$\sum_{n=1}^\infty \dfrac{(-1)^n}{n}$ 收敛（交错调和级数）。
- 当 $x = 1$ 时，$\sum_{n=1}^\infty \dfrac{1}{n}$ 发散。

故收敛域为 $[-1, 1)$。

</ul>

#### 抽象型

<ul>

<span style="color: aqua;">**定理：**</span>根据阿贝尔定理，已知 $\sum_{n=0}^\infty a_n (x - x_0)^n$ 在某点 $x_1$（$x_1 \neq x_0$）的敛散性，可分为三种情况：

1. 若在 $x_1$ 处收敛，则 $R \geqslant |x_1 - x_0|$；
2. 若在 $x_1$ 处发散，则 $R \leqslant |x_1 - x_0|$；
3. <span style="color: orange;">**注意**：</span>若在 $x_1$ 处条件收敛，则 $R = |x_1 - x_0|$。

<span style="color: aqua;">**定理：**</span>已知 $\sum a_n (x - x_1)^n$ 的敛散性，讨论 $\sum b_n (x - x_2)^m$ 的敛散性：

1. $(x - x_1)^n$ 与 $(x - x_2)^m$ 通过初等变形转换：
   - 平移收敛区间；
   - 提出或乘以 $(x - x_0)^k$。
2. $a_n$ 与 $b_n$ 通过微积分变形转换：
   - 逐项求导；
   - 逐项积分。
3. 以下情况收敛半径不变，收敛域需具体讨论：
   - 提出或乘以 $(x - x_0)^k$ 或平移，半径不变；
   - 逐项求导，半径不变，收敛域可能缩小；
   - 逐项积分，半径不变，收敛域可能扩大。

**例题**：设 $\sum_{n=1}^\infty a_n (x + 1)^n$ 在 $x = 1$ 处条件收敛，则 $\sum_{n=1}^\infty n a_n (x - 1)^n$ 在 $x = 2$ 处的敛散性为：

A. 绝对收敛  
B. 条件收敛  
C. 发散  
D. 敛散性不确定

**解**：

- $\sum_{n=1}^\infty a_n (x + 1)^n = \sum_{n=1}^\infty a_n (x - (-1))^n$，中心为 $x_0 = -1$。
- 在 $x = 1$ 处条件收敛，$R = |1 - (-1)| = 2$，收敛区间为 $(-3, 1]$。
- 对于 $\sum_{n=1}^\infty n a_n (x - 1)^n$，由 $\limsup_{n \to \infty} \sqrt[n]{|a_n|} = \dfrac{1}{2}$，则 $\limsup_{n \to \infty} \sqrt[n]{|n a_n|} \sim \dfrac{1}{2}$，故 $R = 2$，收敛区间为 $(-1, 3)$。
- $x = 2$ 在 $(-1, 3)$ 内，绝对收敛。

**答案**：A

</ul>

</ul>

</ul>

## 函数展开为幂级数

<ul>

### 函数展开概念

<ul>

<span style="color: violet;">**定义：**</span>若函数 $f(x)$ 在 $x = x_0$ 处存在任意阶导数，则：

$$
f(x_0) + f'(x_0)(x - x_0) + \dfrac{f''(x_0)}{2!} (x - x_0)^2 + \cdots + \dfrac{f^{(n)}(x_0)}{n!} (x - x_0)^n + \cdots
$$

称为 $f(x)$ 在 $x_0$ 处的**泰勒级数**，若收敛，则：

$$
f(x) = \sum_{n=0}^\infty \dfrac{f^{(n)}(x_0)}{n!} (x - x_0)^n
$$

当 $x_0 = 0$ 时，称为**麦克劳林级数**：

$$
f(x) = \sum_{n=0}^\infty \dfrac{f^{(n)}(0)}{n!} x^n
$$

<span style="color: aqua;">**定理：**</span>若 $f(x)$ 在 $x = x_0$ 处任意阶可导，则 $\sum_{n=0}^\infty \dfrac{f^{(n)}(x_0)}{n!} (x - x_0)^n$ 在 $(x_0 - R, x_0 + R)$ 上收敛于 $f(x)$ 等价于 $\lim_{n \to \infty} R_n(x) = 0$，其中余项：

$$
R_n(x) = \dfrac{f^{(n+1)}(\xi)}{(n+1)!} (x - x_0)^{n+1}
$$

</ul>

### 重要展开式

<ul>

$x$ 的取值是幂级数收敛域与定义域的交集。第 7 个展开式的收敛区间与 $\alpha$ 有关。

1. $e^x = \sum_{n=0}^\infty \dfrac{x^n}{n!} = 1 + x + \dfrac{x^2}{2!} + \dfrac{x^3}{3!} + \cdots$，$-\infty < x < +\infty$
2. $\dfrac{1}{1 + x} = \sum_{n=0}^\infty (-1)^n x^n = 1 - x + x^2 - x^3 + \cdots$，$-1 < x < 1$
3. $\dfrac{1}{1 - x} = \sum_{n=0}^\infty x^n = 1 + x + x^2 + x^3 + \cdots$，$-1 < x < 1$
4. $\ln (1 + x) = \sum_{n=1}^\infty (-1)^{n-1} \dfrac{x^n}{n} = x - \dfrac{x^2}{2} + \dfrac{x^3}{3} - \cdots$，$-1 < x \leqslant 1$
5. $\sin x = \sum_{n=0}^\infty (-1)^n \dfrac{x^{2n+1}}{(2n+1)!} = x - \dfrac{x^3}{3!} + \dfrac{x^5}{5!} - \cdots$，$-\infty < x < +\infty$
6. $\cos x = \sum_{n=0}^\infty (-1)^n \dfrac{x^{2n}}{(2n)!} = 1 - \dfrac{x^2}{2!} + \dfrac{x^4}{4!} - \cdots$，$-\infty < x < +\infty$
7. $(1 + x)^\alpha = 1 + \alpha x + \dfrac{\alpha (\alpha - 1)}{2!} x^2 + \cdots + \dfrac{\alpha (\alpha - 1) \cdots (\alpha - n + 1)}{n!} x^n + \cdots$，  
   $\begin{cases} 
   x \in (-1, 1), & \alpha \leqslant -1 \\ 
   x \in (-1, 1], & -1 < \alpha < 0 \\ 
   x \in [-1, 1], & \alpha > 0 
   \end{cases}$

</ul>

### 求法

<ul>

#### 直接法

<ul>

逐个计算 $a_n = \dfrac{f^{(n)}(x_0)}{n!}$ 并代入，但通常较麻烦。

</ul>

#### 间接法

<ul>

利用上述七个展开式，通过变量代换、四则运算、逐项求导、逐项积分和待定系数等方法求解。

</ul>

</ul>

</ul>

## 幂级数求和函数

<ul>

### 求和函数概念

<ul>

<span style="color: violet;">**定义：**</span>在收敛域上，记 $S(x) = \sum_{n=1}^\infty u_n(x)$，称 $S(x)$ 为 $\sum_{n=1}^\infty u_n(x)$ 的**和函数**。

</ul>

### 运算法则

<ul>

设 $\sum_{n=0}^\infty a_n x^n$ 和 $\sum_{n=0}^\infty b_n x^n$ 的收敛半径分别为 $R_a$ 和 $R_b$：

- $k \sum_{n=0}^\infty a_n x^n = \sum_{n=0}^\infty k a_n x^n$，$|x| < R$，$k$ 为常数
- $\sum_{n=0}^\infty a_n x^n \pm \sum_{n=0}^\infty b_n x^n = \sum_{n=0}^\infty (a_n \pm b_n) x^n$，$|x| < R = \min \{R_a, R_b\}$
- $\left( \sum_{n=0}^\infty a_n x^n \right) \cdot \left( \sum_{n=0}^\infty b_n x^n \right) = \sum_{n=0}^\infty \left( a_0 b_n + a_1 b_{n-1} + \cdots + a_n b_0 \right) x^n$

**恒等变形方法**：

1. 通项与下标一起变化：$\sum_{n=k}^\infty a_n x^n = \sum_{n=k+l}^\infty a_{n-l} x^{n-l}$
2. 只变下标：$\sum_{n=0}^\infty a_n x^n = a_k x^k + \cdots + a_{k+l-1} x^{k+l-1} + \sum_{n=k+l}^\infty a_n x^n$
3. 只变通项：$\sum_{n=0}^\infty a_n x^n = x^l \sum_{n=0}^\infty a_n x^{n-l}$

</ul>

### 幂级数性质

<ul>

- **连续性**：和函数 $S(x)$ 在收敛区间 $I$ 上连续，若端点 $x = \pm R$ 收敛，则在 $(-R, R]$ 或 $[-R, R)$ 上连续。
- **逐项可积性**：$S(x)$ 在 $I$ 上可积，且：

  $$
  \int_0^x S(t) \, dt = \sum_{n=0}^\infty \dfrac{a_n}{n+1} x^{n+1}
  $$

  收敛半径不变，收敛域可能扩大。

- **逐项可导性**：$S(x)$ 在 $(-R, R)$ 内可导，且：

  $$
  S'(x) = \sum_{n=1}^\infty n a_n x^{n-1}
  $$

  收敛半径不变，收敛域可能缩小。

</ul>

</ul>

</ul>

</ul>

---

# 傅里叶级数

<ul>

## 傅里叶级数概念

<ul>

### 三角级数

<ul>

周期函数可由正弦函数叠加表示：

$$
f(x) = A_0 + \sum_{n=1}^\infty A_n \sin (n \omega t + \varphi_n)
$$

称为**三角级数**。

</ul>

### 三角函数族

<ul>

$\{1, \cos nx, \sin nx\}$（$n \in \mathbb{N}^*$）在 $[-\pi, \pi]$ 上具有**正交性**：

- $\int_{-\pi}^\pi 1 \cdot \cos nx \, dx = 0$
- $\int_{-\pi}^\pi 1 \cdot \sin nx \, dx = 0$
- $\int_{-\pi}^\pi \cos mx \cdot \sin nx \, dx = 0$
- $\int_{-\pi}^\pi \cos mx \cdot \cos nx \, dx = 0$（$m \neq n$），$=\pi$（$m = n$）
- $\int_{-\pi}^\pi \sin mx \cdot \sin nx \, dx = 0$（$m \neq n$），$=\pi$（$m = n$）
- $\int_{-\pi}^\pi 1^2 \, dx = 2\pi$

</ul>

</ul>

## 周期傅里叶级数

<ul>

对于周期为 $2\pi$ 的函数 $f(x)$，其傅里叶级数为：

$$
S(x) = \dfrac{a_0}{2} + \sum_{n=1}^\infty (a_n \cos nx + b_n \sin nx)
$$

**迪利克雷充分条件**：

1. $f(x)$ 在 $[-\pi, \pi]$ 上连续或只有有限个第一类间断点；
2. $f(x)$ 在 $[-\pi, \pi]$ 上至多有有限个极值点。

则 $f(x) \sim S(x)$，系数为：

- $a_0 = \dfrac{1}{\pi} \int_{-\pi}^\pi f(x) \, dx$
- $a_n = \dfrac{1}{\pi} \int_{-\pi}^\pi f(x) \cos nx \, dx$
- $b_n = \dfrac{1}{\pi} \int_{-\pi}^\pi f(x) \sin nx \, dx$

- 连续点：$S(x) = f(x)$
- 间断点：$S(x) = \dfrac{f(x-0) + f(x+0)}{2}$

**例题**：设周期为 $2\pi$ 的 $f(x)$ 在 $[-\pi, \pi]$ 上为：

$$
f(x) = \begin{cases} 
0, & -\pi \leqslant x < 0 \\ 
x, & 0 \leqslant x < \pi 
\end{cases}
$$

**解**：

- $a_0 = \dfrac{1}{\pi} \int_0^\pi x \, dx = \dfrac{\pi}{2}$
- $a_n = \dfrac{1}{\pi} \int_0^\pi x \cos nx \, dx = \dfrac{(-1)^n - 1}{\pi n^2}$（奇数时为 $-\dfrac{2}{\pi n^2}$，偶数时为 0）
- $b_n = \dfrac{1}{\pi} \int_0^\pi x \sin nx \, dx = \dfrac{(-1)^{n+1}}{n}$

$$
f(x) \sim \dfrac{\pi}{4} + \sum_{n=1}^\infty \left( a_n \cos nx + b_n \sin nx \right)
$$

</ul>

## 非周期傅里叶级数

<ul>

### $[-\pi, \pi]$

<ul>

将 $f(x)$ 周期延拓为 $F(x)$，展开后判断端点是否包含。

**例题**：展开 $f(x) = |x|$（$-\pi \leqslant x \leqslant \pi$）。

**解**：

- $a_0 = \dfrac{2}{\pi} \int_0^\pi x \, dx = \pi$
- $a_n = \dfrac{2}{\pi} \int_0^\pi x \cos nx \, dx = \dfrac{2}{\pi n^2} [(-1)^n - 1]$（奇数时 $-\dfrac{4}{\pi n^2}$，偶数时 0）
- $b_n = 0$

$$
|x| = \dfrac{\pi}{2} - \dfrac{4}{\pi} \left( \cos x + \dfrac{1}{9} \cos 3x + \dfrac{1}{25} \cos 5x + \cdots \right)
$$

收敛域为 $[-\pi, \pi]$。

</ul>

### $[0, \pi]$

<ul>

1. **奇延拓**（正弦级数）：
   - $a_0 = a_n = 0$
   - $b_n = \dfrac{2}{\pi} \int_0^\pi f(x) \sin nx \, dx$
   - $f(x) = \sum_{n=1}^\infty b_n \sin nx$
2. **偶延拓**（余弦级数）：
   - $a_0 = \dfrac{2}{\pi} \int_0^\pi f(x) \, dx$
   - $a_n = \dfrac{2}{\pi} \int_0^\pi f(x) \cos nx \, dx$
   - $f(x) = \dfrac{a_0}{2} + \sum_{n=1}^\infty a_n \cos nx$

**例题**：展开 $f(x) = x$（$0 \leqslant x \leqslant \pi$）。

**解**：

- **偶延拓**：
  - $a_0 = \pi$
  - $a_n = \dfrac{2}{\pi} \int_0^\pi x \cos nx \, dx = \dfrac{2}{\pi n^2} [(-1)^n - 1]$（奇数时 $-\dfrac{4}{\pi n^2}$）
  - $x = \dfrac{\pi}{2} - \dfrac{4}{\pi} \left( \cos x + \dfrac{1}{9} \cos 3x + \cdots \right)$，$[0, \pi]$
- **奇延拓**：
  - $b_n = \dfrac{2}{\pi} \int_0^\pi x \sin nx \, dx = \dfrac{2 (-1)^{n+1}}{n}$
  - $x = \sum_{n=1}^\infty \dfrac{2 (-1)^{n+1}}{n} \sin nx$，$[0, \pi)$

</ul>

</ul>

## 任意区间傅里叶级数

<ul>

$$
S(x) = \dfrac{a_0}{2} + \sum_{n=1}^\infty \left( a_n \cos \dfrac{n \pi x}{l} + b_n \sin \dfrac{n \pi x}{l} \right)
$$

- $a_n = \dfrac{1}{l} \int_{-l}^l f(x) \cos \dfrac{n \pi x}{l} \, dx$
- $b_n = \dfrac{1}{l} \int_{-l}^l f(x) \sin \dfrac{n \pi x}{l} \, dx$

**例题**：展开 $f(x) = 1 - x^2$（$-\pi \leqslant x \leqslant \pi$）。

**解**：

- $a_0 = \dfrac{2}{\pi} \int_0^\pi (1 - x^2) \, dx = 2 - \dfrac{2}{3} \pi^2$
- $a_n = \dfrac{2}{\pi} \int_0^\pi (1 - x^2) \cos nx \, dx = \dfrac{4 (-1)^n}{n^2}$
- $b_n = 0$

$$
f(x) \sim 1 - \dfrac{\pi^2}{3} + \sum_{n=1}^\infty \dfrac{4 (-1)^n}{n^2} \cos nx
$$

</ul>

</ul>

</ul>