# 二重积分

<ul>

## 概念

<ul>

### 几何背景

<ul>

二重积分的几何背景是曲顶柱体的体积。定积分通过极限思想求解了二维平面曲边梯形的面积，类似地，二重积分 $\iint_D f(x,y) \, \mathrm{d}\sigma$ 用于求解曲顶柱体的体积。

被积函数 $f(x,y)$ 作为曲顶柱体在点 $(x,y)$ 处柱体微元的高度，底面积 $\mathrm{d}\sigma > 0$ 乘以高度 $f(x,y)$ 得到小柱体体积。将所有 $D$ 上的柱体相加即为整个曲顶柱体的体积。

</ul>

### 性质

<ul>

- **求区域面积：** $\iint_D 1 \cdot \mathrm{d}\sigma = \iint_D \mathrm{d}\sigma = A$，其中 $A$ 为 $D$ 的面积。
- **可积函数必有界：** 当 $f(x,y)$ 在有界闭区域 $D$ 上可积时，$f(x,y)$ 在 $D$ 上必有界。
- **积分线性性质：** $k_1, k_2$ 为常数，则 $\iint_D [k_1 f(x,y) \pm k_2 g(x,y)] \, \mathrm{d}\sigma = k_1 \iint_D f(x,y) \, \mathrm{d}\sigma \pm k_2 \iint_D g(x,y) \, \mathrm{d}\sigma$。
- **积分可加性：** 当 $f(x,y)$ 在有界闭区域 $D$ 上可积，且 $D = D_1 \cup D_2$，$D_1 \cap D_2 = \varnothing$，则 $\iint_D f(x,y) \, \mathrm{d}\sigma = \iint_{D_1} f(x,y) \, \mathrm{d}\sigma + \iint_{D_2} f(x,y) \, \mathrm{d}\sigma$。
- **积分保号性：** 当 $f(x,y), g(x,y)$ 在有界闭区域 $D$ 上可积，若在 $D$ 上 $f(x,y) \leqslant g(x,y)$，则 $\iint_D f(x,y) \, \mathrm{d}\sigma \leqslant \iint_D g(x,y) \, \mathrm{d}\sigma$，特别地 $\left| \iint_D f(x,y) \, \mathrm{d}\sigma \right| \leqslant \iint_D |f(x,y)| \, \mathrm{d}\sigma$。
- **二重积分估值定理：** 设 $M, m$ 分别为 $f(x,y)$ 在有界闭区域 $D$ 上的最大值和最小值，$A$ 为 $D$ 的面积，则 $m A \leqslant \iint_D f(x,y) \, \mathrm{d}\sigma \leqslant M A$。
- **二重积分中值定理：** 设函数 $f(x,y)$ 在有界闭区域 $D$ 上连续，$A$ 为 $D$ 的面积，则在 $D$ 上至少存在一点 $(\xi, \eta)$ 使得 $\iint_D f(x,y) \, \mathrm{d}\sigma = f(\xi, \eta) A$。

**例题：** 设 $I_1 = \iint_D \cos \sqrt{x^2 + y^2} \, \mathrm{d}\sigma$，$I_2 = \iint_D \cos (x^2 + y^2) \, \mathrm{d}\sigma$，$I_3 = \iint_D \cos (x^2 + y^2)^2 \, \mathrm{d}\sigma$，其中 $D = \{(x,y) \mid x^2 + y^2 \leqslant 1\}$，则()。  
A. $I_3 > I_2 > I_1$  
B. $I_1 > I_2 > I_3$  
C. $I_2 > I_1 > I_3$  
D. $I_3 > I_1 > I_2$  

**解：** 令 $x^2 + y^2 = t$，则 $0 < t \leqslant 1$，所以 $1 \geqslant \sqrt{t} \geqslant t \geqslant t^2 \geqslant 0$。由于 $\cos x$ 单调递减，$I_3 > I_2 > I_1$，选 A。

</ul>

### 对称性

<ul>

#### 普通对称性

<ul>

设 $D$ 关于 $y$ 轴对称，$I = \iint_D f(x,y) \, \mathrm{d}\sigma$，将 $D$ 分为对称的两部分 $D_1$ 和 $D_2$，则：  
- 若 $f(x,y) = f(-x,y)$，$I = 2 \iint_{D_1} f(x,y) \, \mathrm{d}\sigma$  
- 若 $f(x,y) = -f(-x,y)$，$I = 0$  
关于 $x$ 轴对称同理。

</ul>

#### 轮换对称性

<ul>

若 $xy$ 对调后区域 $D$ 不变或关于 $y = x$ 对称，则 $\iint_D f(x,y) \, \mathrm{d}x \mathrm{d}y = \iint_D f(y,x) \, \mathrm{d}y \mathrm{d}x$。类似一元函数积分的不变性 $\int_a^b f(x) \, \mathrm{d}x = \int_a^b f(y) \, \mathrm{d}y$。

**例题：** 设区域 $D = \{(x,y) \mid x^2 + y^2 \leqslant 1, x \geqslant 0, y \geqslant 0\}$，$f(x)$ 在 $D$ 上为正值连续函数，$a, b$ 为常数，求 $I = \iint_D \frac{a \sqrt{f(x)} + b \sqrt{f(y)}}{\sqrt{f(x)} + \sqrt{f(y)}} \, \mathrm{d}\sigma$。  
**解：** 由于 $D$ 关于 $y = x$ 对称，利用轮换对称性：  
$I = \iint_D \frac{a \sqrt{f(y)} + b \sqrt{f(x)}}{\sqrt{f(y)} + \sqrt{f(x)}} \, \mathrm{d}\sigma$  
$2I = \iint_D \left( \frac{a \sqrt{f(x)} + b \sqrt{f(y)}}{\sqrt{f(x)} + \sqrt{f(y)}} + \frac{a \sqrt{f(y)} + b \sqrt{f(x)}}{\sqrt{f(y)} + \sqrt{f(x)}} \right) \mathrm{d}\sigma = \iint_D (a + b) \, \mathrm{d}\sigma = (a + b) \frac{\pi}{4}$  
故 $I = \frac{a + b}{8} \pi$。

</ul>

</ul>

</ul>

## 计算

<ul>

### 直角坐标系

<ul>

后积先定限，先内画条线，先交写下限，后交写上限。  
二重积分需化为累次积分，求解上下限。

#### $X$ 型区域

<ul>

$\sigma = \{(x,y) \mid a \leqslant x \leqslant b, \psi(x) \leqslant y \leqslant \phi(x)\}$（上下型区域）  
$\iint_D f(x,y) \, \mathrm{d}\sigma = \int_a^b \mathrm{d}x \int_{\psi(x)}^{\phi(x)} f(x,y) \, \mathrm{d}y$  
*图像描述：$X$ 型区域底部由 $\phi(x)$ 和 $\psi(x)$ 上下界定，$x$ 从 $a$ 到 $b$，横截面面积 $S(x) = \int_{\psi(x)}^{\phi(x)} f(x,y) \, \mathrm{d}y$，体积 $V = \int_a^b S(x) \, \mathrm{d}x$。*

</ul>

#### $Y$ 型区域

<ul>

$\sigma = \{(x,y) \mid c \leqslant y \leqslant d, \psi(y) \leqslant x \leqslant \phi(y)\}$（左右型区域）  
$\iint_D f(x,y) \, \mathrm{d}\sigma = \int_c^d \mathrm{d}y \int_{\psi(y)}^{\phi(y)} f(x,y) \, \mathrm{d}x$  
*图像描述：$Y$ 型区域左右由 $\phi(y)$ 和 $\psi(y)$ 界定，$y$ 从 $c$ 到 $d$。*

</ul>

#### 区域类型选择

<ul>

- 若上下为两条曲线，则为 $X$ 型。  
- 若左右为两条曲线，则为 $Y$ 型。  
- 若同一方向有不同表达式，则从另一方向分割求积分。

</ul>

</ul>

### 极坐标系

<ul>

根据极点与区域 $D$ 的位置关系：  
1. **极点 $O$ 在 $D$ 外部：** $\iint_D f(x,y) \, \mathrm{d}\sigma = \int_\alpha^\beta \mathrm{d}\theta \int_{r_1(\theta)}^{r_2(\theta)} f(r \cos \theta, r \sin \theta) r \, \mathrm{d}r$  
2. **极点 $O$ 在 $D$ 边界上：** $\iint_D f(x,y) \, \mathrm{d}\sigma = \int_\alpha^\beta \mathrm{d}\theta \int_0^{r(\theta)} f(r \cos \theta, r \sin \theta) r \, \mathrm{d}r$  
3. **极点 $O$ 在 $D$ 内部：** $\iint_D f(x,y) \, \mathrm{d}\sigma = \int_0^{2\pi} \mathrm{d}\theta \int_0^{r(\theta)} f(r \cos \theta, r \sin \theta) r \, \mathrm{d}r$  
微元面积 $\mathrm{d}\sigma = r \, \mathrm{d}r \mathrm{d}\theta$，通常先积 $r$ 后积 $\theta$。

</ul>

### 极坐标系与直角坐标系选择

<ul>

- 若被积函数为 $f(x^2 + y^2)$、$f\left(\frac{y}{x}\right)$、$f\left(\frac{x}{y}\right)$ 等形式，或积分区域为圆或圆的一部分，优先使用极坐标系。

</ul>

### 极直互化

<ul>

极坐标转直角坐标：$x = r \cos \theta$，$y = r \sin \theta$。

**例题：** 设 $D = \{(x,y) \mid x^2 + y^2 \leqslant R^2\}$，计算 $\iint_D \left( \frac{x^2}{a^2} + \frac{y^2}{b^2} \right) \mathrm{d}x \mathrm{d}y$。  
**解：** 利用积分变量对称性：  
$I = \iint_D \left( \frac{x^2}{a^2} + \frac{y^2}{b^2} \right) \mathrm{d}x \mathrm{d}y = \iint_D \left( \frac{y^2}{a^2} + \frac{x^2}{b^2} \right) \mathrm{d}x \mathrm{d}y$  
$2I = \left( \frac{1}{a^2} + \frac{1}{b^2} \right) \iint_D (x^2 + y^2) \mathrm{d}\sigma$  
$I = \frac{1}{2} \left( \frac{1}{a^2} + \frac{1}{b^2} \right) \int_0^{2\pi} \mathrm{d}\theta \int_0^R r^2 \cdot r \, \mathrm{d}r = \frac{\pi R^4}{4} \left( \frac{1}{a^2} + \frac{1}{b^2} \right)$

**例题：** 计算 $I = \int_0^1 \mathrm{d}x \int_{1-x}^{\sqrt{1-x^2}} \frac{x + y}{x^2 + y^2} \mathrm{d}y$。  
**解：** $D$ 为第一象限圆的一部分，转换为极坐标：  
$\theta \in (0, \frac{\pi}{2})$，下限 $r = \frac{1}{\cos \theta + \sin \theta}$（由 $x + y = 1$），上限 $r = 1$（由 $x^2 + y^2 = 1$）。  
$I = \int_0^{\frac{\pi}{2}} \mathrm{d}\theta \int_{\frac{1}{\cos \theta + \sin \theta}}^1 (\cos \theta + \sin \theta) r \cdot \frac{1}{r} \, \mathrm{d}r = \int_0^{\frac{\pi}{2}} (\cos \theta + \sin \theta - 1) \, \mathrm{d}\theta = 2 - \frac{\pi}{2}$

</ul>

### 积分次序

<ul>

选择积分次序以简化计算，避免无法求解的原函数。常见无法用初等函数表示的原函数：$\frac{\sin x}{x}$、$\frac{\cos x}{x}$、$\frac{\tan x}{x}$、$\frac{e^x}{x}$、$\sin x^2$、$\cos x^2$、$\tan x^2$、$e^{ax^2 + bx + c}$、$\frac{1}{\ln x}$ 等。

**例题：** 计算 $I = \int_1^2 \mathrm{d}x \int_{\sqrt{x}}^x \sin \frac{\pi x}{2y} \mathrm{d}y + \int_2^4 \mathrm{d}x \int_{\sqrt{x}}^2 \sin \frac{\pi x}{2y} \mathrm{d}y$。  
**解：** 积分区域 $D$ 由 $\sqrt{x}$、$x$、$2$ 围成，交换积分次序：  
$I = \iint_D \sin \frac{\pi x}{2y} \mathrm{d}\sigma = \int_1^2 \mathrm{d}y \int_y^{y^2} \sin \frac{\pi x}{2y} \mathrm{d}x = \int_1^2 \frac{2y}{\pi} \left( -\cos \frac{\pi y}{2} + \cos \frac{\pi}{2} \right) \mathrm{d}y = \frac{4}{\pi^3} (2 + \pi)$

</ul>

### 二重积分处理一元积分

<ul>

**例题：** 设 $f(x) = \int_x^1 \sin (\pi u^2) \, \mathrm{d}u$，求 $\int_0^1 f(x) \, \mathrm{d}x$。  
**解：**  
$\int_0^1 f(x) \, \mathrm{d}x = \int_0^1 \mathrm{d}x \int_x^1 \sin (\pi u^2) \, \mathrm{d}u = \int_0^1 \mathrm{d}u \int_0^u \sin (\pi u^2) \, \mathrm{d}x = \int_0^1 u \sin (\pi u^2) \, \mathrm{d}u = \frac{1}{\pi}$

**例题：** 利用广义二重积分求 $\int_0^{+\infty} e^{-x^2} \, \mathrm{d}x$。  
**解：**  
$I^2 = \left( \int_0^{+\infty} e^{-x^2} \, \mathrm{d}x \right)^2 = \int_0^{+\infty} \int_0^{+\infty} e^{-x^2 - y^2} \, \mathrm{d}x \mathrm{d}y$  
转换为极坐标：$I^2 = \int_0^{\frac{\pi}{2}} \mathrm{d}\theta \int_0^{+\infty} e^{-r^2} r \, \mathrm{d}r = \frac{\pi}{2}$，故 $I = \frac{\sqrt{\pi}}{2}$

</ul>

</ul>

## 二重积分应用

<ul>

### 体积

<ul>

</ul>

### 形心公式

<ul>

对于直角坐标系和参数方程：  
$\overline{x} = \frac{\iint_D x \, \mathrm{d}\sigma}{\iint_D \mathrm{d}\sigma} = \frac{\int x(t) y(t) x'(t) \, \mathrm{d}t}{\int y(t) x'(t) \, \mathrm{d}t}$，$\overline{y} = \frac{\iint_D y \, \mathrm{d}\sigma}{\iint_D \mathrm{d}\sigma} = \frac{\int y(t)^2 x'(t) \, \mathrm{d}t}{2 \int y(t) x'(t) \, \mathrm{d}t}$

</ul>

</ul>

</ul>

# 三重积分

<ul>

## 概念

<ul>

三重积分被积函数 $f(x,y,z)$ 定义在三维空间 $\Omega$ 上，用于求解四维空间图形的体积（抽象），常用于质量计算。

### 定义

<ul>

设 $f(x,y,z)$ 定义在有界闭区域 $\Omega$ 上，将 $\Omega$ 划分为 $n$ 个子域 $\Delta v_i$，取 $\lambda = \max \{\Delta v_i\}$，若 $\lim_{\lambda \to 0} \sum_{i=1}^n f(\alpha_i, \beta_i, \gamma_i) \Delta v_i$ 存在，称为 $f(x,y,z)$ 在 $\Omega$ 上的三重积分 $\iiint_\Omega f(x,y,z) \, \mathrm{d}v$。

</ul>

### 性质

<ul>

- **空间区域体积：** $\iiint_\Omega 1 \, \mathrm{d}v = V$，$V$ 为 $\Omega$ 的体积  
- **可积函数必有界：** $f(x,y,z)$ 在 $\Omega$ 上可积 $\Rightarrow$ 在 $\Omega$ 上有界  
- **积分线性：** $\iiint_\Omega [k_1 f \pm k_2 g] \, \mathrm{d}v = k_1 \iiint_\Omega f \, \mathrm{d}v \pm k_2 \iiint_\Omega g \, \mathrm{d}v$  
- **积分可加性：** $\iiint_\Omega f \, \mathrm{d}v = \iiint_{\Omega_1} f \, \mathrm{d}v + \iiint_{\Omega_2} f \, \mathrm{d}v$，若 $\Omega = \Omega_1 \cup \Omega_2$，$\Omega_1 \cap \Omega_2 = \varnothing$  
- **积分保号性：** 若 $f \leqslant g$，则 $\iiint_\Omega f \, \mathrm{d}v \leqslant \iiint_\Omega g \, \mathrm{d}v$，且 $\left| \iiint_\Omega f \, \mathrm{d}v \right| \leqslant \iiint_\Omega |f| \, \mathrm{d}v$  
- **三重积分估值定理：** $m V \leqslant \iiint_\Omega f \, \mathrm{d}v \leqslant M V$，$V$ 为 $\Omega$ 体积，$m, M$ 为 $f$ 最小、最大值  
- **三重积分中值定理：** 存在 $(\xi, \eta, \zeta) \in \Omega$ 使 $\iiint_\Omega f \, \mathrm{d}v = f(\xi, \eta, \zeta) V$

</ul>

### 对称性

<ul>

#### 普通对称性

<ul>

若 $\Omega$ 关于 $yOz$ 面对称，$\iiint_\Omega f(x,y,z) \, \mathrm{d}v = \begin{cases} 2 \iiint_{\Omega_1} f(x,y,z) \, \mathrm{d}v, & f(x,y,z) = f(-x,y,z) \\ 0, & f(x,y,z) = -f(-x,y,z) \end{cases}$，$\Omega_1$ 为 $\Omega$ 在 $yOz$ 面前面的部分。

</ul>

#### 轮换对称性

<ul>

若 $x$ 与 $y$ 对调后 $\Omega$ 不变，则 $\iiint_\Omega f(x,y,z) \, \mathrm{d}v = \iiint_\Omega f(y,x,z) \, \mathrm{d}v$。

</ul>

</ul>

</ul>

## 计算

<ul>

### 基础方法

<ul>

#### 直角坐标系

<ul>

$\mathrm{d}v = \mathrm{d}x \mathrm{d}y \mathrm{d}z$，微元为长方体。

##### 先一后二法

<ul>

先积 $z$ 后积 $xy$（投影穿线法）：  
$\iiint_\Omega f(x,y,z) \, \mathrm{d}v = \iint_{D_{xy}} \mathrm{d}\sigma \int_{z_1(x,y)}^{z_2(x,y)} f(x,y,z) \, \mathrm{d}z$  
适用场合：$\Omega$ 有下曲面 $z = z_1(x,y)$、上曲面 $z = z_2(x,y)$，无侧面或侧面为柱面。

**例题：** 计算 $I = \iiint_\Omega \frac{\mathrm{d}x \mathrm{d}y \mathrm{d}z}{(1 + x + y + z)^3}$，$\Omega$ 为平面 $x=0, y=0, z=0$ 及 $x + y + z = 1$ 围成的四面体。  
**解：**  
$I = \iint_{D_{xy}} \mathrm{d}\sigma \int_0^{1 - x - y} \frac{1}{(1 + x + y + z)^3} \mathrm{d}z = \iint_{D_{xy}} \frac{1}{2} \left( \frac{1}{(1 + x + y)^2} - \frac{1}{4} \right) \mathrm{d}\sigma = \frac{1}{2} \left( \ln 2 - \frac{5}{8} \right)$

</ul>

##### 先二后一法

<ul>

先积 $xy$ 后积 $z$（定限截面法）：  
$\iiint_\Omega f(x,y,z) \, \mathrm{d}v = \int_a^b \mathrm{d}z \iint_{D_z} f(x,y,z) \, \mathrm{d}\sigma$  
适用场合：$\Omega$ 为旋转体，上下为平面，中间为曲面。

</ul>

</ul>

#### 柱面坐标系

<ul>

若 $\iint_{D_{xy}}$ 适合极坐标，设 $x = r \cos \theta$，$y = r \sin \theta$，则 $\iiint_\Omega f(x,y,z) \, \mathrm{d}x \mathrm{d}y \mathrm{d}z = \iiint_\Omega f(r \cos \theta, r \sin \theta, z) r \, \mathrm{d}r \mathrm{d}\theta \mathrm{d}z$。  
适用场合：被积函数含 $x^2 + y^2$，积分区域为圆或圆的部分。

**例题：** 计算 $\iiint_\Omega (x^2 + y^2) \, \mathrm{d}v$，$\Omega$ 为曲线 $y^2 = 2z$、$x = 0$ 绕 $z$ 轴旋转一周与 $z = 8$ 围成的区域。  
**解：** 旋转曲面 $z = \frac{x^2 + y^2}{2}$，与 $z = 8$ 围成旋转体。使用先二后一法：  
$I = \int_0^8 \mathrm{d}z \iint_{D_z} (x^2 + y^2) \, \mathrm{d}\sigma = \int_0^8 \mathrm{d}z \int_0^{2\pi} \mathrm{d}\theta \int_0^{\sqrt{2z}} r^2 \cdot r \, \mathrm{d}r = \frac{1024}{3} \pi$

</ul>

#### 球面坐标系

<ul>

**适用场合：** 被积函数含 $x^2 + y^2 + z^2$ 或 $x^2 + y^2$，积分区域为球、锥或其部分。  
**转换：** $x = r \sin \phi \cos \theta$，$y = r \sin \phi \sin \theta$，$z = r \cos \phi$，$\mathrm{d}v = r^2 \sin \phi \, \mathrm{d}r \mathrm{d}\phi \mathrm{d}\theta$。  
**例题：** 计算 $\iiint_\Omega (x^2 + y^2) \, \mathrm{d}v$，$\Omega$ 为半球 $x^2 + y^2 + z^2 = a^2$（$y \geqslant 0$）与 $xOz$ 面围成的区域。  
**解：**  
$I = \int_0^\pi \mathrm{d}\theta \int_0^\pi \mathrm{d}\phi \int_0^a (r^2 \sin^2 \phi) r^2 \sin \phi \, \mathrm{d}r = \frac{4\pi a^5}{15}$

</ul>

</ul>

### 对称性

<ul>

#### 普通对称性

<ul>

**例题：** 计算 $\iiint_\Omega e^{|z|} \, \mathrm{d}v$，$\Omega: x^2 + y^2 + z^2 \leqslant 1$。  
**解：** 利用对称性，$I = 2 \iiint_{\Omega_1} e^z \, \mathrm{d}v$，$\Omega_1: z \geqslant 0$。  
$I = 2 \int_0^1 \mathrm{d}z \iint_{D_z} e^z \, \mathrm{d}\sigma = 2 \pi \int_0^1 e^z (1 - z^2) \, \mathrm{d}z = 2\pi$

</ul>

#### 轮换对称性

<ul>

**例题：** 设 $\Omega = \{(x,y,z) \mid x^2 + y^2 + z^2 \leqslant 1\}$，求 $\iiint_\Omega z^2 \, \mathrm{d}x \mathrm{d}y \mathrm{d}z$。  
**解：** 利用轮换对称性，$I = \frac{1}{3} \iiint_\Omega (x^2 + y^2 + z^2) \, \mathrm{d}v = \frac{4\pi}{15}$

</ul>

</ul>

</ul>

</ul>

# 第一型曲线积分

<ul>

## 概念

<ul>

用于计算密度不均匀的不规则形状细线质量。

### 几何性质

<ul>

对曲线 $L$ 进行分割，近似质量 $\Delta m_i \approx \rho(\xi_i, \eta_i) \Delta S_i$，总质量 $m = \lim_{\lambda \to 0} \sum \rho(\xi_i, \eta_i) \Delta S_i = \int_L \rho(x,y) \, \mathrm{d}s$。

</ul>

### 定义

<ul>

第一型曲线积分为 $\int_L f(x,y) \, \mathrm{d}s$。

</ul>

### 性质

<ul>

- $\int_L 1 \, \mathrm{d}s = l$（弧长）  
- $\int_L f(x,y) \, \mathrm{d}s = \int_{L_1} f(x,y) \, \mathrm{d}s + \int_{L_2} f(x,y) \, \mathrm{d}s$  
- $\int_L (k_1 f \pm k_2 g) \, \mathrm{d}s = k_1 \int_L f \, \mathrm{d}s \pm k_2 \int_L g \, \mathrm{d}s$

</ul>

### 对称性

<ul>

- 若 $L$ 关于 $y$ 轴对称，$f(-x,y) = -f(x,y)$，则 $\int_L f(x,y) \, \mathrm{d}s = 0$  
- 若 $f(-x,y) = f(x,y)$，则 $\int_L f(x,y) \, \mathrm{d}s = 2 \int_{L_1} f(x,y) \, \mathrm{d}s$  
- 类似地，关于 $x$ 轴或 $y = x$ 对称。

</ul>

</ul>

## 计算

<ul>

### 基础方法

<ul>

- **显式方程：** $\int_L f(x,y) \, \mathrm{d}s = \int_a^b f[x, g(x)] \sqrt{1 + g'(x)^2} \, \mathrm{d}x$  
- **参数方程：** $\int_L f(x,y) \, \mathrm{d}s = \int_\alpha^\beta f[\phi(t), \psi(t)] \sqrt{\phi'(t)^2 + \psi'(t)^2} \, \mathrm{d}t$  

**例题：** 计算 $\oint_\Gamma |y| \, \mathrm{d}s$，$\Gamma$ 为球面 $x^2 + y^2 + z^2 = 2$ 与平面 $x = y$ 的交线。  
**解：** 利用对称性，$\oint_\Gamma |y| \, \mathrm{d}s = 4 \int_{\Gamma_1} y \, \mathrm{d}s$，$\Gamma_1$ 为第一象限部分。  
参数化：$x = \cos t$，$y = \cos t$，$z = \sqrt{2} \sin t$，$t \in (0, \frac{\pi}{2})$，$\mathrm{d}s = \sqrt{2} \, \mathrm{d}t$，  
$I = 4 \int_0^{\frac{\pi}{2}} \cos t \cdot \sqrt{2} \, \mathrm{d}t = 4\sqrt{2}$

</ul>

</ul>

</ul>

# 第一型曲面积分

<ul>

## 概念

<ul>

### 几何性质

<ul>

对曲面 $\Sigma$，质量 $\mathrm{d}m = \rho(x,y,z) \mathrm{d}s$，总质量 $m = \iint_\Sigma \rho(x,y,z) \, \mathrm{d}s$。

</ul>

### 定义

<ul>

$\iint_\Sigma f(x,y,z) \, \mathrm{d}s$ 为 $f(x,y,z)$ 在曲面 $\Sigma$ 上的面积曲面积分。

</ul>

### 性质

<ul>

- $\iint_\Sigma 1 \, \mathrm{d}s = \sigma$（曲面面积）  
- 若 $\Sigma$ 关于 $xOy$ 对称，$f(x,y,-z) = -f(x,y,z)$，则 $\iint_\Sigma f(x,y,z) \, \mathrm{d}s = 0$  
- 若 $f(x,y,-z) = f(x,y,z)$，则 $\iint_\Sigma f(x,y,z) \, \mathrm{d}s = 2 \iint_{\Sigma_1} f(x,y,z) \, \mathrm{d}s$

</ul>

</ul>

## 计算

<ul>

### 二重积分法

<ul>

1. 投影到 $xy$ 平面：$\Sigma: z = \psi(x,y)$，$(x,y) \in D_{xy}$，$\mathrm{d}s = \sqrt{1 + \left( \frac{\partial z}{\partial x} \right)^2 + \left( \frac{\partial z}{\partial y} \right)^2} \mathrm{d}\sigma$  
2. $\iint_\Sigma f(x,y,z) \, \mathrm{d}s = \iint_{D_{xy}} f[x,y,\psi(x,y)] \sqrt{1 + \left( \frac{\partial z}{\partial x} \right)^2 + \left( \frac{\partial z}{\partial y} \right)^2} \mathrm{d}\sigma$

**例题：** $I = \oiint_\Sigma (x y^2 + z) \mathrm{d}s$，$\Sigma: z = x^2 + y^2, z \leqslant 1$。  
**解：** 利用对称性，$I = \iint_\Sigma z \, \mathrm{d}s$。投影到 $xOy$，$D_{xy}: x^2 + y^2 \leqslant 1$，$\mathrm{d}s = \sqrt{1 + 4x^2 + 4y^2} \mathrm{d}\sigma$，  
$I = \iint_{D_{xy}} (x^2 + y^2) \sqrt{1 + 4(x^2 + y^2)} \mathrm{d}\sigma = \frac{10}{3} \sqrt{5} + \frac{2}{15}$

</ul>

</ul>

</ul>

# 多元积分应用

<ul>

## 几何量

<ul>

### 平面区域

<ul>

</ul>

### 空间区域

<ul>

</ul>

### 空间曲线

<ul>

</ul>

### 空间曲面

<ul>

</ul>

</ul>

## 重心与形心

<ul>

密度 $\rho$ 为常数时重心即形心。

### 空间物体

<ul>

**例题：** 设 $\Omega = \{(x,y,z) \mid x^2 + y^2 \leqslant z \leqslant 1\}$，求 $\Omega$ 形心的 $z$ 坐标 $\overline{z}$。  
**解：** $\overline{z} = \frac{\iiint_\Omega z \, \mathrm{d}v}{\iiint_\Omega \mathrm{d}v}$

</ul>

</ul>

## 转动惯量

<ul>

### 空间物体

<ul>

</ul>

### 空间曲线

<ul>

</ul>

### 空间曲面

<ul>

</ul>

</ul>

</ul>

# 第二型曲线积分

<ul>

## 概念

<ul>

### 场的概念

<ul>

空间区域 $\Omega$ 上的一种对应法则：  
- 数量场：对应数量无方向。  
- 向量场：对应数量有方向。

</ul>

### 几何性质

<ul>

对物体沿曲线 $L$ 的变力 $\vec{F}(x,y) = \{P(x,y), Q(x,y)\}$ 做功：$\mathrm{d}\omega = \vec{F} \cdot \overrightarrow{\mathrm{d}s} = P \mathrm{d}x + Q \mathrm{d}y$，$\omega = \int_L P \mathrm{d}x + Q \mathrm{d}y$。

</ul>

### 定义

<ul>

对坐标的曲线积分为 $\int_L P \mathrm{d}x + Q \mathrm{d}y$。

</ul>

### 性质

<ul>

- $\int_{L^-} P \mathrm{d}x + Q \mathrm{d}y = -\int_L P \mathrm{d}x + Q \mathrm{d}y$  
- $\int_L P \mathrm{d}x + Q \mathrm{d}y = \int_L (P \cos \alpha + Q \cos \beta) \mathrm{d}s$

</ul>

</ul>

## 计算

<ul>

### 定积分法

<ul>

- **显式：** $\int_L P \mathrm{d}x + Q \mathrm{d}y = \int_a^b [P(x, g(x)) + Q(x, g(x)) g'(x)] \mathrm{d}x$  
- **参数：** $\int_L P \mathrm{d}x + Q \mathrm{d}y = \int_\alpha^\beta [P(\phi(t), \psi(t)) \phi'(t) + Q(\phi(t), \psi(t)) \psi'(t)] \mathrm{d}t$

</ul>

### 二重积分法

<ul>

#### 格林公式

<ul>

若 $D$ 为连通区域，$L$ 为 $D$ 的正向边界，$P, Q$ 在 $D$ 上连续可偏导，则 $\oint_L P \mathrm{d}x + Q \mathrm{d}y = \iint_D \left( \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} \right) \mathrm{d}\sigma$。

</ul>

</ul>

### 路径无关积分

<ul>

当 $\frac{\partial Q}{\partial x} = \frac{\partial P}{\partial y}$ 时，$\int_L P \mathrm{d}x + Q \mathrm{d}y$ 与路径无关，可简化为 $\int_{(x_0, y_0)}^{(x_1, y_1)} P \mathrm{d}x + Q \mathrm{d}y = \int_{x_0}^{x_1} P(x, y_0) \mathrm{d}x + \int_{y_0}^{y_1} Q(x_1, y) \mathrm{d}y$，或存在 $u(x,y)$ 使 $\mathrm{d}u = P \mathrm{d}x + Q \mathrm{d}y$，$\int_L = u(x_1, y_1) - u(x_0, y_0)$。

**例题：** 已知 $\psi(x)$ 可导，$\psi(0) = 2$，$\int_L x y^2 \mathrm{d}x + \psi(x) y \mathrm{d}y$ 与路径无关，求 $\psi(x)$，并计算 $I = \int_{(1,2)}^{(2,3)} x y^2 \mathrm{d}x + \psi(x) y \mathrm{d}y$。  
**解：** 由柯西-黎曼条件 $\frac{\partial Q}{\partial x} = \frac{\partial P}{\partial y}$，$\psi'(x) y = 2x y$，$\psi'(x) = 2x$，$\psi(x) = x^2 + 2$。  
$I = \int_{(1,2)}^{(2,3)} x y^2 \mathrm{d}x + (x^2 + 2) y \mathrm{d}y = 6 + 15 = 21$

</ul>

</ul>

</ul>

# 第二型曲面积分

<ul>

## 概念

<ul>

### 向量场的通量

<ul>

对不可压缩的向量场 $\vec{v} = \{P, Q, R\}$，曲面 $\Sigma$，流量 $\mathrm{d}\phi = \vec{v} \cdot \overrightarrow{\mathrm{d}s} = P \mathrm{d}y \mathrm{d}z + Q \mathrm{d}z \mathrm{d}x + R \mathrm{d}x \mathrm{d}y$，总流量 $\iint_\Sigma P \mathrm{d}y \mathrm{d}z + Q \mathrm{d}z \mathrm{d}x + R \mathrm{d}x \mathrm{d}y$。

</ul>

### 定义

<ul>

$\iint_\Sigma P \mathrm{d}y \mathrm{d}z + Q \mathrm{d}z \mathrm{d}x + R \mathrm{d}x \mathrm{d}y$ 为在 $\Sigma$ 上的曲面积分。

</ul>

### 性质

<ul>

- $\iint_{\Sigma^-} = -\iint_\Sigma$  
- $\iint_\Sigma P \cos \alpha + Q \cos \beta + R \cos \gamma \, \mathrm{d}s$

</ul>

</ul>

## 计算

<ul>

### 二重积分法

<ul>

- $\iint_\Sigma P \mathrm{d}y \mathrm{d}z = \pm \iint_{D_{yz}} P[\phi(y,z), y, z] \mathrm{d}y \mathrm{d}z$（前正后负）  
- $\iint_\Sigma Q \mathrm{d}z \mathrm{d}x = \pm \iint_{D_{zx}} Q[x, \phi(z,x), z] \mathrm{d}z \mathrm{d}x$（右正左负）  
- $\iint_\Sigma R \mathrm{d}x \mathrm{d}y = \pm \iint_{D_{xy}} R[x, y, \phi(x,y)] \mathrm{d}x \mathrm{d}y$（上正下负）

</ul>

### 三重积分法

<ul>

#### 高斯公式

<ul>

$\oiint_\Sigma P \mathrm{d}y \mathrm{d}z + Q \mathrm{d}z \mathrm{d}x + R \mathrm{d}x \mathrm{d}y = \iiint_\Omega \left( \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} + \frac{\partial R}{\partial z} \right) \mathrm{d}v$  
**例题：** $I = \iint_\Sigma y z \mathrm{d}z \mathrm{d}x + 2 \mathrm{d}x \mathrm{d}y$，$\Sigma$ 为 $x^2 + y^2 + z^2 = 4$ 的 $xOy$ 面以上的部分。  
**解：** $I = \oiint_{\Sigma + \Sigma_0} - \iint_{\Sigma_0}$，$\oiint_{\Sigma + \Sigma_0} = 4\pi$，$\iint_{\Sigma_0} = -8\pi$，$I = 12\pi$

</ul>

</ul>

</ul>

</ul>

# 空间第二型曲线积分计算

<ul>

使用斯托克斯公式。

</ul>