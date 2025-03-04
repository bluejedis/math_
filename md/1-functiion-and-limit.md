# 映射与函数

<ul>

## 邻域

<ul>

### 一维

<ul>

**邻域定义：** 以点 $x_0$ 为中心的任何开区间为点 $x_0$ 的邻域，记为 $U(x_0)$。

**$\delta$ 邻域定义：** 设 $\delta$ 为一正数，则称开区间 $(x_0 - \delta, x_0 + \delta)$ 为点 $x_0$ 的 $\delta$ 邻域，记作 $U(x_0, \delta)$。$x_0$ 称为邻域的中心，$\delta$ 为邻域的半径。

**去心 $\delta$ 邻域** 就是去除 $x_0$ 的 $\delta$ 邻域，记为 $\mathring{U}(x_0, \delta)$，**左 $\delta$ 邻域** 为左侧的去心 $\delta$ 邻域，记为 $U^+(x_0, \delta)$，**右 $\delta$ 邻域** 为右侧的去心 $\delta$ 邻域，记为 $U^-(x_0, \delta)$。

</ul>

### 二维

<ul>

**邻域定义：** 设点 $P_0(x_0, y_0)$ 为 $xOy$ 平面上的一点，$\delta$ 为某正数，与点 $P_0(x_0, y_0)$ 的距离小于 $\delta$ 的点 $P(x, y)$ 的全体，称为点 $P_0$ 的 $\delta$ 邻域，记为 $U(P_0, \delta)$。

同理可定义 **去心 $\delta$ 邻域**。

**$\delta$ 邻域的几何意义：** 以 $P_0(x_0, y_0)$ 为中心，以 $\delta > 0$ 为半径的圆内部所有的点。

函数的邻域是一个区间，因此函数在某点的某邻域内有定义，说明函数在这个点的附近有定义，而这个附近的距离无需具体说明。

</ul>

</ul>

## 函数的概念

<ul>

### 函数

<ul>

- 函数即 $y = f(x), x \in D$，其中 $x$ 为自变量，$y$ 为因变量，$D$ 为定义域。
- 一个 $x$ 对应一个 $y$，一个 $y$ 可能对应多个 $x$。

</ul>

### 反函数

<ul>

$y = f(x)$，定义域为 $D$，值域为 $R$。若对于每一个 $y \in R$，必然存在 $x \in D$ 使 $y = f(x)$ 成立，则可定义新函数 $x = \psi(y)$，此函数为 $y = f(x)$ 的 **反函数**，记作 $x = f^{-1}(y)$。其定义域为 $R$，值域为 $D$。对于反函数，原函数称为 **直接函数**。

1. **严格单调** 函数必然有反函数，即函数导数恒正或恒负时必有反函数。
2. $x = f^{-1}(y)$ 与 $y = f(x)$ 在同一坐标系中完全重合。
3. $y = f^{-1}(x)$ 与 $y = f(x)$ 关于 $y = x$ 对称。
4. $f[f^{-1}(x)]$（即 $f[\psi(x)]$）或 $f^{-1}[f(x)] = x$（即 $\psi[f(x)]$），称为湮灭。

验证性质 4：已知 $y = e^x$ 和 $y = \ln x$ 是一对反函数，$y = \ln e^x = f^{-1}(f(x)) = x$。

**反函数的求法：**

1. 求值域。
2. 求解（用 $y$ 表示 $x$）。
3. 互换 $x$ 和 $y$。

**例题：** 若函数 $y = f(x)$ 的反函数为 $y = f^{-1}(x)$，求 $y = f(2x - 1) + 1$ 的反函数解析式。

**解：**  
整理 $y = f(2x - 1) + 1$，得 $f(2x - 1) = y - 1$。  
将 $2x - 1$ 视为 $x$，$y - 1$ 视为 $y$，则反函数为 $2x - 1 = f^{-1}(y - 1)$。  
解得 $x = \dfrac{f^{-1}(y - 1) + 1}{2}$。  
交换表示法，反函数为 $y = \dfrac{f^{-1}(x - 1) + 1}{2}$。

**例题：** 已知 $f(x) = \dfrac{1}{1 - x^2}$（$x < -1$），求 $f^{-1}\left(-\dfrac{1}{3}\right)$。

**解：**  
求 $f^{-1}\left(-\dfrac{1}{3}\right)$，即原函数中 $y = -\dfrac{1}{3}$ 时 $x$ 的值。  
解 $\dfrac{1}{1 - x^2} = -\dfrac{1}{3}$，得 $1 - x^2 = -3$，$x = \pm 2$。因 $x < -1$，取 $x = -2$。

**例题：** 已知 $f(x) = \dfrac{1 - 2x}{1 + x}$，函数 $g(x)$ 的图像与 $y = f^{-1}(x + 1)$ 关于 $y = x$ 对称，求 $g(5)$。

**解：**  
因 $g(x)$ 与 $f^{-1}(x + 1)$ 关于 $y = x$ 对称，$g(x)$ 与 $f^{-1}(x + 1)$ 互为反函数。  
设 $y = f^{-1}(x + 1)$，则 $x + 1 = f(y)$，$x = f(y) - 1$，即 $y = f^{-1}(x + 1) = f(y) - 1$。  
故 $g(x) = f(x) - 1$，$g(5) = f(5) - 1 = \dfrac{1 - 2 \cdot 5}{1 + 5} - 1 = -\dfrac{5}{2}$。

**例题：** 已知 $f(x) = \dfrac{1}{2}(x^2 + \sqrt{x + 1})$（$x \geqslant 0$）的反函数为 $f^{-1}(x)$，求不等式 $f^{-1}(x + 1) > 3$ 的解集。

**解：**  
当 $x \geqslant 0$ 时，$f(x)$ 单调递增（因 $f'(x) = x + \dfrac{1}{2\sqrt{x + 1}} > 0$）。  
反函数 $f^{-1}(x)$ 在定义域 $[\dfrac{1}{2}, +\infty)$ 上也单调递增（$f(0) = \dfrac{1}{2}$）。  
由 $f^{-1}(x + 1) > 3$，两边取 $f$，得 $x + 1 > f(3)$。  
计算 $f(3) = \dfrac{1}{2}(3^2 + \sqrt{3 + 1}) = \dfrac{9 + 2}{2} = \dfrac{11}{2}$。  
且 $x + 1 \geqslant \dfrac{1}{2}$，故 $x \geqslant -\dfrac{1}{2}$。  
解 $x + 1 > \dfrac{11}{2}$，得 $x > \dfrac{9}{2}$。  
结合 $x \geqslant 0$，解集为 $x > \dfrac{9}{2}$。

**例题：** 求函数 $y = f(x) = \ln(x + \sqrt{x^2 + 1})$ 的反函数 $f^{-1}(x)$ 的表达式及其定义域。

**解：**  
**定义域：** $\ln(x)$ 要求 $x + \sqrt{x^2 + 1} > 0$，对任意实数 $x$，$x + \sqrt{x^2 + 1} > 0$ 恒成立，故 $x \in \mathbb{R}$。  
**奇偶性：** $f(-x) = \ln(-x + \sqrt{x^2 + 1}) = -\ln(x + \sqrt{x^2 + 1}) = -f(x)$，故为奇函数。  
**单调性：** $f'(x) = \dfrac{1}{x + \sqrt{x^2 + 1}} \cdot \left(1 + \dfrac{x}{\sqrt{x^2 + 1}}\right) = \dfrac{1}{\sqrt{x^2 + 1}} > 0$，故严格单调递增。  
**反函数：**  
设 $y = \ln(x + \sqrt{x^2 + 1})$，则 $e^y = x + \sqrt{x^2 + 1}$。  
又 $-y = \ln\left(\dfrac{1}{x + \sqrt{x^2 + 1}}\right) = \ln(\sqrt{x^2 + 1} - x)$，$e^{-y} = \sqrt{x^2 + 1} - x$。  
两式相减：$e^y - e^{-y} = 2x$，$x = \dfrac{e^y - e^{-y}}{2}$。  
故 $f^{-1}(x) = \dfrac{e^x - e^{-x}}{2}$，定义域为 $\mathbb{R}$（因 $f(x)$ 值域为 $\mathbb{R}$）。

</ul>

### 复合函数

<ul>

设 $y = f(u)$ 的定义域为 $D_1$，$u = g(x)$ 在 $D$ 上有定义且 $g(D) \subseteq D_1$，则 $y = f[g(x)], x \in D$ 为复合函数，定义域为 $D$，$u$ 为中间变量。

**例题：** 设 $f(x) = x^2$，$f[\psi(x)] = -x^2 + 2x + 3$，且 $\psi(x) \geqslant 0$，求 $\psi(x)$ 及其定义域与值域。

**解：**  
由 $f[\psi(x)] = [\psi(x)]^2 = -x^2 + 2x + 3$，且 $\psi(x) \geqslant 0$，  
故 $\psi(x) = \sqrt{-x^2 + 2x + 3}$。  
**定义域：** $-x^2 + 2x + 3 \geqslant 0$，解得 $x \in [-1, 3]$。  
**值域：** $\psi(x) = \sqrt{-(x - 1)^2 + 4}$，最大值 $\sqrt{4} = 2$（$x = 1$），最小值 0（$x = -1$ 或 $3$），故值域为 $[0, 2]$。

**例题：** 设 $f(x) = \begin{cases} \ln \sqrt{x}, & x \geqslant 1 \\ 2x - 1, & x < 1 \end{cases}$，求 $f[f(x)]$。

**解：**  
$f[f(x)] = \begin{cases} \ln \sqrt{f(x)}, & f(x) \geqslant 1 \\ 2f(x) - 1, & f(x) < 1 \end{cases}$。  
分析 $f(x)$：  
- $x < 1$ 时，$f(x) = 2x - 1 < 1$，故 $f[f(x)] = 2(2x - 1) - 1 = 4x - 3$。  
- $x \geqslant 1$ 时，$f(x) = \ln \sqrt{x} \geqslant 0$：  
  - 若 $0 \leqslant \ln \sqrt{x} < 1$，即 $1 \leqslant x < e^2$，则 $f[f(x)] = 2\ln \sqrt{x} - 1 = \ln x - 1$。  
  - 若 $\ln \sqrt{x} \geqslant 1$，即 $x \geqslant e^2$，则 $f[f(x)] = \ln \sqrt{\ln \sqrt{x}}$。  
故 $f[f(x)] = \begin{cases} 4x - 3, & x < 1 \\ \ln x - 1, & 1 \leqslant x < e^2 \\ \ln \sqrt{\ln \sqrt{x}}, & x \geqslant e^2 \end{cases}$。

</ul>

</ul>

## 函数的特性

<ul>

### 有界性

<ul>

**定义：** 函数 $f(x)$ 的定义域为 $D$，数集 $I \subseteq D$，若存在正数 $M$，对任意 $x \in I$，有 $|f(x)| \leqslant M$，则 $f(x)$ 在 $I$ 上有界，否则无界。

须指明定义域区间才能讨论有界性。  
- 若 $f(x) \geqslant M$，则有下界。  
- 若 $f(x) \leqslant M$，则有上界。

</ul>

### 单调性

<ul>

**定义：** $y = f(x)$，$x \in D$，若 $\forall x_1, x_2 \in D$ 且 $x_1 < x_2$，有 $f(x_1) < f(x_2)$，则函数在 $D$ 上单调递增；反之单调递减。

$$
\begin{cases}
\dfrac{dy}{dx} > 0 \Rightarrow (x_1 - x_2)[f(x_1) - f(x_2)] > 0 \Rightarrow f(x) \nearrow \\
\dfrac{dy}{dx} < 0 \Rightarrow (x_1 - x_2)[f(x_1) - f(x_2)] < 0 \Rightarrow f(x) \searrow
\end{cases}
$$

</ul>

### 奇偶性

<ul>

1. **奇函数：** 关于原点对称，$f(-x) = -f(x)$。  
2. **偶函数：** 关于 $y$ 轴对称，$f(-x) = f(x)$。  
3. 对于定义在 $[-l, l]$ 上的任意函数 $f(x)$，$F_1(x) = f(x) - f(-x)$ 为奇函数，$F_2(x) = f(x) + f(-x)$ 为偶函数。  
4. 若奇函数在 0 处有定义，则 $f(0) = 0$。  
5. 若偶函数在 0 处有导数，则 $f'(0) = 0$。  
6. 函数 $y = f(x)$ 关于 $x = T$ 对称的充要条件是 $f(x) = f(2T - x)$ 或 $f(x + T) = f(x - T)$。

</ul>

### 周期性

<ul>

$f(x + T) = f(x)$，其中 $T$ 为周期。

</ul>

### 重要结论

<ul>

1. 若 $f(x)$ 为可导偶函数，则 $f'(x)$ 为奇函数。  
2. 若 $f(x)$ 为可导奇函数，则 $f'(x)$ 为偶函数。  
3. 若 $f(x)$ 为周期函数，则 $f'(x)$ 也为周期函数且周期不变。  
4. 连续奇函数的一切原函数均为偶函数。  
5. 连续偶函数的原函数中仅一个为奇函数。  
6. 若连续函数 $f(x)$ 以 $T$ 为周期且 $\int_0^T f(x) \, dx = 0$，则其一切原函数也以 $T$ 为周期。  
7. 若 $f(x)$ 在有限区间 $(a, b)$ 中可导且 $f'(x)$ 有界，则 $f(x)$ 在 $(a, b)$ 有界。

**注意：** 0 和 1 处的函数定义需谨慎：  
- 如 $a = 0$ 时，$f(b) - f(a) = f'(\xi)(b - a) = f(b) = b f'(\xi)$。  
- 如 $f(x) > x f(1)$，可变形为 $\dfrac{f(x)}{x} > f(1)$，辅助函数 $F(x) = \dfrac{f(x)}{x}$。

</ul>

</ul>

</ul>

# 数列的极限

<ul>

极限是一个无限逼近某值的过程。例如 $\dfrac{n}{n + 1}$ 在 $n$ 无限增大时逼近 1，记为 $\lim_{n \to \infty} \dfrac{n}{n + 1} = 1$。

## 定义

<ul>

### 数列极限定义

<ul>

**定义：** 设 $\{x_n\}$ 为一数列，若存在常数 $a$，对于任意小的 $\xi > 0$，总存在正整数 $N$，使 $n > N$ 时，$|x_n - a| < \xi$ 恒成立，则 $a$ 为数列 $\{x_n\}$ 的极限，记为 $\lim_{n \to \infty} x_n = a$ 或 $x_n \to a (n \to \infty)$。

**$\xi - N$ 语言：** $\lim_{n \to \infty} x_n = a \Leftrightarrow \forall \xi > 0, \exists N \in \mathbb{N_+}, \text{当 } n > N \text{ 时}, |x_n - a| < \xi$。

若不存在这样的 $a$，则称数列 $x_n$ 发散。

</ul>

### 极限证明

<ul>

令 $x_n$ 为通项，$a$ 为极限值，$\xi$ 为任意正数：

1. 写出 $|x_n - a| < \xi$。  
2. 反解出 $n > g(\xi)$。  
3. 取 $N = [g(\xi)] + 1$，令 $n > N$ 即可证明。

**例题：** 用定义证明 $\lim_{n \to \infty} \left[1 + \dfrac{(-1)^n}{n}\right] = 1$。

**证明：**  
1. $\left|1 + \dfrac{(-1)^n}{n} - 1\right| = \left|\dfrac{(-1)^n}{n}\right| < \xi$。  
2. $\dfrac{1}{n} < \xi$，$n > \dfrac{1}{\xi}$。  
3. 取 $N = \left[\dfrac{1}{\xi}\right] + 1$。  
4. 当 $n > N$ 时，$n > \dfrac{1}{\xi}$，$\left|\dfrac{(-1)^n}{n}\right| < \xi$。  
故极限为 1。

**例题：** 用定义证明 $\lim_{n \to \infty} q^n = 0$（$|q| < 1$）。

**证明：**  
1. $|q^n - 0| < \xi$。  
2. $|q^n| < \xi$，$n \ln |q| < \ln \xi$（因 $\ln |q| < 0$），$n > \dfrac{\ln \xi}{\ln |q|}$。  
3. 取 $N = \left[\dfrac{\ln \xi}{\ln |q|}\right] + 1$。  
4. 当 $n > N$ 时，$|q^n| < \xi$。  
故 $\lim_{n \to \infty} q^n = 0$。

</ul>

### 数列绝对值

<ul>

**定理：** 若 $\lim_{n \to \infty} a_n = A$，则 $\lim_{n \to \infty} |a_n| = |A|$。

**证明：**  
由 $| |a_n| - |A| | \leqslant |a_n - A| < \xi$（当 $n > N$），得 $\lim_{n \to \infty} |a_n| = |A|$。  
**推论：** $\lim_{n \to \infty} a_n = 0 \Leftrightarrow \lim_{n \to \infty} |a_n| = 0$。

</ul>

### 子数列

<ul>

**定义：** 从数列 $\{a_n\}: a_1, a_2, \cdots, a_n, \cdots$ 中按原顺序选取无穷多项，组成新数列 $\{a_{n_k}\}$，称为子列。

**定理：** 若 $\{a_n\}$ 收敛，则其任何子列 $\{a_{n_k}\}$ 也收敛，且极限相同。

**变式：**  
1. 若 $\{a_n\}$ 存在发散子列，则发散。  
2. 若 $\{a_n\}$ 有两个极限不同的收敛子列，则发散。  
3. 若 $\{a_n\}$ 收敛，则奇数子列与偶数子列极限相同。

例：$\{(-1)^n\}$ 的奇数子列极限为 -1，偶数子列为 1，故发散。

</ul>

</ul>

## 性质

<ul>

### 唯一性

<ul>

**定义：** 若数列 $\{x_n\}$ 收敛于 $a$，则 $a$ 唯一。

**证明：**  
假设 $\lim_{n \to \infty} a_n = A$ 且 $\lim_{n \to \infty} a_n = B$，$A > B$。取 $\xi = \dfrac{A - B}{2}$，当 $n > N$ 时，$a_n > \dfrac{A + B}{2}$ 且 $a_n < \dfrac{A + B}{2}$，矛盾。故 $A = B$。

</ul>

### 有界性

<ul>

**定义：** 若数列 $\{x_n\}$ 极限存在，则有界。

**证明：**  
取 $\xi = 1$，当 $n > N$，$|a_n| < 1 + |A|$。取 $M = \max\{|a_1|, \cdots, |a_N|, 1 + |A|\}$，则 $|a_n| \leqslant M$。

**反例：** 有界不一定收敛，如 $1 + (-1)^n$。

</ul>

### 保号性

<ul>

**定义：** 若 $\lim_{n \to \infty} a_n = a \neq 0$，则存在 $N$，当 $n > N$ 时，$a_n$ 与 $a$ 同号。

**证明：** 若 $a > 0$，取 $\xi = \dfrac{a}{2}$，则 $a_n > \dfrac{a}{2} > 0$。

**推论（戴帽法）：** 若 $a_n \geqslant b$（某项起），且 $\lim_{n \to \infty} a_n = a$，则 $a \geqslant b$。

</ul>

</ul>

## 海涅定理（归结原则）

<ul>

**定理：** $\lim_{x \to x_0} f(x) = A$ 存在 $\Leftrightarrow$ 对任何 $\mathring{U}(x_0, \delta)$ 内以 $x_0$ 为极限的数列 $\{x_n\}$（$x_n \neq x_0$），$\lim_{n \to \infty} f(x_n) = A$。

**例题：** 求 $\lim_{n \to \infty} \left(n \tan \dfrac{1}{n}\right)^{n^2}$。

**解：**  
令 $x = \dfrac{1}{n}$，原式为 $\lim_{x \to 0} \left(\dfrac{\tan x}{x}\right)^{\dfrac{1}{x^2}} = e^{\lim_{x \to 0} \dfrac{1}{x^2} \ln \dfrac{\tan x}{x}}$。  
因 $\dfrac{\tan x}{x} \to 1$，$\ln \dfrac{\tan x}{x} \sim \dfrac{\tan x}{x} - 1 \sim \dfrac{x^2}{3}$（泰勒展开），  
hence $\lim_{x \to 0} \dfrac{1}{x^2} \cdot \dfrac{x^2}{3} = \dfrac{1}{3}$，原式 $= e^{\dfrac{1}{3}}$。

</ul>

</ul>

# 函数的极限

<ul>

## 函数极限定义

<ul>

### 极限定义

<ul>

**定义：** 设 $f(x)$ 在 $x_0$ 的去心邻域有定义，若存在常数 $A$，对任意 $\xi > 0$，存在 $\delta > 0$，当 $0 < |x - x_0| < \delta$ 时，$|f(x) - A| < \xi$，则 $A$ 为 $\lim_{x \to x_0} f(x)$。

**$\xi - \delta$ 语言：** $\lim_{x \to x_0} f(x) = A \Leftrightarrow \forall \xi > 0, \exists \delta > 0, 0 < |x - x_0| < \delta \Rightarrow |f(x) - A| < \xi$。

**趋向无穷：** $\lim_{x \to \infty} f(x) = A \Leftrightarrow \forall \xi > 0, \exists X > 0, |x| > X \Rightarrow |f(x) - A| < \xi$。

**注意：** 趋向类型包括 $x \to x_0, x_0^+, x_0^-, \infty, +\infty, -\infty$。

</ul>

### 单侧极限

<ul>

- **左极限：** $x \to x_0^-$。  
- **右极限：** $x \to x_0^+$。

</ul>

### 函数极限存在条件

<ul>

1. $\lim_{x \to x_0} f(x) = A \Leftrightarrow \lim_{x \to x_0^-} f(x) = \lim_{x \to x_0^+} f(x) = A$。  
2. **脱帽法：** $\lim_{x \to x_0} f(x) = A \Leftrightarrow f(x) = A + \alpha(x), \lim_{x \to x_0} \alpha(x) = 0$。

</ul>

### 极限情况总结

<ul>

| 过程         | $n \to \infty$ | $x \to \infty$ | $x \to +\infty$ | $x \to -\infty$ |
|--------------|----------------|-----------------|-----------------|-----------------|
| 时刻         | $N$            | $N$             | $N$             | $N$             |
| 从此时刻以后 | $n > N$        | $|x| > N$       | $x > N$         | $x < -N$        |
| $f(x)$       | $|f(x) - A| < \xi$ | $|f(x) - A| < \xi$ | $|f(x) - A| < \xi$ | $|f(x) - A| < \xi$ |

| 过程         | $x \to x_0$            | $x \to x_0^+$         | $x \to x_0^-$         |
|--------------|------------------------|-----------------------|-----------------------|
| 时刻         | $\delta$              | $\delta$             | $\delta$             |
| 从此时刻以后 | $0 < |x - x_0| < \delta$ | $0 < x - x_0 < \delta$ | $-\delta < x - x_0 < 0$ |
| $f(x)$       | $|f(x) - A| < \xi$ | $|f(x) - A| < \xi$ | $|f(x) - A| < \xi$ |

</ul>

</ul>

## 性质

<ul>

### 唯一性

<ul>

**定义：** 若极限存在，则唯一。

</ul>

### 局部有界性

<ul>

**定义：** 若 $\lim_{x \to x_0} f(x) = A$，则存在 $M > 0$ 和 $\delta > 0$，当 $0 < |x - x_0| < \delta$ 时，$|f(x)| \leqslant M$。

1. 极限存在是局部有界性的充分非必要条件。  
2. $f(x)$ 在 $[a, b]$ 上连续，则有界。  
3. 有限个有界函数的和、差、积仍是有界函数。  
4. 若 $f'(x)$ 在 $(a, b)$ 内有界，则 $f(x)$ 在 $(a, b)$ 有界。

**证明结论 4：**  
由中值定理，$|f(x)| = |f(x_0) + f'(\xi)(x - x_0)| \leqslant |f(x_0)| + K(b - a) = M$。

**例题：** $f(x) = \dfrac{|x| \sin(x - 2)}{x(x - 1)(x - 2)^2}$ 在哪区间有界？  
A. $(-1, 0)$ B. $(0, 1)$ C. $(1, 2)$ D. $(2, 3)$

**解：**  
- $x \to 0^-$：$\lim_{x \to 0^-} f(x) = -\dfrac{\sin 2}{4}$，有界。  
- $x \to 0^+$：$\lim_{x \to 0^+} f(x) = \dfrac{\sin 2}{4}$，有界。  
- $x \to 1^-$：$\lim_{x \to 1^-} f(x) = \infty$，无界。  
- $x \to 2^+$：$\lim_{x \to 2^+} f(x) = \infty$，无界。  
故选 A。

</ul>

### 局部保号性

<ul>

**定义：** 若 $\lim_{x \to x_0} f(x) = A \neq 0$，则存在 $\delta > 0$，当 $0 < |x - x_0| < \delta$ 时，$f(x)$ 与 $A$ 同号。

**证明：** 若 $A > 0$，取 $\xi = \dfrac{A}{2}$，则 $f(x) > \dfrac{A}{2} > 0$。

**推论：** 若 $f(x)$ 在 $x \to x_0$ 时非负或非正，则极限 $A$ 与其同号。

**注意：** 极限不存在的例子：  
1. $\lim_{x \to \infty} e^x$ 不存在（$\lim_{x \to +\infty} e^x = +\infty$, $\lim_{x \to -\infty} e^x = 0$）。  
2. $\lim_{x \to 0} \dfrac{\sin x}{|x|}$ 不存在（$\lim_{x \to 0^+} = 1$, $\lim_{x \to 0^-} = -1$）。

</ul>

</ul>

</ul>

# 极限运算法则

<ul>

1. 有限个无穷小的和为无穷小。  
2. 有界函数与无穷小的乘积为无穷小。  
3. 有限个无穷小的乘积为无穷小。

## 数列极限

<ul>

若 $\lim_{n \to \infty} x_n = a$，$\lim_{n \to \infty} y_n = b$，则：  
1. $\lim_{n \to \infty} (x_n \pm y_n) = a \pm b$。  
2. $\lim_{n \to \infty} (x_n y_n) = ab$。  
3. $\lim_{n \to \infty} \dfrac{x_n}{y_n} = \dfrac{a}{b}$（$b \neq 0$）。

**例题：** 若 $\lim_{n \to \infty} (a_n + b_n) = 1$ 且 $\lim_{n \to \infty} (a_n - b_n) = 3$，求 $\lim_{n \to \infty} a_n$ 和 $\lim_{n \to \infty} b_n$。

**解：**  
令 $u_n = a_n + b_n$，$v_n = a_n - b_n$，则 $\lim u_n = 1$，$\lim v_n = 3$。  
$\lim (u_n + v_n) = 2 \lim a_n = 4$，$\lim a_n = 2$。  
$\lim (u_n - v_n) = 2 \lim b_n = -2$，$\lim b_n = -1$。

</ul>

## 函数极限

<ul>

若 $\lim f(x) = A$，$\lim g(x) = B$，则：  
1. $\lim [k \cdot f(x) \pm l \cdot g(x)] = kA \pm lB$（$k, l$ 为常数）。  
2. $\lim [f(x) \cdot g(x)] = A \cdot B$。  
3. $\lim [f(x)]^n = A^n$（$n$ 为正整数）。  
4. $\lim \dfrac{f(x)}{g(x)} = \dfrac{A}{B}$（$B \neq 0$）。  
5. $\lim_{x \to \infty} \dfrac{a_n x^n + \cdots + a_0}{b_m x^m + \cdots + b_0} = \begin{cases} \dfrac{a_n}{b_m}, & n = m \\ 0, & n < m \\ \infty, & n > m \end{cases}$。  
6. 若 $f(x) \geqslant g(x)$，则 $A \geqslant B$。  
7. 若 $y = f[g(x)]$，$\lim_{x \to x_0} g(x) = u_0$，$\lim_{u \to u_0} f(u) = a$，且 $g(x) \neq u_0$，则 $\lim_{x \to x_0} f[g(x)] = a$。

</ul>

## 存在与不存在的运算关系

<ul>

1. 存在与不存在的和差一定不存在。  
2. 不存在与不存在的和差不一定存在（如 $\sin \dfrac{1}{x} + \sin \dfrac{1}{x}$）。  
3. 存在与不存在的乘积不一定存在（如 $x \sin \dfrac{1}{x}$）。

</ul>

</ul>

# 极限存在准则与两个重要极限

<ul>

## 夹逼准则

<ul>

### 数列的夹逼准则

<ul>

1. $y_n \leqslant x_n \leqslant z_n$。  
2. $\lim_{n \to \infty} y_n = a$，$\lim_{n \to \infty} z_n = a$。  
3. 则 $\lim_{n \to \infty} x_n = a$。

**例题：** 求 $\lim_{n \to \infty} \left(\dfrac{n}{n^2 + 1} + \cdots + \dfrac{n}{n^2 + n}\right)$。

**解：**  
$\dfrac{n^2}{n^2 + n} < \sum_{i=1}^n \dfrac{n}{n^2 + i} < \dfrac{n^2}{n^2 + 1}$，  
两边极限均为 1，故原极限为 1。

</ul>

### 函数的夹逼准则

<ul>

1. $g(x) \leqslant f(x) \leqslant h(x)$（在 $\mathring{U}(x_0, \delta)$）。  
2. $\lim g(x) = A$，$\lim h(x) = A$。  
3. 则 $\lim f(x) = A$。

**例题：** 求 $\lim_{x \to +\infty} (2 + \sin x)^{\dfrac{1}{x}}$。

**解：**  
$1 \leqslant 2 + \sin x \leqslant 3$，$1^{\dfrac{1}{x}} \leqslant (2 + \sin x)^{\dfrac{1}{x}} \leqslant 3^{\dfrac{1}{x}}$，  
两边极限为 1，故原极限为 1。

</ul>

</ul>

## 单调有界准则

<ul>

### 数列单调有界准则

<ul>

**定义：** 单调有界数列必有极限。

**证明需：**  
1. 单调性：$x_{n+1} - x_n$ 或 $\dfrac{x_{n+1}}{x_n}$。  
2. 有界性：$|x_n| \leqslant M$。

**例题：** $a_1 = a > 0$，证明 $a_{n+1} = \dfrac{1}{2} \left(a_n + \dfrac{2}{a_n}\right)$ 极限存在并求出。

**解：**  
$a_n > 0$，$a_{n+1} \geqslant \sqrt{2}$（由 $\dfrac{a + b}{2} \geqslant \sqrt{ab}$），有下界。  
$a_{n+1} - a_n = \dfrac{2 - a_n^2}{2a_n} \leqslant 0$，单调减少。  
极限存在，设为 $A$，则 $A = \dfrac{1}{2} \left(A + \dfrac{2}{A}\right)$，$A = \sqrt{2}$。

</ul>

### 柯西极限存在准则

<ul>

**定义：** $\{x_n\}$ 收敛 $\Leftrightarrow$ $\forall \xi > 0, \exists N, m, n > N \Rightarrow |x_n - x_m| < \xi$。

</ul>

</ul>

## $\lim_{x \to 0} \dfrac{\sin x}{x} = 1$

<ul>

**证明：**  
当 $0 < x < \dfrac{\pi}{2}$，$\sin x < x < \tan x$，  
$\cos x < \dfrac{\sin x}{x} < 1$，  
$0 < 1 - \dfrac{\sin x}{x} < 1 - \cos x = 2 \sin^2 \dfrac{x}{2} \leqslant \dfrac{x^2}{2}$，  
由夹逼准则，极限为 1。

</ul>

## $\lim_{x \to \infty} \left(1 + \dfrac{1}{x}\right)^x = e$

<ul>

**证明：**  
$\lim_{x \to \infty} e^{x \ln \left(1 + \dfrac{1}{x}\right)} = e^{\lim_{x \to \infty} \dfrac{\ln \left(1 + \dfrac{1}{x}\right)}{\dfrac{1}{x}}} = e^1 = e$。

</ul>

</ul>

# 无穷大与无穷小

<ul>

## 无穷

<ul>

### 无穷定义

<ul>

**无穷小：** $\lim_{x \to x_0 (\infty)} f(x) = 0$。  
**无穷大：** $\lim_{x \to x_0 (\infty)} |f(x)| \to \infty$。

**定理：** 若 $f(x)$ 为无穷大，则 $\dfrac{1}{f(x)}$ 为无穷小；若 $f(x)$ 为无穷小且不为 0，则 $\dfrac{1}{f(x)}$ 为无穷大。

</ul>

### 无穷小的比较

<ul>

设 $\lim \alpha(x) = 0$，$\lim \beta(x) = 0$，$\beta(x) \neq 0$：  
1. $\lim \dfrac{\alpha(x)}{\beta(x)} = 0$，$\alpha(x) = o(\beta(x))$（高阶）。  
2. $\lim \dfrac{\alpha(x)}{\beta(x)} = \infty$，低阶。  
3. $\lim \dfrac{\alpha(x)}{\beta(x)} = c \neq 0$，同阶。  
4. $\lim \dfrac{\alpha(x)}{\beta(x)} = 1$，$\alpha(x) \sim \beta(x)$（等价）。  
5. $\lim \dfrac{\alpha(x)}{[\beta(x)]^k} = c \neq 0$，$k$ 阶。

**例题：** 证明 $\sqrt[n]{1 + x} - 1 \sim \dfrac{1}{n} x$（$x \to 0$）。

**解：**  
令 $t = \sqrt[n]{1 + x} - 1$，$x = (1 + t)^n - 1 \approx n t$，  
$\lim_{x \to 0} \dfrac{t}{x} = \dfrac{1}{n}$，故等价。

</ul>

</ul>

## 洛必达法则

<ul>

**定理：** 若 $f(x), F(x) \to 0$ 或 $\infty$，$f'(x), F'(x)$ 存在且 $F'(x) \neq 0$，$\lim \dfrac{f'(x)}{F'(x)}$ 存在，则 $\lim \dfrac{f(x)}{F(x)} = \lim \dfrac{f'(x)}{F'(x)}$。

</ul>

## 泰勒公式

<ul>

### 麦克劳林公式

<ul>

1. $e^x = 1 + x + \dfrac{x^2}{2!} + o(x^2)$。  
2. $\ln(1 + x) = x - \dfrac{x^2}{2} + o(x^2)$。

</ul>

### 常用等价无穷小

<ul>

1. $x \sim \sin x \sim \tan x$（$x \to 0$）。  
2. $1 - \cos x \sim \dfrac{1}{2} x^2$。

</ul>

</ul>

</ul>

# 函数连续性与间断点

<ul>

## 连续定义

<ul>

**定义：** 若 $\lim_{x \to x_0} f(x) = f(x_0)$，则 $f(x)$ 在 $x_0$ 处连续。

</ul>

## 间断定义

<ul>

**定义：** 若 $\lim_{x \to x_0} f(x) \neq f(x_0)$，则间断。

</ul>

## 间断点分类

<ul>

### 可去间断点

<ul>

**定义：** $\lim_{x \to x_0} f(x) = A \neq f(x_0)$（或未定义）。

</ul>

### 跳跃间断点

<ul>

**定义：** $\lim_{x \to x_0^-} f(x) \neq \lim_{x \to x_0^+} f(x)$。

</ul>

### 无穷间断点

<ul>

**定义：** $\lim_{x \to x_0} f(x) = \infty$。

</ul>

### 振荡间断点

<ul>

**定义：** $\lim_{x \to x_0} f(x)$ 因振荡不存在。

**例题：** $f(x) = \begin{cases} 2x + a, & x \leqslant 0 \\ e^x (\sin x + \cos x), & x > 0 \end{cases}$ 在 $\mathbb{R}$ 上连续，求 $a$。

**解：**  
$\lim_{x \to 0^-} f(x) = a$，$\lim_{x \to 0^+} f(x) = 1$，故 $a = 1$。

</ul>

</ul>

</ul>

# 闭区间上连续函数的性质

<ul>

## 有界性与最大最小值定理

<ul>

**定理：** $f(x)$ 在 $[a, b]$ 上连续，必有最大值、最小值和有界。

</ul>

## 零点与介值定理

<ul>

**零点定理：** 若 $f(a)f(b) < 0$，则 $\exists \xi \in [a, b], f(\xi) = 0$。  
**介值定理：** 若 $f(a) \neq f(b)$，则 $\exists \xi \in [a, b], f(\xi) = \mu$（$\mu$ 介于 $f(a)$ 和 $f(b)$ 之间）。

**例题：** 证明 $x = a \sin x + b$（$a, b > 0$）至少有一个正根且不超过 $a + b$。

**解：**  
令 $f(x) = x - a \sin x - b$，$f(0) = -b < 0$，$f(a + b) = a(1 - \sin(a + b)) \geqslant 0$，  
由零点定理，$\exists \xi \in [0, a + b]$ 使 $f(\xi) = 0$。

</ul>

## 一致连续性

<ul>

**定义：** 若 $\forall \xi > 0, \exists \delta > 0$，当 $|x_1 - x_2| < \delta$ 时，$|f(x_1) - f(x_2)| < \xi$，则 $f(x)$ 在区间 $I$ 上一致连续。

**定理：** 在闭区间上连续的函数一致连续。

</ul>

</ul>