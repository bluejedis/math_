<div style="float: left; width: 64%; padding: 1%;">


### 1. 直角坐标与极坐标的转换关系
在极坐标中：
$$
x = r \cos \theta, \quad y = r \sin \theta,
$$
其中：
- $ r $ 是点到原点的距离（半径），
- $ \theta $ 是点与正 $ x $-轴之间的夹角。


---

### 2. 面积元的变换：雅可比行列式
在二维空间中，如果变量从 $(x, y)$ 转换为新的变量 $(r, \theta)$，那么面积元的变化可以由雅可比行列式给出：
$$
dx \, dy = \left| J \right| \, dr \, d\theta,
$$
其中雅可比行列式 $ J $ 定义为：
$$
J = \begin{vmatrix}
\frac{\partial x}{\partial r} & \frac{\partial x}{\partial \theta} \\
\frac{\partial y}{\partial r} & \frac{\partial y}{\partial \theta}
\end{vmatrix}.
$$

根据极坐标与直角坐标的关系：
$$
x = r \cos \theta, \quad y = r \sin \theta,
$$
我们可以计算出各偏导数：
$$
\frac{\partial x}{\partial r} = \cos \theta, \quad \frac{\partial x}{\partial \theta} = -r \sin \theta,
$$
$$
\frac{\partial y}{\partial r} = \sin \theta, \quad \frac{\partial y}{\partial \theta} = r \cos \theta.
$$

将这些偏导数代入雅可比行列式中：
$$
J = \begin{vmatrix}
\cos \theta & -r \sin \theta \\
\sin \theta & r \cos \theta
\end{vmatrix}.
$$

计算行列式的值：
$$
J = (\cos \theta)(r \cos \theta) - (-r \sin \theta)(\sin \theta),
$$
$$
J = r \cos^2 \theta + r \sin^2 \theta.
$$

利用三角恒等式 $\cos^2 \theta + \sin^2 \theta = 1$，得到：
$$
J = r.
$$

因此，面积元的变换为：
$$
dx \, dy = |J| \, dr \, d\theta = r \, dr \, d\theta.
$$

---

### 3. 几何解释
看作是一个小扇形区域的近似。

假设 $ r $ 和 $ \theta $ 的微小变化分别为 $ dr $ 和 $ d\theta $，则这个小扇形的面积为：
$$
\text{面积} = \text{半径} \times \text{弧长} = r \cdot (r \, d\theta).
$$

弧长为 $ r \, d\theta $，而宽度为 $ dr $。

故：
$$
dA = r \, dr \, d\theta.
$$





</div>
<div style="float: right; width: 26%; padding: 1%;">

- 几何:
  - $$dA = r \, dr \, d\theta.$$
    - 弧长 $ r \, d\theta $
    - 宽度 $ dr $
<br>

- 雅可比
  - $dx \, dy = |J| \, dr \, d\theta = r \, dr \, d\theta$

---
though极坐标 与 直角坐标 的图形状一样, but actually 还是坐标系转换
- 直角坐标 映射到 极坐标 (放大|J|= r)
  - 即 J决定的是 面积元 的变化

![a6a9e97b9e613144da210594eb64d8f8b97499b9](https://bluejedis.github.io/picx-images-hosting/Math/a6a9e97b9e613144da210594eb64d8f8b97499b9.gif@622w_518h.3rbf4v3yfl.gif)
</div>
<div style="clear: both;"></div>
