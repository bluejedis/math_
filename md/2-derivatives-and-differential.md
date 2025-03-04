# 导数概念

<ul>

## 引例

<ul>

设 $f(x)$ 在 $x_0$ 的邻域内定义，$\alpha$ 为切线所成夹角。

$$
\tan \alpha = f'(x_0) = \lim_{x \to x_0} \frac{f(x) - f(x_0)}{x - x_0} = k
$$

导数的本质是增量比的极限。

</ul>

## 定义

<ul>

设 $y = f(x)$ 定义在区间 $I$ 上，令自变量在 $x = x_0$ 处加增量 $\Delta x$（$x_0 \in I$，$x_0 + \Delta x \in I$），则函数增量 $\Delta y = f(x_0 + \Delta x) - f(x_0)$。若 $\Delta y$ 与 $\Delta x$ 的比值在 $\Delta x \to 0$ 时极限存在，则称 $y = f(x)$ 在 $x_0$ 处可导，该极限为导数 $f'(x_0)$：

$$
f'(x_0) = \lim_{\Delta x \to 0} \frac{\Delta y}{\Delta x} = \lim_{\Delta x \to 0} \frac{f(x_0 + \Delta x) - f(x_0)}{\Delta x}
$$

以下三句等价：

1. $y = f(x)$ 在 $x_0$ 处可导。
2. $y = f(x)$ 在 $x_0$ 处导数存在。
3. $f'(x_0) = A$（$A$ 为有限数）。

**单侧导数：**

- 左导数：$f'_-(x_0) = \lim_{\Delta x \to 0^-} \frac{f(x_0 + \Delta x) - f(x_0)}{\Delta x}$
- 右导数：$f'_+(x_0) = \lim_{\Delta x \to 0^+} \frac{f(x_0 + \Delta x) - f(x_0)}{\Delta x}$

**可导充要条件：** 左右导数存在且相等。

**角点：** 若左右导数不相等，$x_0$ 为角点，不可导。例如 $y = |x|$ 在 $x = 0$ 处。

**无穷导数：** 若导数为无穷（如 $y = x^{1/3}$ 在 $x = 0$ 处为正无穷），考研中视为不存在。

**定理：**

- 若 $f(x)$ 为可导偶函数，则 $f'(x)$ 为奇函数。  
  **证明：** $f(-x) = f(x)$，则 $f'(-x) = \lim_{\Delta x \to 0} \frac{f(-x + \Delta x) - f(-x)}{\Delta x} = -\lim_{-\Delta x \to 0} \frac{f(x + (-\Delta x))}{-\Delta x} = -f'(x)$。
- 若 $f(x)$ 为可导奇函数，则 $f'(x)$ 为偶函数。  
  **证明：** $f(-x) = -f(x)$，则 $f'(-x) = f'(x)$（类似推导）。
- 若 $f(x)$ 为可导周期函数（周期 $T$），则 $f'(x)$ 也以 $T$ 为周期。  
  **证明：** $f(x + T) = f(x)$，则 $f'(x + T) = \lim_{\Delta x \to 0} \frac{f(x + T + \Delta x) - f(x + T)}{\Delta x} = f'(x)$。

**例题：** 设 $f(x)$ 为二阶可导、以 2 为周期的奇函数，且 $f\left(\frac{1}{2}\right) > 0$，$f'\left(\frac{1}{2}\right) > 0$，比较 $f\left(-\frac{1}{2}\right)$、$f'\left(\frac{3}{2}\right)$、$f''(0)$ 的大小。

**解：**  
- $f(x)$ 为奇函数，$f''(x)$ 也为奇函数，故 $f''(0) = 0$。  
- $f\left(-\frac{1}{2}\right) = -f\left(\frac{1}{2}\right) < 0$。  
- $f'(x)$ 为偶函数且周期为 2，$f'\left(\frac{3}{2}\right) = f'\left(\frac{3}{2} - 2\right) = f'\left(-\frac{1}{2}\right) = f'\left(\frac{1}{2}\right) > 0$。  
- 故 $f'\left(\frac{3}{2}\right) > f''(0) > f\left(-\frac{1}{2}\right)$。

**例题：** 求 $\left(x^\alpha\right)' = \alpha x^{\alpha - 1}$（$x > 0$）。

**解：**  
$$
\left(x^\alpha\right)' = \lim_{\Delta x \to 0} \frac{(x + \Delta x)^\alpha - x^\alpha}{\Delta x} = \lim_{\Delta x \to 0} \frac{x^\alpha \left[\left(1 + \frac{\Delta x}{x}\right)^\alpha - 1\right]}{\Delta x} = \alpha x^{\alpha - 1}
$$

</ul>

## 导数的几何意义

<ul>

导数 $f'(x_0)$ 是曲线 $y = f(x)$ 在点 $(x_0, f(x_0))$ 处切线的斜率。

- **切线方程：** $y - y_0 = f'(x_0)(x - x_0)$  
- **法线方程：** $y - y_0 = -\frac{1}{f'(x_0)}(x - x_0)$

</ul>

## 可导与连续的关系

<ul>

**定理：** 可导 $\Rightarrow$ 连续，连续不一定可导。

**证明：**  
若可导，$\lim_{\Delta x \to 0} [f(x + \Delta x) - f(x)] = \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x} \cdot \Delta x = A \cdot 0 = 0$，故连续。

**定理：** 若 $f(x)$ 在 $x_0$ 处连续，且 $\lim_{x \to x_0} \frac{f(x)}{x - x_0} = A$，则 $f(x_0) = 0$ 且 $f'(x_0) = A$。

**证明：**  
因连续，$f(x_0) = \lim_{x \to x_0} f(x) = \lim_{x \to x_0} \frac{f(x)}{x - x_0} (x - x_0) = A \cdot 0 = 0$。  
又 $f'(x_0) = \lim_{x \to x_0} \frac{f(x) - f(x_0)}{x - x_0} = \lim_{x \to x_0} \frac{f(x)}{x - x_0} = A$。

**例：** 若 $\lim_{x \to 1} \frac{f(x)}{x - 1} = 2$ 且 $f(x)$ 连续，则 $f(1) = 0$，$f'(1) = 2$。

</ul>

</ul>

# 函数求导法则

<ul>

## 四则运算

<ul>

若函数可导：

1. **和差导数：** $[u(x) \pm v(x)]' = u'(x) \pm v'(x)$  
2. **积导数：** $[u(x) v(x)]' = u'(x) v(x) + u(x) v'(x)$  
   $[u(x) v(x) w(x)]' = u'(x) v(x) w(x) + u(x) v'(x) w(x) + u(x) v(x) w'(x)$  
3. **商导数：** $\left[\frac{u(x)}{v(x)}\right]' = \frac{u'(x) v(x) - u(x) v'(x)}{[v(x)]^2}$（$v(x) \neq 0$）

**证明（积导数）：**  
$$
(uv)' = \lim_{\Delta x \to 0} \frac{u(x + \Delta x) v(x + \Delta x) - u(x) v(x)}{\Delta x} = u'(x) v(x) + u(x) v'(x)
$$

</ul>

## 反函数导数

<ul>

**定理：** 若 $y = f(x)$ 可导且 $f'(x) \neq 0$，则反函数 $x = \varphi(y)$ 存在且 $\frac{dx}{dy} = \frac{1}{\frac{dy}{dx}}$。

**例题：** 求 $y = \arcsin x$（$x \in (-1, 1)$）和 $y = \arctan x$ 的导数。

**解：**  
- $y = \arcsin x \Rightarrow x = \sin y \Rightarrow \frac{d}{dx} \arcsin x = \frac{1}{\cos y} = \frac{1}{\sqrt{1 - x^2}}$  
- $y = \arctan x \Rightarrow x = \tan y \Rightarrow \frac{d}{dx} \arctan x = \frac{1}{\sec^2 y} = \frac{1}{1 + x^2}$

**二阶反函数导数：**  
$$
f''(x) = -\frac{\varphi''(y)}{[\varphi'(y)]^3}
$$

**例题：** 设 $y = f(x)$ 的反函数为 $x = \varphi(y)$，且 $f(x) = \int_1^{2x} e^{t^2} \, dt + 1$，求 $\varphi''(1)$。

**解：**  
- $f'(x) = 2 e^{4x^2}$，$f''(x) = 16x e^{4x^2}$  
- $y = 1 \Rightarrow x = \frac{1}{2}$  
- $\varphi''(1) = -\frac{f''\left(\frac{1}{2}\right)}{\left[f'\left(\frac{1}{2}\right)\right]^3} = -\frac{1}{e^2}$

</ul>

## 复合函数的导数

<ul>

**定理：** 若 $u = g(x)$ 可导，$y = f(u)$ 在 $u = g(x)$ 处可导，则 $[f(g(x))]' = f'(g(x)) g'(x)$。

**例题：** 设 $f(x) = \prod_{n=1}^{100} \left( \tan \frac{\pi x^n}{4} - n \right)$，求 $f'(1)$。

**解：**  
令 $g(x) = \prod_{n=2}^{100} \left( \tan \frac{\pi x^n}{4} - n \right)$，则 $f(x) = \left( \tan \frac{\pi x}{4} - 1 \right) g(x)$。  
$$
f'(x) = \left( \sec^2 \frac{\pi x}{4} \cdot \frac{\pi}{4} \right) g(x) + \left( \tan \frac{\pi x}{4} - 1 \right) g'(x)
$$
当 $x = 1$，$\tan \frac{\pi}{4} - 1 = 0$，故 $f'(1) = \frac{\pi}{4} g(1)$。  
$$
g(1) = \prod_{n=2}^{100} (-n) = (-1)^{99} \cdot 99!
$$
故 $f'(1) = -\frac{\pi}{4} \cdot 99!$

</ul>

## 分段函数的导数

<ul>

设 $f(x) = \begin{cases} f_1(x), & x \geqslant x_0 \\ f_2(x), & x < x_0 \end{cases}$。  
- 在 $x > x_0$，$f'(x) = f_1'(x)$  
- 在 $x < x_0$，$f'(x) = f_2'(x)$  
- 在 $x = x_0$，需判断 $f'_+(x_0) \overset{?}{=} f'_-(x_0)$

</ul>

## 对数求导法

<ul>

对于多项相乘、相除、开方、乘方的式子，先取对数再求导：  
1. $\ln |y| = \ln |f(x)|$  
2. $\frac{y'}{y} = [\ln |f(x)|]' \Rightarrow y' = y [\ln |f(x)|]'$

**例题：** 求 $y = \sqrt[3]{\frac{(x + 1)(2x - 1)^2}{(4 - 3x)^5}}$ 的导数。

**解：**  
$$
\ln |y| = \frac{1}{3} [\ln |x + 1| + 2 \ln |2x - 1| - 5 \ln |4 - 3x|]
$$
$$
\frac{y'}{y} = \frac{1}{3} \left( \frac{1}{x + 1} + \frac{4}{2x - 1} + \frac{15}{4 - 3x} \right)
$$
$$
y' = \frac{1}{3} \left( \frac{1}{x + 1} + \frac{4}{2x - 1} + \frac{15}{4 - 3x} \right) y
$$

</ul>

## 幂指函数求导法

<ul>

对于 $u(x)^{v(x)}$（$u(x) > 0, u(x) \neq 1$），可使用 $u(x)^{v(x)} = e^{v(x) \ln u(x)}$，  
$$
[u(x)^{v(x)}]' = u(x)^{v(x)} \left[ v'(x) \ln u(x) + v(x) \cdot \frac{u'(x)}{u(x)} \right]
$$

**例题：** 求 $y = x^x$（$x > 0$）的导数。

**解：**  
$$
y = x^x = e^{x \ln x} \Rightarrow y' = x^x (\ln x + 1)
$$

**例题：** 求 $y = x^{\frac{1}{x}}$（$x > 0$）的整数最大值。

**解：**  
$$
y' = x^{\frac{1}{x}} \cdot \frac{1 - \ln x}{x^2}
$$
驻点 $x = e$ 时最大，$\lim_{x \to 0^+} y = 0$，$\lim_{x \to +\infty} y = 1$。比较 $\sqrt{2}$ 和 $\sqrt[3]{3}$，$(\sqrt{2})^6 = 8 < 9 = (\sqrt[3]{3})^6$，故最大整数值为 $\sqrt[3]{3}$。

</ul>

</ul>

# 高阶导数

<ul>

## 定义

<ul>

**高阶导数：**  
$$
f^{(n)}(x_0) = \lim_{\Delta x \to 0} \frac{f^{(n-1)}(x_0 + \Delta x) - f^{(n-1)}(x_0)}{\Delta x}
$$
若 $f^{(n-1)}(x)$ 在 $x_0$ 邻域内定义。

**常见高阶导数：**  
- $(e^x)^{(n)} = e^x$  
- $(\sin x)^{(n)} = \sin\left(x + n \frac{\pi}{2}\right)$  
- $(\cos x)^{(n)} = \cos\left(x + n \frac{\pi}{2}\right)$  
- $(\ln(1 + x))^{(n)} = (-1)^{n-1} \frac{(n-1)!}{(1 + x)^n}$

**定理：**  
- $(u \pm v)^{(n)} = u^{(n)} \pm v^{(n)}$  
- **莱布尼兹公式：** $(uv)^{(n)} = \sum_{k=0}^n C_n^k u^{(n - k)} v^{(k)}$

</ul>

## 归纳法

<ul>

**例题：** 求 $\sin x$ 的 $n$ 阶导数。

**解：**  
$$
(\sin x)' = \cos x = \sin\left(x + \frac{\pi}{2}\right), \quad (\sin x)'' = \sin\left(x + \pi\right), \quad \dots \quad (\sin x)^{(n)} = \sin\left(x + n \frac{\pi}{2}\right)
$$

</ul>

## 莱布尼茨公式

<ul>

**定义：** $(uv)^{(n)} = \sum_{k=0}^n C_n^k u^{(n - k)} v^{(k)}$

**例题：** 已知 $y = e^x \cos x$，求 $y^{(4)}$。

**解：**  
$$
y^{(4)} = e^x \cos x + 4 e^x (-\sin x) + 6 e^x (-\cos x) + 4 e^x \sin x + e^x \cos x = -4 e^x \cos x
$$

</ul>

</ul>

# 隐函数与参数方程的导数以及相关变化率

<ul>

## 隐函数求导法

<ul>

设 $y = y(x)$ 由 $F(x, y) = 0$ 确定，求导：  
1. 对方程两边对 $x$ 求导。  
2. 解方程求 $y'$。

**例题：** 设 $y = y(x)$ 由 $\sin(xy) = \ln \frac{x + e}{y} + 1$ 确定，求 $y'(0)$。

**解：**  
$$
\cos(xy)(y + x y') = \frac{1}{x + e} - \frac{y'}{y}
$$
代入 $x = 0$，$y = e^2$：  
$$
e^2 = \frac{1}{e} - \frac{y'(0)}{e^2} \Rightarrow y'(0) = e - e^4
$$

</ul>

## 参数方程函数导数

<ul>

**定理：** 设 $y = y(x)$ 由 $\begin{cases} x = \varphi(t) \\ y = \psi(t) \end{cases}$ 确定，$\varphi'(t) \neq 0$，则：  
- 一阶导数：$\frac{dy}{dx} = \frac{\psi'(t)}{\varphi'(t)}$  
- 二阶导数：$\frac{d^2 y}{dx^2} = \frac{\frac{d}{dt} \left( \frac{dy}{dx} \right)}{\varphi'(t)}$

**例题：** 设 $y = y(x)$ 由 $\begin{cases} x = \sin t \\ y = t \sin t + \cos t \end{cases}$ 确定，求 $\frac{d^2 y}{dx^2} \big|_{t = \frac{\pi}{4}}$。

**解：**  
$$
\frac{dy}{dx} = \frac{t \cos t}{\cos t} = t, \quad \frac{d^2 y}{dx^2} = \frac{1}{\cos t}
$$
当 $t = \frac{\pi}{4}$，$\frac{d^2 y}{dx^2} = \sqrt{2}$。

</ul>

## 相关变化率

<ul>

若 $x = x(t)$，$y = y(t)$ 可导，变量 $x, y$ 间有关系，则 $\frac{dx}{dt}$ 与 $\frac{dy}{dt}$ 间有相关变化率。

</ul>

</ul>

# 函数微分

<ul>

## 定义

<ul>

设正方形边长 $x$ 变化 $\Delta x$，面积变化 $\Delta S = 2x \Delta x + (\Delta x)^2$。当 $\Delta x \to 0$，$\Delta S \approx 2x \Delta x$，定义微分 $dS = 2x \, dx$。

**一般定义：** 若 $\Delta y = f(x_0 + \Delta x) - f(x_0) = A \Delta x + o(\Delta x)$，则 $dy = A \Delta x = f'(x_0) \, dx$。

**可微与可导：** 可导 $\Leftrightarrow$ 可微。

</ul>

## 基本运算

<ul>

### 四则运算

<ul>

1. **和差微分：** $d[ku(x) \pm lv(x)] = k \, du(x) \pm l \, dv(x)$  
2. **积微分：** $d[u(x) v(x)] = u(x) \, dv(x) + v(x) \, du(x)$  
3. **商微分：** $d\left[\frac{u(x)}{v(x)}\right] = \frac{v(x) \, du(x) - u(x) \, dv(x)}{[v(x)]^2}$  
4. **复合函数微分：** $\frac{du}{dx} = \frac{du}{dy} \cdot \frac{dy}{dx}$

</ul>

### 微分形式不变性

<ul>

**定义：** 设 $y = f(u)$，$u = g(x)$ 可微，则 $dy = f'(u) \, du = f'(g(x)) g'(x) \, dx$。

**例题：** 设 $y = e^{\sin(\ln x)}$，求 $dy$。

**解：**  
$$
dy = e^{\sin(\ln x)} \cdot \cos(\ln x) \cdot \frac{1}{x} \, dx
$$

</ul>

</ul>

</ul>

# 基本求导公式

<ul>

## 对幂指函数

<ul>

| 原函数       | 导函数          | 原函数       | 导函数          |
|--------------|-----------------|--------------|-----------------|
| $C$          | $0$             | $n^x$        | $n^x \ln n$     |
| $\log_a x$   | $\frac{1}{x \ln a}$ | $\ln x$      | $\frac{1}{x}$  |
| $x^n$        | $n x^{n-1}$     | $\sqrt[n]{x}$ | $\frac{x^{-\frac{n-1}{n}}}{n}$ |
| $\frac{1}{x^n}$ | $-\frac{n}{x^{n+1}}$ |              |                 |

</ul>

## 三角与反三角函数

<ul>

| 原函数       | 导函数          | 原函数       | 导函数          |
|--------------|-----------------|--------------|-----------------|
| $\sin x$     | $\cos x$        | $\cos x$     | $-\sin x$       |
| $\tan x$     | $\sec^2 x$      | $\cot x$     | $-\csc^2 x$    |
| $\sec x$     | $\sec x \tan x$ | $\csc x$     | $-\csc x \cot x$|
| $\arcsin x$  | $\frac{1}{\sqrt{1 - x^2}}$ | $\arccos x$  | $-\frac{1}{\sqrt{1 - x^2}}$ |
| $\arctan x$  | $\frac{1}{1 + x^2}$ | $\text{arccot}\,x$ | $-\frac{1}{1 + x^2}$ |
| $\text{arcsec}\,x$ | $\frac{1}{x \sqrt{x^2 - 1}}$ | $\text{arccsc}\,x$ | $-\frac{1}{x \sqrt{x^2 - 1}}$ |

</ul>

## 双曲与反双曲函数

<ul>

- $\sinh x = \frac{e^x - e^{-x}}{2}$  
- $\cosh x = \frac{e^x + e^{-x}}{2}$  
- $\tanh x = \frac{\sinh x}{\cosh x}$  

| 原函数       | 导函数          | 原函数       | 导函数          |
|--------------|-----------------|--------------|-----------------|
| $\sinh x$    | $\cosh x$       | $\cosh x$    | $\sinh x$       |
| $\tanh x$    | $\text{sech}^2 x$ | $\text{arcsinh}\, x$ | $\frac{1}{\sqrt{x^2 + 1}}$ |
| $\text{arccosh}\, x$ | $\frac{1}{\sqrt{x^2 - 1}}$ | $\text{arctanh}\, x$ | $\frac{1}{1 - x^2}$ |

</ul>

</ul>