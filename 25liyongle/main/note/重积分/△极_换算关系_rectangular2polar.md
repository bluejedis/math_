<div style="float: left; width: 64%; padding: 1%;">

##  <span style="color: silver;">积分 直角→极 计算
<ul>

###  <span style="color: silver;">题1$$\iint_D (x^2 + y^2) \, dx \, dy,$$ $ D $ 由不等式$$\sqrt{2x - x^2} \leq y \leq \sqrt{9 - x^2}$$在第一象限内确定。
<ul>

####  <span style="color: silver;">draw $ \color{gray}{D} $
1. **上边界**：$ y = \sqrt{9 - x^2} $，这是圆 $ x^2 + y^2 = 9 $ 的上半部分。
2. **下边界**：$ y = \sqrt{2x - x^2} $，这是圆 $ (x-1)^2 + y^2 = 1 $ 的上半部分。
3. **第一象限**：$ x \geq 0 $ 且 $ y \geq 0 $。

![](https://bluejedis.github.io/picx-images-hosting/Math/屏幕截图-2025-04-16-120818.7w70grqaup.png)

####  <span style="color: silver;"> 🌟$\color{greenyellow}r$ 区间 & $\theta$ ← is 上界 & 下界 
<ul>

$$
\iint_D (x^2 + y^2) \, dx \, dy = \iint_D r^2 \cdot r \, dr \, d\theta = \iint_D r^3 \, dr \, d\theta.
$$

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.6bh9j5f1wu.png)

↑ 数形结合

上界 $ r = 3 $
下界 $ r = 2 \cos \theta $



角度范围： $ 0 \leq \theta \leq \frac{\pi}{2} $。



则 积分区间:

$$
\iint_D r^3 \, dr \, d\theta = \int_0^{\frac{\pi}{2}} \int_{2 \cos \theta}^3 r^3 \, dr \, d\theta.
$$
</ul>

####  <span style="color: silver;">计算
<ul>

1. **内层积分（关于 $ r $）**：
   
   $$
   \int_{2 \cos \theta}^3 r^3 \, dr = \left[ \frac{r^4}{4} \right]_{2 \cos \theta}^3
   $$

   $
   = \frac{3^4}{4} - \frac{(2 \cos \theta)^4}{4} 
   $
   $
   = \frac{81}{4} - \frac{16 \cos^4 \theta}{4} = \frac{81}{4} - 4 \cos^4 \theta.
   $

1. **外层积分（关于 $ \theta $）**：
   $$
   \int_0^{\frac{\pi}{2}} \left( \frac{81}{4} - 4 \cos^4 \theta \right) d\theta
   $$

   $$
 = \frac{81}{4} \int_0^{\frac{\pi}{2}} d\theta - 4 \int_0^{\frac{\pi}{2}} \cos^4 \theta \, d\theta.
   $$
   - 第一项：
     $$
     \frac{81}{4} \int_0^{\frac{\pi}{2}} d\theta = \frac{81}{4} \cdot \frac{\pi}{2} = \frac{81\pi}{8}.
     $$
   - 第二项：利用 $\cos^4 \theta = \left( \frac{1 + \cos 2\theta}{2} \right)^2 = \frac{1 + 2 \cos 2\theta + \cos^2 2\theta}{4}$，进一步展开：
     $$
     \cos^4 \theta = \frac{1 + 2 \cos 2\theta + \frac{1 + \cos 4\theta}{2}}{4} = \frac{3}{8} + \frac{\cos 2\theta}{2} + \frac{\cos 4\theta}{8}.
     $$
     thus：
     $$
     \int_0^{\frac{\pi}{2}} \cos^4 \theta \, d\theta = \int_0^{\frac{\pi}{2}} \left( \frac{3}{8} + \frac{\cos 2\theta}{2} + \frac{\cos 4\theta}{8} \right) d\theta.
     $$
     各项积分分别为：
     $$
     \int_0^{\frac{\pi}{2}} \frac{3}{8} \, d\theta = \frac{3}{8} \cdot \frac{\pi}{2} = \frac{3\pi}{16},
     $$
     $$
     \int_0^{\frac{\pi}{2}} \frac{\cos 2\theta}{2} \, d\theta = \frac{1}{2} \left[ \frac{\sin 2\theta}{2} \right]_0^{\frac{\pi}{2}} = 0,
     $$
     $$
     \int_0^{\frac{\pi}{2}} \frac{\cos 4\theta}{8} \, d\theta = \frac{1}{8} \left[ \frac{\sin 4\theta}{4} \right]_0^{\frac{\pi}{2}} = 0.
     $$
</ul>
</ul>


###  <span style="color: silver;"> 题2 $$\int_{0}^{2} dx \int_{0}^{\sqrt{2x-x^{2}}} \sqrt{x^{2}+y^{2}} \, dy$$

<ul>

####  <span style="color: silver;">draw $ \color{gray}{D} $ 

约束条件: ← 根据一项 画一个limit

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.2a5a4u8hyr(1).64e1nt3ivj.png)


####  <span style="color: silver;">$\color{greenyellow}r$ 区间 & $\theta$

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.2a5a4u8hyr2.9kgdfwd9g9.png)

$\color{greenyellow}r$
- 上界: $2\cos \theta$
- 下界: $0$
<br>

$\theta \in [0, \frac{\pi}{2}]$



####  <span style="color: silver;">计算
<ul>

$$\int_{0}^{\frac{\pi}{2}} d\theta \int_{0}^{2 \cos \theta} r^2 \, dr$$

---
第二层$\int$:
$$\cos^3 \theta$$

$$ = \cos \theta \cdot \cos^2 \theta$$ 


$$
=\cos \theta (1 - \sin^2 \theta) 
$$


$$
= \cos \theta - \cos \theta \sin^2 \theta.
$$



令 $u = \sin \theta$，则 $du = \cos \theta \, d\theta$
- 当 $\theta = 0$ 时，$u = 0$；当 $\theta = \frac{\pi}{2}$ 时，$u = 1$

则 $\int_0^{\frac{\pi}{2}} \cos \theta \sin^2 \theta \, d\theta$

$$
\int_0^{\frac{\pi}{2}} \cos \theta \sin^2 \theta \, d\theta = \int_0^1 u^2 \, du.
$$

</ul>



</ul>




</div>
<div style="float: right; width: 26%; padding: 1%;">

##  <span style="color: silver;">key

###  <span style="color: silver;">$dx \, dy = r \, dr \, d\theta$ $$x = r \cos \theta, \quad y = r \sin \theta, \quad $$
将直角坐标 $(x, y)$ 转换为极坐标 $(r, \theta)$：
$$
x = r \cos \theta, \quad y = r \sin \theta, \quad 
$$


$$
dx \, dy = r \, dr \, d\theta.
$$


---


###  <span style="color: silver;">极径$\color{greenyellow}r$ 的区间 is 上下界

<ul>

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.92qbr87467.png)

- 极坐标中only care for $r$ $\theta$
<br>

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.6bh9j5f1wu.png)

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.7zqmfu59gy.png)

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.2a5a4u8hyr2.9kgdfwd9g9.png)

</ul>

###  <span style="color: silver;">$\int_0^{\frac{\pi}{2}} \cos^4 \theta \, d\theta$

积分计算:
高次 降次 三角函数 avoid换元法
<br>
$\cos^4 \theta = \left( \frac{1 + \cos 2\theta}{2} \right)^2 = \frac{1 + 2 \cos 2\theta + \cos^2 2\theta}{4}$


---
###  <span style="color: silver;">$\int_0^{\frac{\pi}{2}} \cos^3 \theta \, d\theta$

<ul>

####  <span style="color: silver;">sin²θ+cos²θ=1⇒cos²θ=1-sin²θ _换元法_ 令u=sinθ 求积分

</ul>

</div>
<div style="clear: both;"></div>
