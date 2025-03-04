# 基本概念

<ul>

## 平面与点

<ul>

### 平面点集

<ul>

<span style="color: violet">**定义：**</span> 在平面上建立直角坐标系 $xOy$，则平面上的点可用两个实数组成的有序数组 $(x,y)$ 表示，而二元函数 $f(x,y)$ 的定义域是以 $(x,y)$ 为元素的几何集合，因此 $f(x,y)$ 的定义域就是**平面上的点集**。

</ul>

### 距离

<ul>

<span style="color: aqua">**定理：**</span> 平面上任意两点 $M_1(x_1,y_1)$ 与 $M_2(x_2,y_2)$ 之间的距离定义为：

$$
\rho(M_1,M_2) = \sqrt{(x_2-x_1)^2 + (y_2-y_1)^2}
$$

$\rho(M_1,M_2)$ 满足以下性质：

- **非负性**：$\rho(M_1,M_2) \geqslant 0$。
- **对称性**：$\rho(M_1,M_2) = \rho(M_2,M_1)$。
- **三角不等式**：$\rho(M_1,M_3) \leqslant \rho(M_1,M_2) + \rho(M_2,M_3)$。

</ul>

### 邻域

<ul>

设 $M_0$ 为平面上一点，$\delta > 0$，则平面上以 $M_0$ 为圆心，$\delta$ 为半径的圆的内部称为 $M_0$ 的**$\delta$ 邻域**，记为 $U(M_0,\delta)$。

若领域中去掉圆心 $M_0$，称为 $M_0$ 的**$\delta$ 去心邻域**，记为 $\mathring{U}(M_0,\delta)$。

</ul>

### 点的分类

<ul>

<span style="color: violet">**定义：**</span> 设 $M$ 为平面上一个点，若存在 $\delta > 0$，使得 $U(M,\delta) \subset E$，则 $M$ 为点集 $E$ 的**内点**。

<span style="color: violet">**定义：**</span> 若存在 $\delta > 0$，使得 $U(M,\delta) \cap E = \varnothing$，则 $M$ 为点集 $E$ 的**外点**。

<span style="color: violet">**定义：**</span> 若对任意 $\delta > 0$，$U(M,\delta)$ 既有 $E$ 内的点也有 $E$ 外的点，则 $M$ 为点集 $E$ 的**边界点**。

<span style="color: violet">**定义：**</span> $E$ 所有边界点的集合称为 $E$ 的**边界**，记为 $\partial E$。对于任意一个点集 $E$ 与其补集 $E^C$ 有公共边界，即 $\partial E = \partial E^C$。

</ul>

### 集合

<ul>

<span style="color: violet">**定义：**</span> 设 $E$ 为一个平面点集，若存在常数 $\delta > 0$，使得 $E \subset U(O,\delta)$，则 $E$ 为**有界集**，否则为**无界集**。

<span style="color: violet">**定义：**</span> 若 $E$ 中的每个点都是 $E$ 的内点，则 $E$ 为**开集**；若 $E$ 的边界点都是 $E$ 的点，则 $E$ 为**闭集**。若一个点集是开集，则其补集为闭集；若一个点集为闭集，则其补集为开集。

<span style="color: violet">**定义：**</span> 若 $E$ 中任意两点，都可用一条完全属于 $E$ 的曲线连接，则 $E$ 为**（道路）连通集**。连通的开集为**开区域**，一个开区域与其边界点的并集为**闭区域**，统称**区域**。

<span style="color: violet">**定义：**</span> 若 $E$ 内任意一条**简单闭曲线**的内部仍在 $E$ 内，则 $E$ 为**单连通区域**，否则为**多连通区域**。

</ul>

### 聚点

<ul>

<span style="color: violet">**定义：**</span> 对一个平面点集 $E$，$M_0$ 为平面上一点，若对任意 $\delta > 0$，总有 $\mathring{U}(M_0,\delta) \cap E \neq \varnothing$，即 $M_0$ 的任意邻域中都含有异于 $M_0$ 的 $E$ 中的点，则 $M_0$ 为 $E$ 的**聚点**。

<span style="color: aqua">**定理：**</span> 非空开集的内点及边界点都是该点集的聚点，闭区域的任意一点都是其聚点。

<span style="color: violet">**定义：**</span> 若存在 $\delta > 0$，使得 $U(M_0,\delta) \cap E = \{M_0\}$，即 $M_0$ 的某一邻域与点集 $E$ 的交集仅为孤立点 $M_0$，则称 $M_0$ 为 $E$ 的**孤立点**。边界点要么是聚点，要么是孤立点。

</ul>

</ul>

## 极限

<ul>

对于一元函数的极限，可用列举法从两端逼近该点取极限。但对于多元函数，其邻域逼近方向无穷多，因此无法通过仅取两个方向逼近的方式求极限。

从点集来看，<span style="color: violet">**定义：**</span> 设二元函数 $f(P) = f(x,y)$ 的定义域为 $D$，$P_0(x_0,y_0)$ 为 $D$ 的聚点。若存在常数 $A$，对于任意给定正数 $\epsilon$，总存在正数 $\delta$，使得当 $P(x,y) \in D \cap \mathring{U}(P_0,\delta)$ 时，都有 $|f(x,y) - A| < \epsilon$ 成立，则常数 $A$ 为 $f(x,y)$ 当 $(x,y) \rightarrow (x_0,y_0)$ 时的极限，记为：

$$
\lim_{(x,y) \to (x_0,y_0)} f(x,y) = A \quad \text{或} \quad f(x,y) \to A \ ((x,y) \to (x_0,y_0))
$$

例如：

$$
\lim_{(x,y) \to (0,0)} \frac{\sqrt{xy+1} - 1}{xy} = \lim_{(x,y) \to (0,0)} \frac{xy + 1 - 1}{xy (\sqrt{xy+1} + 1)} = \lim_{(x,y) \to (0,0)} \frac{1}{\sqrt{xy+1} + 1} = \frac{1}{2}
$$

（因 $xy \neq 0$，排除 $xy$ 轴上的点）

从邻域来看，<span style="color: violet">**定义：**</span> 若二元函数 $f(x,y)$ 在 $(x_0,y_0)$ 的去心邻域内有定义，且 $(x,y)$ 以任意方式趋向 $(x_0,y_0)$ 时，$f(x,y)$ 均趋向于 $A$，则：

$$
\lim_{\substack{x \to x_0 \\ y \to y_0}} f(x,y) = A
$$

例如，对于 $\lim_{(x,y) \to (0,0)} \frac{\sqrt{xy+1} - 1}{xy}$，因其在坐标轴上无定义，极限不存在。

两种定义可能得出不同结论。为避免矛盾，通常只讨论某种定义下极限存在或都不存在的情况，例如：

$$
\lim_{\substack{x \to 0 \\ y \to 0}} (x^2 + y^2) \sin \frac{1}{x^2 + y^2} = 0
$$

从现实角度看，点集定义更合理。例如求一根弯曲铁丝在某点的导数，邻域定义无法适用，因此有局限性。

</ul>

## 连续

<ul>

<span style="color: violet">**定义：**</span> 若：

$$
\lim_{\substack{x \to x_0 \\ y \to y_0}} f(x,y) = f(x_0,y_0)
$$

则称 $f(x,y)$ 在点 $(x_0,y_0)$ 处**连续**。若不连续，则不讨论间断类型。

</ul>

## 偏导数

<ul>

当函数含多个变量时，若求极限，所有变量同时变化。为简化运算，假设仅一个变量变化，其余固定，降为一元函数求导，即**偏导数**。

<span style="color: violet">**定义：**</span> 设函数 $z = f(x,y)$ 在点 $(x_0,y_0)$ 的某邻域内有定义，若极限：

$$
\lim_{\Delta x \to 0} \frac{f(x_0 + \Delta x, y_0) - f(x_0, y_0)}{\Delta x}
$$

存在，则称此极限为 $z = f(x,y)$ 在点 $(x_0,y_0)$ 处对 $x$ 的**偏导数**，记为：

$$
\frac{\partial z}{\partial x} \bigg|_{\substack{x=x_0 \\ y=y_0}}, \quad \frac{\partial f}{\partial x} \bigg|_{\substack{x=x_0 \\ y=y_0}}, \quad z' \bigg|_{\substack{x=x_0 \\ y=y_0}}, \quad \text{或} \quad f'_x(x_0,y_0)
$$

即：

$$
f'_x(x_0,y_0) = \lim_{\Delta x \to 0} \frac{f(x_0 + \Delta x, y_0) - f(x_0, y_0)}{\Delta x} = \lim_{x \to x_0} \frac{f(x, y_0) - f(x_0, y_0)}{x - x_0}
$$

$$
f'_y(x_0,y_0) = \lim_{\Delta y \to 0} \frac{f(x_0, y_0 + \Delta y) - f(x_0, y_0)}{\Delta y} = \lim_{y \to y_0} \frac{f(x_0, y) - f(x_0, y_0)}{y - y_0}
$$

<span style="color: violet">**定义：**</span> 若函数 $z = f(x,y)$ 在区域 $D$ 内的偏导数 $f'_x(x,y)$、$f'_y(x,y)$ 仍具有偏导数，则其偏导数为 $z = f(x,y)$ 的**二阶偏导数**，按求导次序分为：

$$
\frac{\partial}{\partial x} \left( \frac{\partial z}{\partial x} \right) = \frac{\partial^2 z}{\partial x^2} = f''_{xx}(x,y)
$$

$$
\frac{\partial}{\partial y} \left( \frac{\partial z}{\partial y} \right) = \frac{\partial^2 z}{\partial y^2} = f''_{yy}(x,y)
$$

$$
\frac{\partial}{\partial y} \left( \frac{\partial z}{\partial x} \right) = \frac{\partial^2 z}{\partial x \partial y} = f''_{xy}(x,y)
$$

$$
\frac{\partial}{\partial x} \left( \frac{\partial z}{\partial y} \right) = \frac{\partial^2 z}{\partial y \partial x} = f''_{yx}(x,y)
$$

其中 $f''_{xy}(x,y)$ 和 $f''_{yx}(x,y)$ 为**混合偏导数**，二阶及以上偏导数统称**高阶偏导数**。

</ul>

## 全微分

<ul>

<span style="color: violet">**定义：**</span> 若函数 $z = f(x,y)$ 在点 $(x,y)$ 的全增量：

$$
\Delta z = f(x + \Delta x, y + \Delta y) - f(x, y)
$$

可表示为：

$$
\Delta z = A \Delta x + B \Delta y + o(\rho), \quad \text{其中} \ \rho = \sqrt{(\Delta x)^2 + (\Delta y)^2}
$$

且 $A$、$B$ 不依赖 $\Delta x$、$\Delta y$，仅与 $x$、$y$ 相关，则称 $z = f(x,y)$ 在点 $(x,y)$ **可微**，而 $A \Delta x + B \Delta y$ 为 $z = f(x,y)$ 在点 $(x,y)$ 的**全微分**，记为：

$$
\textrm{d}z = A \Delta x + B \Delta y = \frac{\partial z}{\partial x} \Delta x + \frac{\partial z}{\partial y} \Delta y = \frac{\partial z}{\partial x} \textrm{d}x + \frac{\partial z}{\partial y} \textrm{d}y
$$

**判断可微的步骤：**

1. 写出全增量：$\Delta z = f(x_0 + \Delta x, y_0 + \Delta y) - f(x_0, y_0)$。
2. 写出线性增量：$A \Delta x + B \Delta y$，其中 $A = f'_x(x_0, y_0)$，$B = f'_y(x_0, y_0)$。
3. 计算极限：

$$
\lim_{\substack{\Delta x \to 0 \\ \Delta y \to 0}} \frac{\Delta z - (A \Delta x + B \Delta y)}{\sqrt{(\Delta x)^2 + (\Delta y)^2}}
$$

若极限等于 0，则 $z = f(x,y)$ 在点 $(x_0, y_0)$ 可微，否则不可微。

</ul>

## 偏导数连续性

<ul>

对 $z = f(x,y)$，讨论其在某点 $(x_0, y_0)$ 处偏导数是否连续的步骤：

1. 用定义法求 $f'_x(x_0, y_0)$ 和 $f'_y(x_0, y_0)$（某点偏导数）。
2. 用公式法求 $f'_x(x,y)$ 和 $f'_y(x,y)$（偏导函数）。
3. 计算极限：

$$
\lim_{\substack{x \to x_0 \\ y \to y_0}} f'_x(x,y), \quad \lim_{\substack{x \to x_0 \\ y \to y_0}} f'_y(x,y)
$$

4. 若 $\lim_{\substack{x \to x_0 \\ y \to y_0}} f'_x(x,y) = f'_x(x_0, y_0)$ 且 $\lim_{\substack{x \to x_0 \\ y \to y_0}} f'_y(x,y) = f'_y(x_0, y_0)$ 成立，则连续，否则不连续。

**例题：** 设：

$$
z = f(x,y) = \begin{cases} 
(x^2 + y^2) \sin \frac{1}{\sqrt{x^2 + y^2}}, & x^2 + y^2 \neq 0 \\ 
0, & x^2 + y^2 = 0 
\end{cases}
$$

判断以下结论正确个数：

1. $f(x,y)$ 在 $(0,0)$ 处连续。
2. $f'_x(0,0)$ 和 $f'_y(0,0)$ 存在。
3. $f'_x(x,y)$ 和 $f'_y(x,y)$ 在 $(0,0)$ 处连续。
4. $f(x,y)$ 在 $(0,0)$ 可微。

选项：A. 1  B. 2  C. 3  D. 4

**解：**

- **连续性**：

$$
\lim_{\substack{x \to 0 \\ y \to 0}} (x^2 + y^2) \sin \frac{1}{\sqrt{x^2 + y^2}} = 0 = f(0,0)
$$

结论 1 正确。

- **偏导数存在性**：

$$
f'_x(0,0) = \lim_{\Delta x \to 0} \frac{f(\Delta x, 0) - f(0,0)}{\Delta x} = \lim_{\Delta x \to 0} \frac{(\Delta x)^2 \sin \frac{1}{|\Delta x|}}{\Delta x} = \lim_{\Delta x \to 0} \Delta x \sin \frac{1}{|\Delta x|} = 0
$$

同理 $f'_y(0,0) = 0$，结论 2 正确。

- **偏导数连续性**：

先求偏导函数：

$$
f'_x(x,y) = 2x \sin \frac{1}{\sqrt{x^2 + y^2}} - \frac{x}{\sqrt{x^2 + y^2}} \cos \frac{1}{\sqrt{x^2 + y^2}}
$$

$$
f'_y(x,y) = 2y \sin \frac{1}{\sqrt{x^2 + y^2}} - \frac{y}{\sqrt{x^2 + y^2}} \cos \frac{1}{\sqrt{x^2 + y^2}}
$$

计算极限：

$$
\lim_{\substack{x \to 0 \\ y \to 0}} f'_x(x,y) = \lim_{\substack{x \to 0 \\ y \to 0}} 2x \sin \frac{1}{\sqrt{x^2 + y^2}} - \lim_{\substack{x \to 0 \\ y \to 0}} \frac{x}{\sqrt{x^2 + y^2}} \cos \frac{1}{\sqrt{x^2 + y^2}}
$$

第一项为 0，第二项震荡无极限，总极限不存在，不等于 $f'_x(0,0) = 0$，故不连续。同理 $f'_y(x,y)$ 不连续，结论 3 错误。

- **可微性**：

全增量：

$$
\Delta z = (\Delta x^2 + \Delta y^2) \sin \frac{1}{\sqrt{\Delta x^2 + \Delta y^2}}
$$

线性增量：

$$
A \Delta x + B \Delta y = f'_x(0,0) \Delta x + f'_y(0,0) \Delta y = 0
$$

极限：

$$
\lim_{\substack{\Delta x \to 0 \\ \Delta y \to 0}} \frac{\Delta z}{\sqrt{(\Delta x)^2 + (\Delta y)^2}} = \lim_{\substack{\Delta x \to 0 \\ \Delta y \to 0}} \sqrt{\Delta x^2 + \Delta y^2} \sin \frac{1}{\sqrt{\Delta x^2 + \Delta y^2}} = 0
$$

可微，结论 4 正确。

**综上**：正确结论有 1、2、4，选 **C**。

</ul>

</ul>

---

# 多元函数微分法则

<ul>

## 链式求导法则

<ul>

多元函数链式求导类似一元函数，从因变量通过中间变量到自变量。每条路径为一个加项，每条路含多个乘项。例如：

若 $z$ 到 $x$ 有两条路 $z-u-x$ 和 $z-v-x$：

$$
\frac{\textrm{d}z}{\textrm{d}x} = \frac{\partial z}{\partial u} \frac{\textrm{d}u}{\textrm{d}x} + \frac{\partial z}{\partial v} \frac{\textrm{d}v}{\textrm{d}x}
$$

**例题：** 设 $z = f(e^x \sin y, x^2 + y^2)$，$f$ 具二阶连续偏导数，求 $\frac{\partial^2 z}{\partial x \partial y}$。

**解：**

$$
\frac{\partial z}{\partial x} = f'_1 e^x \sin y + f'_2 \cdot 2x
$$

$$
\frac{\partial^2 z}{\partial x \partial y} = \frac{\partial}{\partial y} (f'_1 e^x \sin y) + \frac{\partial}{\partial y} (f'_2 \cdot 2x)
$$

$$
= (f''_{11} e^x \cos y + f''_{12} \cdot 2y) e^x \sin y + f'_1 e^x \cos y + 2x (f''_{21} e^x \cos y + f''_{22} \cdot 2y)
$$

化简：

$$
= f'_1 e^x \cos y + f''_{11} e^{2x} \sin y \cos y + 2 e^x f''_{12} (y \sin y + x \cos y) + 4 f''_{22} xy
$$

</ul>

## 隐函数存在定理

<ul>

<span style="color: violet">**定义：**</span> 设 $F(x,y)$ 在 $(x_0,y_0)$ 邻域内具连续偏导数，$F(x_0,y_0) = 0$，$F'_y(x_0,y_0) \neq 0$，则 $F(x,y) = 0$ 在 $(x_0,y_0)$ 邻域内唯一确定一个连续且具连续导数的函数 $y = f(x)$。

**求导公式**：

$$
\frac{\textrm{d}y}{\textrm{d}x} = -\frac{F'_x}{F'_y}
$$

**例题：** 设 $z = f(x,y)$ 由 $z - y - x + x e^{z - y - x} = 0$ 确定，求 $\textrm{d}z$。

**解：**

$$
F'_x = -1 + e^{z-y-x} - x e^{z-y-x}, \quad F'_y = -1 - x e^{z-y-x}, \quad F'_z = 1 + x e^{z-y-x}
$$

$$
\textrm{d}z = \frac{\partial z}{\partial x} \textrm{d}x + \frac{\partial z}{\partial y} \textrm{d}y = -\frac{F'_x}{F'_z} \textrm{d}x - \frac{F'_y}{F'_z} \textrm{d}y
$$

</ul>

</ul>

---

# 多元函数极值最值

<ul>

## 概念

<ul>

<span style="color: violet">**定义：**</span> 若 $(x_0,y_0)$ 的某邻域内，$f(x,y) \leqslant f(x_0,y_0)$ 或 $f(x,y) \geqslant f(x_0,y_0)$，则 $(x_0,y_0)$ 为**广义极大值点/极小值点**。

</ul>

## 无条件极值

<ul>

<span style="color: aqua">**定理：**</span> 若 $z = f(x,y)$ 在 $(x_0,y_0)$ 取极值且一阶偏导存在，则 $f'_x(x_0,y_0) = 0$，$f'_y(x_0,y_0) = 0$。

<span style="color: aqua">**充分条件：**</span> 设 $A = f''_{xx}(x_0,y_0)$，$B = f''_{xy}(x_0,y_0)$，$C = f''_{yy}(x_0,y_0)$，$\Delta = B^2 - AC$：

- $\Delta < 0$：极值（$A < 0$ 为极大值，$A > 0$ 为极小值）。
- $\Delta > 0$：非极值。
- $\Delta = 0$：方法失效，用定义法。

### 显函数

<ul>

**例题：** 求 $f(x,y) = x^4 + y^4 - (x+y)^2$ 的极值。

**解：**

$$
f'_x = 4x^3 - 2(x+y) = 0, \quad f'_y = 4y^3 - 2(x+y) = 0
$$

解得 $x = y = -1, 0, 1$。二阶偏导：

$$
f''_{xx} = 12x^2 - 2, \quad f''_{xy} = -2, \quad f''_{yy} = 12y^2 - 2
$$

代入点 $(-1,-1)$：$\Delta = -96 < 0$，$A = 10 > 0$，极小值 $-2$。

</ul>

### 隐函数

<ul>

（此处原文未完成，可根据需要补充）

</ul>

</ul>

## 条件极值与拉格朗日乘数法

<ul>

构造辅助函数：

$$
F(x,y,z,\lambda_1,\ldots,\lambda_n) = f(x,y,z) + \sum_{i=1}^n \lambda_i \varphi_i(x,y,z)
$$

求偏导并令为 0，解方程组。

**例题：** 求 $u = xyz$ 在 $\frac{1}{x} + \frac{1}{y} + \frac{1}{z} = \frac{1}{a}$（$x,y,z,a > 0$）下的最小值。

**解：**

$$
F = xyz + \lambda \left( \frac{1}{x} + \frac{1}{y} + \frac{1}{z} - \frac{1}{a} \right)
$$

偏导为 0，解得 $x = y = z = 3a$，最小值 $27a^3$。

</ul>

</ul>