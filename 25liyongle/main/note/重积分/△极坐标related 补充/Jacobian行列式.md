<div style="float: left; width: 64%; padding: 1%;">

## why面积元的变化 由Jacobian行列式给出

描述了坐标变换中 局部几何形状的 缩放和旋转效应。

---

### 1. 面积元与坐标变换
在二维空间中，假设我们从一个坐标系 $(u, v)$ 转换到另一个坐标系 $(x, y)$，并且这两个坐标系之间的关系由函数 $x = x(u, v)$ 和 $y = y(u, v)$ 给出。

那么，在新的坐标系 $(u, v)$ 中的一个小区域（面积元）对应于原坐标系 $(x, y)$ 中的一个小区域。

为了理解这种对应关系，我们需要知道：
- 在 $(u, v)$ 坐标系中，一个小矩形的边长分别为 $du$ 和 $dv$。
- 在 $(x, y)$ 坐标系中，这个小矩形被映射为一个平行四边形。

因此，面积元的变化取决于这个映射如何改变形状和大小，而雅可比行列式正是用来量化这种变化的工具。

---

### 2. 雅可比行列式的定义
Jacobian determinant是 两个向量偏导数的叉积模长，用于衡量局部面积的变化。

对于变换 $x = x(u, v)$ 和 $y = y(u, v)$，雅可比行列式定义为：
$$
J = \frac{\partial (x, y)}{\partial (u, v)} = 
\begin{vmatrix}
\frac{\partial x}{\partial u} & \frac{\partial x}{\partial v} \\
\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}
\end{vmatrix}
$$

$$
= \frac{\partial x}{\partial u} \frac{\partial y}{\partial v} - \frac{\partial x}{\partial v} \frac{\partial y}{\partial u}
$$

其值表示从 $(u, v)$ 到 $(x, y)$ 的坐标变换对面积的缩放因子。
-  $|J| > 1$，则面积被 放大
-  $|J| < 1$，则面积被 缩小

---

### 3. 几何解释：面积的缩放
在 $(u, v)$ 坐标系中，一个小矩形的边可以看作是两条向量：
$$
\mathbf{v}_1 = \left( \frac{\partial x}{\partial u}, \frac{\partial y}{\partial u} \right) du,
$$
$$
\mathbf{v}_2 = \left( \frac{\partial x}{\partial v}, \frac{\partial y}{\partial v} \right) dv.
$$

在 $(x, y)$ 坐标系中，这个小矩形被映射为一个平行四边形，其面积由这两个向量的叉积模长给出：
$$
\text{面积} = |\mathbf{v}_1 \times \mathbf{v}_2|.
$$

计算叉积模长时，结果正好等于雅可比行列式的绝对值乘以 $du \, dv$：
$$
|\mathbf{v}_1 \times \mathbf{v}_2| = |J| \, du \, dv.
$$

因此，在新的坐标系中，面积元变为：
$$
dx \, dy = |J| \, du \, dv.
$$

---

### 4. 物理意义
描述坐标变换对局部几何形状的影响：
- 雅可比行列式为正，则变换保持方向（右手系到右手系）。
- ..负，则变换反转方向（右手系到左手系）。
- 其绝对值
  - 表示面积的 缩放比例

---
### 5. pic

<div style="display: flex; justify-content: space-between; gap: 10px;">
  <img src="https://bluejedis.github.io/picx-images-hosting/Math/image.39ldg7sejy.png" alt="图1" style="flex: 1; max-width: 32%;"/>
  <img src="https://bluejedis.github.io/picx-images-hosting/Math/image.3rbf4suffm.png" alt="图2" style="flex: 1; max-width: 32%;"/>
  <img src="https://bluejedis.github.io/picx-images-hosting/Math/image.7lk6nrd5cr.png" alt="图3" style="flex: 1; max-width: 32%;"/>
</div>


1. 在 \((u, v)\) 坐标系中绘制一个小矩形，边长为 \(du\) 和 \(dv\)。
2. 在 \((x, y)\) 坐标系中绘制对应的平行四边形，边由变换后的向量表示。
3. 标注向量 \(\mathbf{v}_1\) 和 \(\mathbf{v}_2\)，并说明雅可比行列式 \(|J|\) 的作用。


为了简化，假设一个具体的坐标变换：
$$
x = 2u + v, \quad y = u + 3v
$$
其雅可比行列式为：
$$
J = \begin{vmatrix}
\frac{\partial x}{\partial u} & \frac{\partial x}{\partial v} \\
\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}
\end{vmatrix} = \begin{vmatrix}
2 & 1 \\
1 & 3
\end{vmatrix} = 2 \cdot 3 - 1 \cdot 1 = 5
$$
因此，面积缩放因子为 \(|J| = 5\)。

1. **\((u, v)\) 坐标系**：
   - 绘制一个小矩形，起点为 \((1, 1)\)，边长 \(du = 0.5\), \(dv = 0.5\)。
   - 用蓝色填充表示面积元 \(du \, dv\)。
   - 添加坐标轴和标注。

2. **\((x, y)\) 坐标系**：
   - 使用变换 \(x = 2u + v\), \(y = u + 3v\)。
   - 起点 \((u, v) = (1, 1)\) 映射到 \((x, y) = (3, 4)\)。
   - 向量 \(\mathbf{v}_1 = \left( \frac{\partial x}{\partial u}, \frac{\partial y}{\partial u} \right) \cdot du = (2, 1) \cdot 0.5 = (1, 0.5)\)。
   - 向量 \(\mathbf{v}_2 = \left( \frac{\partial x}{\partial v}, \frac{\partial y}{\partial v} \right) \cdot dv = (1, 3) \cdot 0.5 = (0.5, 1.5)\)。
   - 平行四边形顶点通过向量加法计算。
   - 用红色填充表示变换后的面积元。


---

### 总结

1. 雅可比行列式量化了坐标变换对局部几何形状的影响。
2. 它描述了从一个坐标系到另一个坐标系中，面积元如何被缩放和旋转。

因此，对于任意坐标变换，面积元的关系总是可以写成：
$$
\boxed{dx \, dy = |J| \, du \, dv.}
$$


</div>
<div style="float: right; width: 26%; padding: 1%;">

对于任意坐标变换，面积元的关系总是可以写成：
$$
dx \, dy = |J| \, du \, dv
$$


</div>
<div style="clear: both;"></div>
