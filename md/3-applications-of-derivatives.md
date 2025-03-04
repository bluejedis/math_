# 函数中值定理

<ul>

都假定 $f(x)$ 在 $[a, b]$ 上连续。

## 有界与最值定理

<ul>

**定理：** $m \leqslant f(x) \leqslant M$，其中 $m$ 和 $M$ 分别为 $f(x)$ 在 $[a, b]$ 上的最小值和最大值。

</ul>

## 介值定理

<ul>

**定理：** 当 $m \leqslant \mu \leqslant M$ 时，存在 $\xi \in [a, b]$，使得 $f(\xi) = \mu$。

</ul>

## 平均值定理

<ul>

**定理：** 当 $a < x_1 < x_2 < \cdots < x_n < b$ 时，在 $[x_1, x_n]$ 内至少存在一点 $\xi$，使得 $f(\xi) = \frac{f(x_1) + f(x_2) + \cdots + f(x_n)}{n}$。

**证明：**  
已知 $f(x)$ 在 $[x_1, x_n]$ 上连续，根据有界与最值定理，$m \leqslant f(x) \leqslant M$。  
即 $m \leqslant f(x_1) \leqslant M$，$m \leqslant f(x_2) \leqslant M$，…，$m \leqslant f(x_n) \leqslant M$。  
将这些式子相加，得 $nm \leqslant f(x_1) + f(x_2) + \cdots + f(x_n) \leqslant nM$。  
所以 $m \leqslant \frac{f(x_1) + f(x_2) + \cdots + f(x_n)}{n} \leqslant M$。  
由介值定理，可知存在 $\xi \in [x_1, x_n]$ 使得 $f(\xi) = \frac{f(x_1) + f(x_2) + \cdots + f(x_n)}{n}$。

</ul>

## 零点定理

<ul>

**定理：** 当 $f(a) \cdot f(b) < 0$ 时，存在 $\xi \in (a, b)$，使得 $f(\xi) = 0$。

</ul>

</ul>

# 微分中值定理

<ul>

四个定理都建立局部与整体的关系，利用导数控制函数，反之不能使用函数控制导数。

$$
\text{罗尔定理} \xrightleftharpoons[\text{特例：} f(a) = f(b)]{\text{泛化：任意端点值}} \text{拉格朗日中值定理} \xrightleftharpoons[\text{特例：} F(x) = x]{\text{泛化：参数方程}} \text{柯西中值定理}
$$

## 罗尔定理

<ul>

### 定义

<ul>

**极值定义：** 若 $\exists \delta > 0$，使 $\forall x \in U(x_0, \delta)$ 恒有 $f(x) \geqslant f(x_0)$，则 $f(x)$ 在 $x_0$ 处取极小值；若 $f(x) \leqslant f(x_0)$，则取极大值。

**费马引理：** 若 $f(x)$ 在 $x_0$ 处取得极值，且 $f(x)$ 在 $x_0$ 处可导，则 $f'(x_0) = 0$。

**罗尔定理：**  
1. $f(x)$ 在 $[a, b]$ 上连续。  
2. $f(x)$ 在 $(a, b)$ 内可导。  
3. $f(a) = f(b)$。  
则 $\exists \xi \in (a, b)$，使得 $f'(\xi) = 0$。

*图像描述：展示一个在 [a, b] 上连续的曲线，例如 y = sin(x - 0.5) + 2，满足 f(a) = f(b)，并标出导数为零的点 ξ₁ 和 ξ₂。*

</ul>

### 推广

<ul>

- 设 $f(x)$ 在 $(a, b)$ 内可导，$\lim_{x \to a^+} f(x) = \lim_{x \to b^-} f(x) = A$，则在 $(a, b)$ 内至少存在一点 $\xi$，使得 $f'(\xi) = 0$。  
- 设 $f(x)$ 在 $(a, b)$ 内可导，$\lim_{x \to a^+} f(x) = \lim_{x \to b^-} f(x) = \pm \infty$，则在 $(a, b)$ 内至少存在一点 $\xi$，使得 $f'(\xi) = 0$。  
- 设 $f(x)$ 在 $(a, +\infty)$ 内可导，$\lim_{x \to a^+} f(x) = \lim_{x \to +\infty} f(x) = A$，则在 $(a, +\infty)$ 内至少存在一点 $\xi$，使得 $f'(\xi) = 0$。  
- 设 $f(x)$ 在 $(-\infty, +\infty)$ 内可导，$\lim_{x \to -\infty} f(x) = \lim_{x \to +\infty} f(x) = A$，则在 $(-\infty, +\infty)$ 内至少存在一点 $\xi$，使得 $f'(\xi) = 0$。

</ul>

</ul>

## 拉格朗日中值定理

<ul>

1. $f(x)$ 在 $[a, b]$ 上连续。  
2. $f(x)$ 在 $(a, b)$ 内可导。  
则 $\exists \xi \in (a, b)$，使得 $f(b) - f(a) = f'(\xi)(b - a)$。

**几何意义：** 若连续曲线 $y = f(x)$ 的弧 $\wideparen{AB}$ 上除端点外处处具有不垂直于 $x$ 轴的切线，则弧上至少有一点 $C$，使曲线在该点处的切线平行于弦 $AB$。

**有限增量公式：** $\Delta y = f(x_0 + \Delta x) - f(x_0) = f'[x_0 + \theta \Delta x] \Delta x$（$0 < \theta < 1$）。  
注：$\Delta x$ 不一定很小，这是一个准确公式，用 $\Delta x$ 和某点导数表示增量 $\Delta y$，与微分值不同（后者为近似值），但因 $\theta$ 未知，实用性有限。

**推论：** $f(x)$ 在 $I$ 上连续且可导，则 $f(x) = C$ 在 $I$ 上 $\Leftrightarrow f'(x) \equiv 0$。

**例题：** 证明 $x > 0$ 时，$\frac{x}{1 + x} < \ln(1 + x) < x$。  
**证明：**  
令 $f(x) = \ln x$，$\ln 1 = 0$，则 $\ln(1 + x) - \ln 1 = f'(\xi) x = \frac{x}{\xi}$（$1 < \xi < 1 + x$）。  
因 $\frac{x}{1 + x} < \frac{x}{\xi} < x$，故得证。

</ul>

## 柯西中值定理

<ul>

1. $f(x)$ 与 $F(x)$ 在 $[a, b]$ 上连续。  
2. $f(x)$ 与 $F(x)$ 在 $(a, b)$ 内可导，且 $\forall x \in (a, b)$，$F'(x) \neq 0$。  
则 $\exists \xi \in (a, b)$，使得 $\frac{f(b) - f(a)}{F(b) - F(a)} = \frac{f'(\xi)}{F'(\xi)}$。

</ul>

## 泰勒中值定理

<ul>

即带拉格朗日余项的泰勒公式。  
设 $f(x)$ 在区间 $I$ 上 $(n + 1)$ 阶可导，$x_0 \in I$，则 $\forall x \in I$，$\exists \xi \in I$ 使得：  
$$
f(x) = f(x_0) + f'(x_0)(x - x_0) + \cdots + \frac{f^{(n)}(x_0)}{n!}(x - x_0)^n + R_n(x)
$$
- **拉格朗日余项：** $R_n(x) = \frac{f^{(n+1)}(\xi)}{(n+1)!}(x - x_0)^{n+1}$，常用于证明。  
- **皮亚诺余项：** $R_n(x) = o((x - x_0)^n)$，常用于求极限，因余项较粗糙。

</ul>

</ul>

# 洛必达法则

<ul>

## 定理

<ul>

若当 $x \to a$ 或 $x \to \infty$ 时，$f(x)$ 和 $F(x)$ 都趋向 0 或无穷大，则 $\lim_{x \to a/\infty} \frac{f(x)}{F(x)}$ 可能存在，也可能不存在，称为不定式。

**定理：**  
1. 当 $x \to a$ 或 $\infty$ 时，$f(x), g(x) \to 0$ 或 $\infty$。  
2. $f'(x), g'(x)$ 在 $a$ 的某去心邻域内或 $|x| > X$ 时存在，且 $g'(x) \neq 0$。  
3. $\lim_{x \to a/\infty} \frac{f'(x)}{g'(x)}$ 存在或为 $\infty$。  
4. 则 $\lim_{x \to a/\infty} \frac{f(x)}{g(x)} = \lim_{x \to a/\infty} \frac{f'(x)}{g'(x)}$。

</ul>

## 注意事项

<ul>

1. 若 $\frac{f(x)}{g(x)}$ 不是 $\frac{0}{0}$ 或 $\frac{\infty}{\infty}$ 型，不能使用洛必达法则。  
2. 若求导后仍为 $\frac{0}{0}$ 或 $\frac{\infty}{\infty}$ 型，可继续使用。  
3. 若 $\lim_{x \to a} \frac{f'(x)}{g'(x)}$ 不存在且不为 $\infty$，不能反推 $\lim_{x \to a} \frac{f(x)}{g(x)}$ 不存在，洛必达法则失效。  
4. 洛必达法则还可变形解决 $0 \cdot \infty$、$\infty - \infty$、$1^\infty$、$\infty^0$、$0^0$ 等类型。

**示例：** $\lim_{x \to 0} \frac{x^2 \sin \frac{1}{x}}{x} = \lim_{x \to 0} x \sin \frac{1}{x} = 0$，但 $\lim_{x \to 0} \frac{d}{dx} (x^2 \sin \frac{1}{x}) / 1 = \lim_{x \to 0} (2x \sin \frac{1}{x} - \cos \frac{1}{x})$ 不存在。

</ul>

</ul>

# 泰勒公式

<ul>

非常重要，许多定义（如等价无穷小）基于泰勒公式。

## 定义

<ul>

泰勒公式用函数在某点的信息近似表达其附近取值。若函数满足一定条件，可用各阶导数构建多项式近似，即 $f(x) \approx \sum a_n x^n$。  
简单来说，泰勒公式是一个近似表达函数的公式，其增量趋向 0。  
相关延申见 [知乎回答](https://www.zhihu.com/question/25627482)。

</ul>

## 泰勒定理

<ul>

拉格朗日定理是泰勒定理特例。泰勒定理建立函数与高阶导数关系，与前三大中值定理组成四大中值定理。

### 皮亚诺余项

<ul>

设 $f(x)$ 在 $x_0$ 处 $n$ 阶可微，则：  
$$
f(x) = \sum_{k=0}^n \frac{f^{(k)}(x_0)}{k!} (x - x_0)^k + o((x - x_0)^n)
$$  
其中 $o((x - x_0)^n)$ 为皮亚诺余项。  
**缺点：**  
1. 仅定性描述余项，无法定量分析。  
2. 适用范围小。

</ul>

### 拉格朗日余项

<ul>

设 $f(x)$ 在 $x_0$ 处 $(n + 1)$ 阶可微，$x_0 \in I$，则 $\forall x \in I$，$\exists \xi \in (x_0, x)$ 使得：  
$$
f(x) = \sum_{k=0}^n \frac{f^{(k)}(x_0)}{k!} (x - x_0)^k + \frac{f^{(n+1)}(\xi)}{(n+1)!} (x - x_0)^{n+1}
$$  
**特点：**  
1. 可进行定量研究。  
2. 可整体研究。  
3. 计算量较大。  
若 $|f^{(n+1)}(x)| \leqslant M$，则 $|R_n(x)| \leqslant \frac{M}{(n+1)!} |x - x_0|^{n+1}$。

</ul>

</ul>

## 泰勒展开

<ul>

### 麦克劳林公式

<ul>

当 $x_0 = 0$ 时：  
1. $\sin x = x - \frac{x^3}{3!} + o(x^3)$  
2. $\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} + o(x^4)$  
3. $\arcsin x = x + \frac{x^3}{6} + o(x^3)$  
4. $\tan x = x + \frac{x^3}{3} + o(x^3)$  
5. $\arctan x = x - \frac{x^3}{3} + o(x^3)$  
6. $\ln(1 + x) = x - \frac{x^2}{2} + \frac{x^3}{3} + o(x^3)$  
7. $e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + o(x^3)$  
8. $(1 + x)^\alpha = 1 + \alpha x + \frac{\alpha (\alpha - 1)}{2!} x^2 + o(x^2)$

**变形示例：** $x - \sin x \sim \frac{x^3}{6}$，$x + \sin x \sim 2x$。  
**例题：** $\lim_{x \to 0} \frac{[\sin x - \sin(\sin x)] \sin x}{x^4}$  
**解：** $\sin x - \sin(\sin x) \approx \frac{x^3}{6} - \frac{(\sin x)^3}{6} \approx 0$，需更高阶展开，结果趋向 0（具体计算略）。

</ul>

### 泰勒公式计算

<ul>

1. 写出 $y = f(x)$ 的泰勒公式：$y = \sum_{n=0}^\infty \frac{f^{(n)}(x_0)}{n!} (x - x_0)^n$ 或麦克劳林公式。  
2. 通过已知公式展开为幂级数。  
3. 比较系数获取 $f^{(n)}(x_0)$。  

**例题：** 设 $y = x^3 \sin x$，求 $y^{(6)}(0)$。  
**解：**  
- $y = x^3 (x - \frac{x^3}{6} + \cdots) = x^4 - \frac{1}{6} x^6 + \cdots$  
- 比较 $\frac{y^{(6)}(0)}{6!} x^6 = -\frac{1}{6} x^6$，得 $y^{(6)}(0) = -120$。

</ul>

</ul>

## 展开幂的选择

<ul>

### $\frac{A}{B}$ 型（上下同阶）

<ul>

展开到分母或分子 $x$ 的 $k$ 次幂。  
**示例：** $\lim_{x \to 0} \frac{x - \sin x}{x^3} = \lim_{x \to 0} \frac{\frac{x^3}{6} + o(x^3)}{x^3} = \frac{1}{6}$。

</ul>

### $A - B$ 型（幂次最高）

<ul>

展开到系数不相等的最高次幂。  
**示例：** $\cos x - e^{-\frac{x^2}{2}} \approx -\frac{1}{12} x^4$，与 $a x^k$ 等价，得 $a = -\frac{1}{12}$，$k = 4$。

</ul>

</ul>

</ul>

# 函数单调性与曲线凹凸性

<ul>

## 函数单调性

<ul>

**定理：**  
1. $f(x)$ 在 $[a, b]$ 上连续，在 $(a, b)$ 内可导。  
2. 若 $f'(x) \geqslant 0$（等号仅在有限点成立），则 $f(x)$ 在 $[a, b]$ 上单调增加。  
3. 若 $f'(x) \leqslant 0$（等号仅在有限点成立），则 $f(x)$ 在 $[a, b]$ 上单调减少。

**例题：** 证明 $x > 0$ 时，$x - \frac{x^3}{6} < \sin x < x$。  
**证明：**  
- 令 $f(x) = x - \sin x$，$f(0) = 0$，$f'(x) = 1 - \cos x \geqslant 0$，则 $f(x) > 0$，即 $x > \sin x$。  
- 令 $g(x) = \sin x - x + \frac{x^3}{6}$，$g(0) = 0$，$g'(x) = \cos x - 1 + \frac{x^2}{2} \geqslant 0$，则 $g(x) > 0$，即 $\sin x > x - \frac{x^3}{6}$。

</ul>

## 曲线凹凸性与拐点

<ul>

**定义：** 若 $f(x)$ 在 $I$ 上连续，且对任意 $x_1, x_2 \in I$：  
1. $f\left(\frac{x_1 + x_2}{2}\right) < \frac{f(x_1) + f(x_2)}{2}$，则 $f(x)$ 在 $I$ 上凹。  
2. $f\left(\frac{x_1 + x_2}{2}\right) > \frac{f(x_1) + f(x_2)}{2}$，则 $f(x)$ 在 $I$ 上凸。  
**拐点：** 凹凸性改变的点。

**定理：**  
1. $f(x)$ 在 $[a, b]$ 上连续，在 $(a, b)$ 内二阶可导。  
2. 若 $f''(x) > 0$，则 $f(x)$ 在 $[a, b]$ 上凹。  
3. 若 $f''(x) < 0$，则 $f(x)$ 在 $[a, b]$ 上凸。  
**拐点条件：** 二阶导数为 0 或不存在。

</ul>

</ul>

# 函数极值与最值

<ul>

## 函数极值

<ul>

**定义：** 若 $\exists \delta > 0$，使 $\forall x \in U(x_0, \delta)$：  
- $f(x) \geqslant f(x_0)$，则 $x_0$ 为极小值点。  
- $f(x) \leqslant f(x_0)$，则 $x_0$ 为极大值点。

**必要条件：** 若 $f(x)$ 在 $x_0$ 处可导且取得极值，则 $f'(x_0) = 0$。

**第一充分条件：** 若 $f'(x_0) = 0$ 或在 $x_0$ 连续：  
1. $x < x_0$ 时 $f'(x) \geqslant 0$，$x > x_0$ 时 $f'(x) \leqslant 0$，则 $x_0$ 为极大值。  
2. $x < x_0$ 时 $f'(x) \leqslant 0$，$x > x_0$ 时 $f'(x) \geqslant 0$，则 $x_0$ 为极小值。  
3. $f'(x)$ 在 $x_0$ 处不变号，则无极值。

**第二充分条件：** 若 $f'(x_0) = 0$ 且 $f''(x_0) \neq 0$：  
1. $f''(x_0) < 0$，则极大值。  
2. $f''(x_0) > 0$，则极小值。

**第三充分条件：** 若 $f'(x_0) = f''(x_0) = \cdots = f^{(n-1)}(x_0) = 0$，$f^{(n)}(x_0) \neq 0$：  
1. $n$ 为偶数：$f^{(n)}(x_0) < 0$ 则极大值，$f^{(n)}(x_0) > 0$ 则极小值。  
2. $n$ 为奇数：无极值。

</ul>

## 函数最值

<ul>

### 连续函数闭区间最值

<ul>

1. 求 $f(x)$ 在 $(a, b)$ 内的驻点和不可导点 $x_1, x_2, \dots, x_n$。  
2. 计算 $f(x_1), \dots, f(x_n)$ 及 $f(a), f(b)$。  
3. 比较求最值。

</ul>

### 最值应用题

<ul>

1. 建立目标函数并确定定义域。  
2. 求驻点并计算值。

</ul>

</ul>

</ul>

# 函数图像绘制

<ul>

## 基本步骤

<ul>

1. 确定定义域，考察奇偶性和周期性。  
2. 求一阶导数与二阶导数，计算导数为 0 或不存在的点。  
3. 判断增减性、凹凸性，求极值与拐点。  
4. 求渐近线。  
5. 确定其他特殊点。

</ul>

## 函数渐近线

<ul>

- 若 $\lim_{x \to \infty} f(x) = A$，则 $y = A$ 为水平渐近线。  
- 若 $\lim_{x \to x_0} f(x) = \infty$，则 $x = x_0$ 为垂直渐近线。  
- 若 $\lim_{x \to \infty} \frac{f(x)}{x} = a$，$b = \lim_{x \to \infty} (f(x) - a x)$，则 $y = a x + b$ 为斜渐近线。

</ul>

</ul>

# 弧微分与曲率

<ul>

## 弧微分

<ul>

当偏移量无穷小时，$y = f(x)$ 的线段趋于直线：  
- $\mathrm{d}y = f(x + \mathrm{d}x) - f(x)$  
- $(\mathrm{d}s)^2 = (\mathrm{d}x)^2 + (\mathrm{d}y)^2$  
- $\mathrm{d}s = \sqrt{(\mathrm{d}x)^2 + (\mathrm{d}y)^2}$（弧微分）

- 对于 $y = f(x)$：$\mathrm{d}s = \sqrt{1 + \left(\frac{\mathrm{d}y}{\mathrm{d}x}\right)^2} \mathrm{d}x = \sqrt{1 + [f'(x)]^2} \mathrm{d}x$。  
- 对于参数方程 $x = \phi(t), y = \psi(t)$：$\mathrm{d}s = \sqrt{\left(\frac{\mathrm{d}x}{\mathrm{d}t}\right)^2 + \left(\frac{\mathrm{d}y}{\mathrm{d}t}\right)^2} \mathrm{d}t = \sqrt{[\phi'(t)]^2 + [\psi'(t)]^2} \mathrm{d}t$。

*图像描述：展示曲线 y = x²，标出 x, x + Δx, Δx, Δy 和弧长 Δs，趋于无穷小时变为 dx, dy, ds。*

</ul>

## 曲率

<ul>

**定义：** 曲率 $k$ 表示曲线在某点的弯曲程度，为切线方向角对弧长的转动率：  
$k = \lim_{\Delta s \to 0} \left| \frac{\Delta \alpha}{\Delta s} \right| = \left| \frac{\mathrm{d} \alpha}{\mathrm{d}s} \right|$，$\alpha$ 为切线与 $x$ 轴夹角。

**公式推导：**  
- $\mathrm{d}s = \sqrt{1 + [f'(x)]^2} \mathrm{d}x$  
- $\tan \alpha = f'(x)$，两边求导：$\sec^2 \alpha \frac{\mathrm{d} \alpha}{\mathrm{d}x} = f''(x)$  
- $\sec^2 \alpha = 1 + \tan^2 \alpha = 1 + [f'(x)]^2$  
- $\frac{\mathrm{d} \alpha}{\mathrm{d}x} = \frac{f''(x)}{1 + [f'(x)]^2}$，$\mathrm{d} \alpha = \frac{f''(x)}{1 + [f'(x)]^2} \mathrm{d}x$  
- $k = \left| \frac{\mathrm{d} \alpha}{\mathrm{d}s} \right| = \frac{|f''(x)|}{(1 + [f'(x)]^2)^{3/2}}$  
- 参数方程：$k = \frac{|x' y'' - y' x''|}{(x'^2 + y'^2)^{3/2}}$。

</ul>

## 曲率半径

<ul>

**定义：** $R = \frac{1}{k}$，为曲率圆的半径。  
*图像描述：展示曲线 L 在点 X 处的曲率圆，圆心 O，半径 R，与曲线相切于 X，切线为 T。*

</ul>

</ul>