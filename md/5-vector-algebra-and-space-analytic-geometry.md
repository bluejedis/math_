# 向量代数

<ul>

## 向量及其表达形式

<ul>

**定义：** 既有方向又有大小的量称为**向量**。  
向量的相等性体现在大小和方向，与空间位置无关。  
向量表达形式为 $\vec{a} = (a_x, a_y, a_z) = a_x \vec{i} + a_y \vec{j} + a_z \vec{k}$。

</ul>

## 向量运算

<ul>

设 $\vec{a} = (a_x, a_y, a_z)$，$\vec{b} = (b_x, b_y, b_z)$，$\vec{c} = (c_x, c_y, c_z)$，且 $\vec{a}, \vec{b}, \vec{c}$ 均不为零向量。

### 数量积

<ul>

也称为内积或点积。  
- $\vec{a} \cdot \vec{b} = (a_x, a_y, a_z) \cdot (b_x, b_y, b_z) = a_x b_x + a_y b_y + a_z b_z$  
- $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos \theta$，其中 $\theta$ 为 $\vec{a}, \vec{b}$ 的夹角  
- $a \perp b \Leftrightarrow \theta = \frac{\pi}{2} \Leftrightarrow \vec{a} \cdot \vec{b} = 0 \Leftrightarrow a_x b_x + a_y b_y + a_z b_z = 0$  
- $Prj_b a = \frac{\vec{a} \cdot \vec{b}}{|\vec{b}|} = \frac{a_x b_x + a_y b_y + a_z b_z}{\sqrt{b_x^2 + b_y^2 + b_z^2}}$ 称为 $\vec{a}$ 在 $\vec{b}$ 上的**投影**

</ul>

### 向量积

<ul>

也称为外积或叉积。  
- $\vec{a} \times \vec{b} = \begin{vmatrix} \vec{i} & \vec{j} & \vec{k} \\ a_x & a_y & a_z \\ b_x & b_y & b_z \end{vmatrix}$，且 $|\vec{a} \times \vec{b}| = |\vec{a}| |\vec{b}| \sin \theta$，方向由右手定则确定（转向角不超过 $\pi$）  
- $\vec{a} \parallel \vec{b} \Leftrightarrow \theta = 0 \text{ 或 } \pi \Leftrightarrow \vec{a} \times \vec{b} = 0 \Leftrightarrow \frac{a_x}{b_x} = \frac{a_y}{b_y} = \frac{a_z}{b_z}$  
- $\vec{a} \times \vec{a} = 0$

向量积的计算也可通过以下方式理解：将两个向量上下排列并复制右半部分：  
$\begin{bmatrix} a_x & a_y & a_z & a_x & a_y & a_z \\ b_x & b_y & b_z & b_x & b_y & b_z \end{bmatrix}$，  
- 第一个分量为第 2、3 列的行列式值  
- 第二个分量为第 3、4 列的行列式值  
- 第三个分量为第 4、5 列的行列式值（第 1 和第 6 列不用）

</ul>

### 混合积

<ul>

- $[\vec{a} \vec{b} \vec{c}] = (\vec{a} \times \vec{b}) \cdot \vec{c} = \begin{vmatrix} a_x & a_y & a_z \\ b_x & b_y & b_z \\ c_x & c_y & c_z \end{vmatrix}$  
- 交换两行不改变值：$\vec{a} \cdot (\vec{b} \times \vec{c}) = \vec{b} \cdot (\vec{c} \times \vec{a}) = \vec{c} \cdot (\vec{a} \times \vec{b})$  
- 交换一行改变符号：$\vec{a} \cdot (\vec{b} \times \vec{c}) = -\vec{a} \cdot (\vec{c} \times \vec{b}) = -\vec{b} \cdot (\vec{a} \times \vec{c}) = -\vec{c} \cdot (\vec{b} \times \vec{a})$  
- $[\vec{a} \vec{b} \vec{c}] = 0 \Leftrightarrow$ 三个向量共面

</ul>

</ul>

## 向量方向角与方向余弦

<ul>

- $\vec{a}$ 与 $x$ 轴、$y$ 轴、$z$ 轴正向的夹角 $\alpha, \beta, \gamma$ 为**方向角**  
- $\cos \alpha, \cos \beta, \cos \gamma$ 为**方向余弦**，且 $\cos \alpha = \frac{a_x}{|\vec{a}|}$，$\cos \beta = \frac{a_y}{|\vec{a}|}$，$\cos \gamma = \frac{a_z}{|\vec{a}|}$  
- $\vec{a}^\circ = \frac{\vec{a}}{|\vec{a}|} = (\cos \alpha, \cos \beta, \cos \gamma)$ 为**单位向量**（表示方向的向量）  
- 任意向量 $\vec{r} = x \vec{i} + y \vec{j} + z \vec{k} = r (\cos \alpha, \cos \beta, \cos \gamma)$，其中 $r = \sqrt{x^2 + y^2 + z^2}$，$\cos \alpha = \frac{x}{r}$，$\cos \beta = \frac{y}{r}$，$\cos \gamma = \frac{z}{r}$

</ul>

</ul>

# 空间解析几何

<ul>

## 平面方程

<ul>

设平面的法向量 $\vec{n} = (A, B, C)$。  
- **一般式：** $A x + B y + C z + D = 0$  
- **点法式：** $A (x - x_0) + B (y - y_0) + C (z - z_0) = 0$  
- **三点式：** $\begin{vmatrix} x - x_1 & y - y_1 & z - z_1 \\ x - x_2 & y - y_2 & z - z_2 \\ x - x_3 & y - y_3 & z - z_3 \end{vmatrix} = 0$（过不共线三点）  
- **截距式：** $\frac{x}{a} + \frac{y}{b} + \frac{z}{c} = 1$（过 $(a, 0, 0), (0, b, 0), (0, 0, c)$）

</ul>

## 直线方程

<ul>

设直线的方向向量 $\vec{\tau} = (l, m, n)$。  
- **一般式：** $\begin{cases} A_1 x + B_1 y + C_1 z + D_1 = 0 \\ A_2 x + B_2 y + C_2 z + D_2 = 0 \end{cases}$，其中 $\vec{\tau} = \vec{n}_1 \times \vec{n}_2$，$\vec{n}_1 = (A_1, B_1, C_1)$，$\vec{n}_2 = (A_2, B_2, C_2)$（两个平面的交线）  
- **点向式（标准式、对称式）：** $\frac{x - x_0}{l} = \frac{y - y_0}{m} = \frac{z - z_0}{n}$  
- **参数式：** $\begin{cases} x = x_0 + l t \\ y = y_0 + m t \\ z = z_0 + n t \end{cases}$，$t$ 为参数  
- **两点式：** $\frac{x - x_1}{x_2 - x_1} = \frac{y - y_1}{y_2 - y_1} = \frac{z - z_1}{z_2 - z_1}$（过两点）

</ul>

## 位置关系

<ul>

### 直线关系

<ul>

设 $\vec{\tau}_1 = (l_1, m_1, n_1)$，$\vec{\tau}_2 = (l_2, m_2, n_2)$ 分别为直线 $L_1, L_2$ 的方向向量。  
- $L_1 \perp L_2 \Leftrightarrow \vec{\tau}_1 \cdot \vec{\tau}_2 = 0 \Leftrightarrow l_1 l_2 + m_1 m_2 + n_1 n_2 = 0$  
- $L_1 \parallel L_2 \Leftrightarrow \vec{\tau}_1 \parallel \vec{\tau}_2 \Leftrightarrow \frac{l_1}{l_2} = \frac{m_1}{m_2} = \frac{n_1}{n_2}$

</ul>

### 平面关系

<ul>

设平面 $\pi_1, \pi_2$ 的法向量分别为 $\vec{n}_1 = (A_1, B_1, C_1)$，$\vec{n}_2 = (A_2, B_2, C_2)$。  
- $\pi_1 \perp \pi_2 \Leftrightarrow \vec{n}_1 \cdot \vec{n}_2 = 0 \Leftrightarrow A_1 A_2 + B_1 B_2 + C_1 C_2 = 0$  
- $\pi_1 \parallel \pi_2 \Leftrightarrow \vec{n}_1 \parallel \vec{n}_2 \Leftrightarrow \frac{A_1}{A_2} = \frac{B_1}{B_2} = \frac{C_1}{C_2}$

</ul>

### 直线与平面关系

<ul>

设直线 $L$ 的方向向量为 $\vec{\tau} = (l, m, n)$，平面 $\pi$ 的法向量为 $\vec{n} = (A, B, C)$。  
- $L \perp \pi \Leftrightarrow \vec{\tau} \parallel \vec{n} \Leftrightarrow \frac{A}{l} = \frac{B}{m} = \frac{C}{n}$  
- $L \parallel \pi \Leftrightarrow \vec{\tau} \perp \vec{n} \Leftrightarrow A l + B m + C n = 0$

</ul>

### 距离

<ul>

- **二维点到直线距离：** 点 $P_0(x_0, y_0)$ 到直线 $A x + B y + C = 0$ 的距离 $d = \frac{|A x_0 + B y_0 + C|}{\sqrt{A^2 + B^2}}$  
- **三维点到平面距离：** 点 $P_0(x_0, y_0, z_0)$ 到平面 $A x + B y + C z + D = 0$ 的距离 $d = \frac{|A x_0 + B y_0 + C z_0 + D|}{\sqrt{A^2 + B^2 + C^2}}$  
- **二维平行直线距离：** 直线 $A x + B y + C_1 = 0$ 到 $A x + B y + C_2 = 0$ 的距离 $d = \frac{|C_2 - C_1|}{\sqrt{A^2 + B^2}}$  
- **二维直线夹角：** 直线 $A_1 x + B_1 y + C_1 = 0$ 与 $A_2 x + B_2 y + C_2 = 0$ 的夹角 $\cos \theta = \frac{|A_1 A_2 + B_1 B_2|}{\sqrt{A_1^2 + B_1^2} \cdot \sqrt{A_2^2 + B_2^2}}$ ($\theta \in [0, \frac{\pi}{2}]$)  
- **三维平行平面距离：** 平面 $A x + B y + C z + D_1 = 0$ 到 $A x + B y + C z + D_2 = 0$ 的距离 $d = \frac{|D_2 - D_1|}{\sqrt{A^2 + B^2 + C^2}}$

**三维点到直线距离：**  
1. 由直线 $L$ 的一般式方程求出两个平面的法向量 $\vec{\xi_1}, \vec{\xi_2}$  
2. 计算方向向量 $\vec{S} = \vec{\xi_1} \times \vec{\xi_2}$  
3. 在 $L$ 上任取一点 $M_0$，计算 $\overrightarrow{M_0 M_1} \times \vec{S}$ 的模  
4. 距离 $d = \frac{|\overrightarrow{M_0 M_1} \times \vec{S}|}{|\vec{S}|}$

</ul>

</ul>

## 空间曲线

<ul>

空间曲线某点的切线向量为其参数方程在该点的导数。

### 表达式

<ul>

- **一般式：** $\Gamma: \begin{cases} F(x, y, z) = 0 \\ G(x, y, z) = 0 \end{cases}$（两个曲面的交线）  
- **参数方程：** $\Gamma: \begin{cases} x = \phi(t) \\ y = \psi(t) \\ z = \omega(t) \end{cases}$，$t \in [\alpha, \beta]$

</ul>

### 空间曲线在坐标面投影

<ul>

例如，求曲线 $\Omega$ 在 $xOy$ 面上的投影：  
消去 $z$，得 $\varphi(x, y) = 0$，则投影曲线包含于 $\begin{cases} \varphi(x, y) = 0 \\ z = 0 \end{cases}$。

</ul>

</ul>

## 空间曲面

<ul>

### 曲面方程

<ul>

- **隐式：** $F(x, y, z) = 0$  
- **显式：** $z = z(x, y)$

</ul>

### 二次曲面

<ul>

- **球面：** $x^2 + y^2 + z^2 = r^2$  
- **椭球面：** $\frac{x^2}{a^2} + \frac{y^2}{b^2} + \frac{z^2}{c^2} = 1$  
- **单叶双曲面：** $\frac{x^2}{a^2} + \frac{y^2}{b^2} - \frac{z^2}{c^2} = 1$  
- **双叶双曲面：** $\frac{x^2}{a^2} - \frac{y^2}{b^2} - \frac{z^2}{c^2} = 1$  
- **椭圆抛物面：** $\frac{x^2}{2p} + \frac{y^2}{2q} = z$（$p, q > 0$，常考旋转抛物面 $x^2 + y^2 = z$）  
- **椭圆锥面：** $\frac{x^2}{a^2} + \frac{y^2}{b^2} = \frac{z^2}{c^2}$（常考旋转锥面 $z = \sqrt{x^2 + y^2}$）  
- **双曲抛物面（马鞍面）：** $-\frac{x^2}{2p} + \frac{y^2}{2q} = z$（$p, q > 0$，可能考 $z = xy$）

</ul>

### 柱面

<ul>

缺少变量的方程通常为柱面，表示动直线沿定曲线平行移动形成的曲面。  
- **椭圆柱面：** $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$（$a = b$ 为圆柱面）  
- **双曲柱面：** $\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1$  
- **抛物柱面：** $y = a x^2$

</ul>

### 旋转曲面

<ul>

曲线绕定直线旋转一周形成的曲面。例如，$f(x, y) = 0$ 绕 $x$ 轴旋转得 $f(x, \pm \sqrt{y^2 + z^2}) = 0$。

**求解步骤：**  
1. 设直线 $L: \frac{x - x_0}{l} = \frac{y - y_0}{m} = \frac{z - z_0}{n}$，方向向量 $\vec{\tau} = (l, m, n)$，上一点 $P_0(x_0, y_0, z_0)$  
2. 曲线 $\Gamma: \begin{cases} F(x, y, z) = 0 \\ G(x, y, z) = 0 \end{cases}$ 上一点 $P_1(x_1, y_1, z_1)$  
3. $P_1$ 绕 $L$ 旋转一周得纬圆，任取 $P(x, y, z)$  
4. 距离相等：$(x_1 - x_0)^2 + (y_1 - y_0)^2 + (z_1 - z_0)^2 = (x - x_0)^2 + (y - y_0)^2 + (z - z_0)^2$  
5. 纬圆平面与 $L$ 垂直：$\vec{\tau} \cdot \overrightarrow{P_1 P} = 0$，即 $l (x - x_1) + m (y - y_1) + n (z - z_1) = 0$  
6. 消去 $x_1, y_1, z_1$ 得曲面方程 $H(x, y, z) = 0$

**例题：** 求曲线 $L: \begin{cases} x - y + 2z - 1 = 0 \\ x - 3y - 2z + 1 = 0 \end{cases}$ 绕 $y$ 轴旋转一周形成的曲面方程。  
**解：**  
- 令 $P_1(x_1, y_1, z_1)$ 在曲线上：$x_1 - y_1 + 2z_1 - 1 = 0$，$x_1 - 3y_1 - 2z_1 + 1 = 0$  
- 取 $P_0(0, 0, 0)$，则 $x_1^2 + y_1^2 + z_1^2 = x^2 + y^2 + z^2$  
- 绕 $y$ 轴旋转，$\overrightarrow{P_1 P} \perp (0, 1, 0)$，即 $y = y_1$  
- 由 $y = y_1$，$x_1^2 + z_1^2 = x^2 + z^2$  
- 解交线方程得 $x_1 = 2y_1$，$z_1 = \frac{1 - y_1}{2}$  
- 代入得 $x^2 + z^2 = (2y_1)^2 + \left( \frac{1 - y_1}{2} \right)^2$，化简为 $x^2 - \frac{17}{4} y^2 + z^2 + \frac{y}{2} - \frac{1}{4} = 0$

</ul>

</ul>

</ul>

# 场论初步

<ul>

## 方向导数

<ul>

偏导数是函数在坐标轴方向上的变化率，方向导数是函数在某点沿其他特定方向上的变化率。

**定义：** 设函数 $u = u(x, y, z)$ 在点 $P_0(x_0, y_0, z_0)$ 的空间领域 $U \in \mathbb{R}^3$ 内有定义，$l$ 为从 $P_0$ 出发的射线，$P(x, y, z)$ 为 $l$ 上在 $U$ 内的点，则：  
$$
\begin{cases}
x - x_0 = t \cos \alpha \\
y - y_0 = t \cos \beta \\
z - z_0 = t \cos \gamma
\end{cases}, \quad t = \sqrt{(\Delta x)^2 + (\Delta y)^2 + (\Delta z)^2}
$$  
若极限 $\lim_{t \to 0^+} \frac{u(P) - u(P_0)}{t}$ 存在，则称此极限为 $u$ 在 $P_0$ 沿 $l$ 的**方向导数**，记为 $\frac{\partial u}{\partial l} \big|_{P_0}$。

**计算公式：** 若 $u$ 在 $P_0$ 可微，则 $\frac{\partial u}{\partial l} \big|_{P_0} = u_x'(P_0) \cos \alpha + u_y'(P_0) \cos \beta + u_z'(P_0) \cos \gamma$，其中 $\cos \alpha, \cos \beta, \cos \gamma$ 为 $l$ 的方向余弦。

**例题：** 求 $z = x e^{2y}$ 在 $P(1, 0)$ 沿 $P(1, 0)$ 指向 $Q(2, -1)$ 方向的方向导数。  
**解：**  
- $\frac{\partial z}{\partial x} = e^{2y}$，$\frac{\partial z}{\partial y} = 2x e^{2y}$，在 $P(1, 0)$ 处为 $\{1, 2\}$  
- $\overrightarrow{PQ} = (1, -1)$，方向余弦 $\left\{ \frac{1}{\sqrt{2}}, -\frac{1}{\sqrt{2}} \right\}$  
- 方向导数：$1 \cdot \frac{1}{\sqrt{2}} + 2 \cdot \left( -\frac{1}{\sqrt{2}} \right) = -\frac{\sqrt{2}}{2}$

</ul>

## 梯度

<ul>

**定义：** 设函数 $u = u(x, y, z)$ 在 $P_0(x_0, y_0, z_0)$ 有一阶偏导数，定义 $\text{grad}\, u \big|_{P_0} = (u_x'(P_0), u_y'(P_0), u_z'(P_0))$ 为 $u$ 在 $P_0$ 的**梯度**。

</ul>

## 方向导数与梯度关系

<ul>

方向导数为梯度与方向余弦的点积。  
函数在某点的梯度是一个向量，其方向与取得最大方向导数的方向一致，模为方向导数的最大值。

</ul>

## 散度与旋度

<ul>

**定义：** 设向量场 $\vec{A}(x, y, z) = (P(x, y, z), Q(x, y, z), R(x, y, z))$，则：  
- **散度：** $\text{div}\, \vec{A} = \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} + \frac{\partial R}{\partial z}$  
- **旋度：** $\overrightarrow{\text{rot}}\, \vec{A} = \begin{vmatrix} \vec{i} & \vec{j} & \vec{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ P & Q & R \end{vmatrix}$

</ul>

</ul>